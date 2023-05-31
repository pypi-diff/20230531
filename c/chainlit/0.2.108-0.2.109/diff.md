# Comparing `tmp/chainlit-0.2.108.tar.gz` & `tmp/chainlit-0.2.109.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlit-0.2.108.tar", max compression
+gzip compressed data, was "chainlit-0.2.109.tar", max compression
```

## Comparing `chainlit-0.2.108.tar` & `chainlit-0.2.109.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     2477 2023-05-30 16:32:07.078750 chainlit-0.2.108/README.md
--rw-r--r--   0        0        0     6604 2023-05-30 16:31:32.894225 chainlit-0.2.108/chainlit/__init__.py
--rw-r--r--   0        0        0       87 2023-05-30 16:31:32.894225 chainlit-0.2.108/chainlit/__main__.py
--rw-r--r--   0        0        0     1234 2023-05-30 16:31:32.894225 chainlit-0.2.108/chainlit/action.py
--rw-r--r--   0        0        0     3773 2023-05-30 16:31:32.894225 chainlit-0.2.108/chainlit/cli/__init__.py
--rw-r--r--   0        0        0     4093 2023-05-30 16:31:32.894225 chainlit-0.2.108/chainlit/cli/auth.py
--rw-r--r--   0        0        0     2594 2023-05-30 16:31:32.894225 chainlit-0.2.108/chainlit/cli/deploy.py
--rw-r--r--   0        0        0      716 2023-05-30 16:31:32.894225 chainlit-0.2.108/chainlit/cli/utils.py
--rw-r--r--   0        0        0     8463 2023-05-30 16:31:32.894225 chainlit-0.2.108/chainlit/client.py
--rw-r--r--   0        0        0     6273 2023-05-30 16:31:32.894225 chainlit-0.2.108/chainlit/config.py
--rw-r--r--   0        0        0     3836 2023-05-30 16:31:32.894225 chainlit-0.2.108/chainlit/element.py
--rw-r--r--   0        0        0     4317 2023-05-30 16:32:33.771134 chainlit-0.2.108/chainlit/frontend/dist/assets/index-bdffdaa0.css
--rw-r--r--   0        0        0  2074093 2023-05-30 16:32:33.771134 chainlit-0.2.108/chainlit/frontend/dist/assets/index-cda2b07f.js
--rw-r--r--   0        0        0     8889 2023-05-30 16:32:33.763134 chainlit-0.2.108/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg
--rw-r--r--   0        0        0     8891 2023-05-30 16:32:33.771134 chainlit-0.2.108/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg
--rw-r--r--   0        0        0     6455 2023-05-30 16:32:32.487115 chainlit-0.2.108/chainlit/frontend/dist/favicon.svg
--rw-r--r--   0        0        0      772 2023-05-30 16:32:33.771134 chainlit-0.2.108/chainlit/frontend/dist/index.html
--rw-r--r--   0        0        0      399 2023-05-30 16:31:32.898225 chainlit-0.2.108/chainlit/hello.py
--rw-r--r--   0        0        0        0 2023-05-30 16:31:32.898225 chainlit-0.2.108/chainlit/lc/__init__.py
--rw-r--r--   0        0        0     8467 2023-05-30 16:31:32.898225 chainlit-0.2.108/chainlit/lc/chainlit_handler.py
--rw-r--r--   0        0        0      863 2023-05-30 16:31:32.898225 chainlit-0.2.108/chainlit/lc/monkey.py
--rw-r--r--   0        0        0     5388 2023-05-30 16:31:32.898225 chainlit-0.2.108/chainlit/lc/new_monkey.py
--rw-r--r--   0        0        0     4129 2023-05-30 16:31:32.898225 chainlit-0.2.108/chainlit/lc/old_monkey.py
--rw-r--r--   0        0        0     1068 2023-05-30 16:31:32.898225 chainlit-0.2.108/chainlit/lc/utils.py
--rw-r--r--   0        0        0      398 2023-05-30 16:31:32.898225 chainlit-0.2.108/chainlit/logger.py
--rw-r--r--   0        0        0     1618 2023-05-30 16:31:32.898225 chainlit-0.2.108/chainlit/markdown.py
--rw-r--r--   0        0        0    11878 2023-05-30 16:31:32.898225 chainlit-0.2.108/chainlit/message.py
--rw-r--r--   0        0        0     5227 2023-05-30 16:31:32.898225 chainlit-0.2.108/chainlit/sdk.py
--rw-r--r--   0        0        0     9980 2023-05-30 16:31:32.898225 chainlit-0.2.108/chainlit/server.py
--rw-r--r--   0        0        0      800 2023-05-30 16:31:32.898225 chainlit-0.2.108/chainlit/session.py
--rw-r--r--   0        0        0     2342 2023-05-30 16:31:32.898225 chainlit-0.2.108/chainlit/telemetry.py
--rw-r--r--   0        0        0     1015 2023-05-30 16:31:32.898225 chainlit-0.2.108/chainlit/types.py
--rw-r--r--   0        0        0     1145 2023-05-30 16:31:32.898225 chainlit-0.2.108/chainlit/user_session.py
--rw-r--r--   0        0        0      196 2023-05-30 16:31:32.898225 chainlit-0.2.108/chainlit/version.py
--rw-r--r--   0        0        0     1551 2023-05-30 16:31:32.898225 chainlit-0.2.108/chainlit/watch.py
--rw-r--r--   0        0        0     1031 2023-05-30 16:31:32.898225 chainlit-0.2.108/pyproject.toml
--rw-r--r--   0        0        0     3906 1970-01-01 00:00:00.000000 chainlit-0.2.108/PKG-INFO
+-rw-r--r--   0        0        0     2477 2023-05-31 10:15:12.656813 chainlit-0.2.109/README.md
+-rw-r--r--   0        0        0     6604 2023-05-31 10:14:32.228700 chainlit-0.2.109/chainlit/__init__.py
+-rw-r--r--   0        0        0       87 2023-05-31 10:14:32.228700 chainlit-0.2.109/chainlit/__main__.py
+-rw-r--r--   0        0        0     1234 2023-05-31 10:14:32.228700 chainlit-0.2.109/chainlit/action.py
+-rw-r--r--   0        0        0     3773 2023-05-31 10:14:32.228700 chainlit-0.2.109/chainlit/cli/__init__.py
+-rw-r--r--   0        0        0     4093 2023-05-31 10:14:32.228700 chainlit-0.2.109/chainlit/cli/auth.py
+-rw-r--r--   0        0        0     2594 2023-05-31 10:14:32.228700 chainlit-0.2.109/chainlit/cli/deploy.py
+-rw-r--r--   0        0        0      716 2023-05-31 10:14:32.228700 chainlit-0.2.109/chainlit/cli/utils.py
+-rw-r--r--   0        0        0     8463 2023-05-31 10:14:32.228700 chainlit-0.2.109/chainlit/client.py
+-rw-r--r--   0        0        0     6548 2023-05-31 10:14:32.228700 chainlit-0.2.109/chainlit/config.py
+-rw-r--r--   0        0        0     3836 2023-05-31 10:14:32.228700 chainlit-0.2.109/chainlit/element.py
+-rw-r--r--   0        0        0     4317 2023-05-31 10:15:41.320929 chainlit-0.2.109/chainlit/frontend/dist/assets/index-bdffdaa0.css
+-rw-r--r--   0        0        0  2074067 2023-05-31 10:15:41.324929 chainlit-0.2.109/chainlit/frontend/dist/assets/index-eb8166a7.js
+-rw-r--r--   0        0        0     8889 2023-05-31 10:15:41.316929 chainlit-0.2.109/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg
+-rw-r--r--   0        0        0     8891 2023-05-31 10:15:41.320929 chainlit-0.2.109/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg
+-rw-r--r--   0        0        0     6455 2023-05-31 10:15:39.936921 chainlit-0.2.109/chainlit/frontend/dist/favicon.svg
+-rw-r--r--   0        0        0      791 2023-05-31 10:15:41.320929 chainlit-0.2.109/chainlit/frontend/dist/index.html
+-rw-r--r--   0        0        0      399 2023-05-31 10:14:32.232699 chainlit-0.2.109/chainlit/hello.py
+-rw-r--r--   0        0        0        0 2023-05-31 10:14:32.232699 chainlit-0.2.109/chainlit/lc/__init__.py
+-rw-r--r--   0        0        0     8467 2023-05-31 10:14:32.232699 chainlit-0.2.109/chainlit/lc/chainlit_handler.py
+-rw-r--r--   0        0        0      863 2023-05-31 10:14:32.232699 chainlit-0.2.109/chainlit/lc/monkey.py
+-rw-r--r--   0        0        0     5388 2023-05-31 10:14:32.232699 chainlit-0.2.109/chainlit/lc/new_monkey.py
+-rw-r--r--   0        0        0     4129 2023-05-31 10:14:32.232699 chainlit-0.2.109/chainlit/lc/old_monkey.py
+-rw-r--r--   0        0        0     1068 2023-05-31 10:14:32.232699 chainlit-0.2.109/chainlit/lc/utils.py
+-rw-r--r--   0        0        0      398 2023-05-31 10:14:32.232699 chainlit-0.2.109/chainlit/logger.py
+-rw-r--r--   0        0        0     1623 2023-05-31 10:14:32.232699 chainlit-0.2.109/chainlit/markdown.py
+-rw-r--r--   0        0        0    11904 2023-05-31 10:14:32.232699 chainlit-0.2.109/chainlit/message.py
+-rw-r--r--   0        0        0     5227 2023-05-31 10:14:32.232699 chainlit-0.2.109/chainlit/sdk.py
+-rw-r--r--   0        0        0    11101 2023-05-31 10:14:32.232699 chainlit-0.2.109/chainlit/server.py
+-rw-r--r--   0        0        0      800 2023-05-31 10:14:32.232699 chainlit-0.2.109/chainlit/session.py
+-rw-r--r--   0        0        0     2342 2023-05-31 10:14:32.232699 chainlit-0.2.109/chainlit/telemetry.py
+-rw-r--r--   0        0        0     1015 2023-05-31 10:14:32.232699 chainlit-0.2.109/chainlit/types.py
+-rw-r--r--   0        0        0     1145 2023-05-31 10:14:32.232699 chainlit-0.2.109/chainlit/user_session.py
+-rw-r--r--   0        0        0      196 2023-05-31 10:14:32.232699 chainlit-0.2.109/chainlit/version.py
+-rw-r--r--   0        0        0     1551 2023-05-31 10:14:32.232699 chainlit-0.2.109/chainlit/watch.py
+-rw-r--r--   0        0        0     1031 2023-05-31 10:14:32.232699 chainlit-0.2.109/pyproject.toml
+-rw-r--r--   0        0        0     3906 1970-01-01 00:00:00.000000 chainlit-0.2.109/PKG-INFO
```

### Comparing `chainlit-0.2.108/README.md` & `chainlit-0.2.109/README.md`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/__init__.py` & `chainlit-0.2.109/chainlit/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/action.py` & `chainlit-0.2.109/chainlit/action.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/cli/__init__.py` & `chainlit-0.2.109/chainlit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/cli/auth.py` & `chainlit-0.2.109/chainlit/cli/auth.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/cli/deploy.py` & `chainlit-0.2.109/chainlit/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/cli/utils.py` & `chainlit-0.2.109/chainlit/cli/utils.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/client.py` & `chainlit-0.2.109/chainlit/client.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/config.py` & `chainlit-0.2.109/chainlit/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 config_dir = os.path.join(root, ".chainlit")
 config_file = os.path.join(config_dir, "config.toml")
 
 # Default config file created if none exists
 DEFAULT_CONFIG_STR = """[project]
 # Name of the app and chatbot.
 name = "Chatbot"
+# Description of the app and chatbot. This is used for HTML tags.
+# description = ""
 
 # If true (default), the app will be available to anonymous users (once deployed).
 # If false, users will need to authenticate and be part of the project to use the app.
 public = true
 
 # The project ID (found on https://cloud.chainlit.io).
 # If provided, all the message data will be stored in the cloud.
@@ -53,14 +55,16 @@
 
 @dataclass()
 class ChainlitConfig:
     # Chainlit server URL. Used only for cloud features
     chainlit_server: str
     # Name of the app and chatbot. Used as the default message author.
     chatbot_name: str
+    # Description of the app and chatbot. This is used for HTML tags.
+    description: str
     # Whether the app is available to anonymous users or only to team members.
     public: bool
     # Whether to enable telemetry. No personal data is collected.
     enable_telemetry: bool
     # List of environment variables to be provided by each user to use the app. If empty, no environment variables will be asked to the user.
     user_env: List[str]
     # Hide the chain of thought details from the user in the UI.
@@ -151,14 +155,15 @@
 
         # If the developer did not explicitly opt out of telemetry, enable it
         enable_telemetry = project_settings.get("enable_telemetry")
         if enable_telemetry is None:
             enable_telemetry = True
 
         chatbot_name = project_settings.get("name")
+        description = project_settings.get("description", "")
         project_id = project_settings.get("id")
         public = project_settings.get("public")
         user_env = project_settings.get("user_env")
         hide_cot = project_settings.get("hide_cot", False)
         github = project_settings.get("github")
         request_limit = project_settings.get("request_limit", "")
 
@@ -171,14 +176,15 @@
         config = ChainlitConfig(
             action_callbacks={},
             github=github,
             request_limit=request_limit,
             hide_cot=hide_cot,
             chainlit_server=chainlit_server,
             chatbot_name=chatbot_name,
+            description=description,
             public=public,
             enable_telemetry=enable_telemetry,
             user_env=user_env,
             lc_cache_path=lc_cache_path,
             project_id=project_id,
         )
```

