# Comparing `tmp/streamlit_chatbox-0.1.2-py3-none-any.whl.zip` & `tmp/streamlit_chatbox-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3996 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     7876 b- defN 23-May-30 10:02 streamlit_chatbox/__init__.py
--rw-rw-rw-  2.0 fat     1305 b- defN 23-May-30 10:11 streamlit_chatbox-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 10:11 streamlit_chatbox-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-May-30 10:11 streamlit_chatbox-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      424 b- defN 23-May-30 10:11 streamlit_chatbox-0.1.2.dist-info/RECORD
-5 files, 9715 bytes uncompressed, 3200 bytes compressed:  67.1%
+Zip file size: 4318 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     8577 b- defN 23-May-30 13:45 streamlit_chatbox/__init__.py
+-rw-rw-rw-  2.0 fat     1927 b- defN 23-May-31 04:24 streamlit_chatbox-0.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-31 04:24 streamlit_chatbox-0.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-May-31 04:24 streamlit_chatbox-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      424 b- defN 23-May-31 04:24 streamlit_chatbox-0.2.0.dist-info/RECORD
+5 files, 11038 bytes uncompressed, 3522 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: streamlit_chatbox/__init__.py
 Comment: 
 
-Filename: streamlit_chatbox-0.1.2.dist-info/METADATA
+Filename: streamlit_chatbox-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: streamlit_chatbox-0.1.2.dist-info/WHEEL
+Filename: streamlit_chatbox-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: streamlit_chatbox-0.1.2.dist-info/top_level.txt
+Filename: streamlit_chatbox-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: streamlit_chatbox-0.1.2.dist-info/RECORD
+Filename: streamlit_chatbox-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamlit_chatbox/__init__.py

```diff
@@ -95,41 +95,54 @@
     def render_msg(self,
                    msg,
                    is_user=False,
                    msg_type=MsgType.TEXT,
                    icon=None,
                    bg_color=None,
                    margin=None,
+                   **kw,
                    ):
         '''
-        渲染单条消息。目前仅支持文本
+        渲染单条消息。
         '''
         margin = margin or self.box_margin
         cols = st.columns([1, 10, 1])
         empty = cols[1].empty()
         if is_user:
             icon = icon or self.user_icon
             bg_color = bg_color or self.user_bg_color
             if icon:
                 cols[2].image(icon, width=40)
             if msg_type == MsgType.TEXT:
                 text = self.format_md(msg, is_user, bg_color, margin)
                 empty.markdown(text, unsafe_allow_html=True)
+            elif msg_type == MsgType.IMAGE:
+                empty.image(msg, use_column_width='auto')
+            elif msg_type == MsgType.VIDEO:
+                empty.video(msg, format=kw.get('format', 'video/mp4'))
+            elif msg_type == MsgType.AUDIO:
+                empty.audio(msg, format=kw.get('format', 'audio/wav'))
             else:
-                raise RuntimeError('only support text message now.')
+                raise RuntimeError(f'unsupported message type: {msg_type} .')
         else:
             icon = icon or self.robot_icon
             bg_color = bg_color or self.robot_bg_color
             if icon:
                 cols[0].image(icon, width=40)
             if msg_type == MsgType.TEXT:
                 text = self.format_md(msg, is_user, bg_color, margin)
                 empty.markdown(text, unsafe_allow_html=True)
+            elif msg_type == MsgType.IMAGE:
+                empty.image(msg, use_column_width='auto')
+            elif msg_type == MsgType.VIDEO:
+                empty.video(msg, format=kw.get('format', 'video/mp4'))
+            elif msg_type == MsgType.AUDIO:
+                empty.audio(msg, format=kw.get('format', 'audio/wav'))
             else:
-                raise RuntimeError('only support text message now.')
+                raise RuntimeError(f'unsupported message type: {msg_type} .')
         return empty
 
     def show_welcome(self):
         if self.greetings and not self.welcomed:
             greetings = self.greetings
             if not isinstance(greetings, list):
                 greetings = [greetings]
@@ -152,14 +165,15 @@
                 bg_color = user_bg_color if msg['is_user'] else robot_bg_color
                 icon = user_icon if msg['is_user'] else robot_icon
                 empty = self.render_msg(msg['content'],
                                         is_user=msg['is_user'],
                                         icon=icon,
                                         msg_type=msg['msg_type'],
                                         bg_color=bg_color,
+
                                         )
                 if not msg['is_user']:
                     self.last_response = empty
         return self.last_response
 
     def update_last_box_text(self, msg):
         if self.last_response is not None:
```