### Comparing `chainlit-0.2.108/chainlit/element.py` & `chainlit-0.2.109/chainlit/element.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/frontend/dist/assets/index-bdffdaa0.css` & `chainlit-0.2.109/chainlit/frontend/dist/assets/index-bdffdaa0.css`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/frontend/dist/assets/index-cda2b07f.js` & `chainlit-0.2.109/chainlit/frontend/dist/assets/index-eb8166a7.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -91266,15 +91266,15 @@
                 logout: l
             } = Ov(),
             u = HNe(e);
         return k.useEffect(() => {
             document.body.style.backgroundColor = u.palette.background.default
         }, [u]), k.useEffect(() => {
             t === void 0 && UNe().then(d => {
-                document.title = d.appTitle, n(d)
+                n(d)
             })
         }, []), k.useEffect(() => {
             o && r === void 0 && s({
                 authorizationParams: {
                     audience: "chainlit-cloud"
                 }
             }).then(d => i(d)).catch(d => {
```

### Comparing `chainlit-0.2.108/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg` & `chainlit-0.2.109/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg` & `chainlit-0.2.109/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/frontend/dist/favicon.svg` & `chainlit-0.2.109/chainlit/frontend/dist/favicon.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/lc/chainlit_handler.py` & `chainlit-0.2.109/chainlit/lc/chainlit_handler.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/lc/monkey.py` & `chainlit-0.2.109/chainlit/lc/monkey.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/lc/new_monkey.py` & `chainlit-0.2.109/chainlit/lc/new_monkey.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/lc/old_monkey.py` & `chainlit-0.2.109/chainlit/lc/old_monkey.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/lc/utils.py` & `chainlit-0.2.109/chainlit/lc/utils.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/markdown.py` & `chainlit-0.2.109/chainlit/markdown.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,12 +29,12 @@
             logger.info(f"Created default chainlit markdown file at {chainlit_md_file}")
 
 
 def get_markdown_str(root: str):
     """Get the chainlit.md file as a string."""
     chainlit_md_path = os.path.join(root, "chainlit.md")
     if os.path.exists(chainlit_md_path):
-        with open(chainlit_md_path, encoding="utf-8") as f:
+        with open(chainlit_md_path, "r", encoding="utf-8") as f:
             chainlit_md = f.read()
             return chainlit_md
     else:
         return None
```

### Comparing `chainlit-0.2.108/chainlit/message.py` & `chainlit-0.2.109/chainlit/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
     Ask the user to upload a file before continuing.
     If the user does not answer in time (see timeout), a TimeoutError will be raised or None will be returned depending on raise_on_timeout.
     If a project ID is configured, the file will be uploaded to the cloud storage.
 
     Args:
         content (str): Text displayed above the upload button.
         accept (List[str]): List of mime type to accept like ["text/csv", "application/pdf"]
-        max_size_mb (int, optional): Maximum file size in MB.
+        max_size_mb (int, optional): Maximum file size in MB. Maximum value is 100.
         author (str, optional): The author of the message, this will be used in the UI. Defaults to the chatbot name (see config).
         timeout (int, optional): The number of seconds to wait for an answer before raising a TimeoutError.
         raise_on_timeout (bool, optional): Whether to raise a socketio TimeoutError if the user does not answer in time.
     """
 
     def __init__(
         self,
@@ -361,15 +361,15 @@
     def to_dict(self):
         return {
             "content": self.content,
             "author": self.author,
             "waitForAnswer": True,
         }
 
-    def send(self) -> Union[AskResponse, None]:
+    def send(self) -> Union[AskFileResponse, None]:
         """
         Sends the message to request a file from the user to the UI and waits for the reply.
         """
         trace_event("send_ask_file")
 
         sdk = get_sdk()
```

### Comparing `chainlit-0.2.108/chainlit/sdk.py` & `chainlit-0.2.109/chainlit/sdk.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/server.py` & `chainlit-0.2.109/chainlit/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,25 +21,58 @@
 from chainlit.logger import logger
 
 root_dir = os.path.dirname(os.path.abspath(__file__))
 build_dir = os.path.join(root_dir, "frontend/dist")
 
 app = Flask(__name__, static_folder=build_dir)
 CORS(app)
-socketio = SocketIO(app, cors_allowed_origins="*", async_mode="gevent")
+socketio = SocketIO(
+    app,
+    cors_allowed_origins="*",
+    async_mode="gevent",
+    max_http_buffer_size=1000000 * 100,
+)
+
+
+def inject_html_tags():
+    PLACEHOLDER = "<!-- TAG INJECTION PLACEHOLDER -->"
+
+    default_url = "https://github.com/Chainlit/chainlit"
+    url = config.github or default_url
+
+    tags = f"""<title>{config.chatbot_name}</title>
+    <meta name="description" content="{config.description}">
+    <meta property="og:type" content="website">
+    <meta property="og:title" content="{config.chatbot_name}">
+    <meta property="og:description" content="{config.description}">
+    <meta property="og:image" content="https://chainlit-cloud.s3.eu-west-3.amazonaws.com/logo/chainlit_banner.png">
+    <meta property="og:url" content="{url}">"""
+
+    orig_index_html_file_path = os.path.join(app.static_folder, "index.html")
+    injected_index_html_file_path = os.path.join(app.static_folder, "_index.html")
+
+    with open(orig_index_html_file_path, "r", encoding="utf-8") as f:
+        content = f.read()
+    content = content.replace(PLACEHOLDER, tags)
+
+    with open(injected_index_html_file_path, "w", encoding="utf-8") as f:
+        f.write(content)
+
+
+inject_html_tags()
 
 
 @app.route("/", defaults={"path": ""})
 @app.route("/<path:path>")
 def serve(path):
     """Serve the UI."""
     if path != "" and os.path.exists(app.static_folder + "/" + path):
         return send_from_directory(app.static_folder, path)
     else:
-        return send_from_directory(app.static_folder, "index.html")
+        return send_from_directory(app.static_folder, "_index.html")
 
 
 @app.route("/completion", methods=["POST"])
 @trace
 def completion():
     """Handle a completion request from the prompt playground."""
```

### Comparing `chainlit-0.2.108/chainlit/session.py` & `chainlit-0.2.109/chainlit/session.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/telemetry.py` & `chainlit-0.2.109/chainlit/telemetry.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/types.py` & `chainlit-0.2.109/chainlit/types.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/user_session.py` & `chainlit-0.2.109/chainlit/user_session.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/chainlit/watch.py` & `chainlit-0.2.109/chainlit/watch.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.108/pyproject.toml` & `chainlit-0.2.109/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainlit"
-version = "0.2.108"
+version = "0.2.109"
 keywords = ['LLM', 'Agents', 'gen ai', 'chat ui', 'chatbot ui', 'langchain']
 description = "A faster way to build chatbot UIs."
 authors = ["Chainlit"]
 license = "Apache-2.0 license"
 repository = "https://github.com/Chainlit/chainlit"
 readme = "README.md"
 exclude = [
```

### Comparing `chainlit-0.2.108/PKG-INFO` & `chainlit-0.2.109/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlit
-Version: 0.2.108
+Version: 0.2.109
 Summary: A faster way to build chatbot UIs.
 Home-page: https://github.com/Chainlit/chainlit
 License: Apache-2.0 license
 Keywords: LLM,Agents,gen ai,chat ui,chatbot ui,langchain
 Author: Chainlit
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

