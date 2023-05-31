# Comparing `tmp/edudraw-1.3.tar.gz` & `tmp/edudraw-1.3.2.tar.gz`

## Comparing `edudraw-1.3.tar` & `edudraw-1.3.2.tar`

### file list

```diff
@@ -1,7 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edudraw-1.3/src/EduDraw/__init__.py
--rw-r--r--   0        0        0    37505 2020-02-02 00:00:00.000000 edudraw-1.3/src/EduDraw/edudraw.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 edudraw-1.3/src/EduDraw/requirements.txt
--rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 edudraw-1.3/LICENSE.txt
--rw-r--r--   0        0        0    30589 2020-02-02 00:00:00.000000 edudraw-1.3/README.md
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 edudraw-1.3/pyproject.toml
--rw-r--r--   0        0        0    31201 2020-02-02 00:00:00.000000 edudraw-1.3/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 edudraw-1.3.2/.idea/.gitignore
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 edudraw-1.3.2/.idea/.name
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 edudraw-1.3.2/.idea/Edu-Draw-Python.iml
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 edudraw-1.3.2/.idea/misc.xml
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 edudraw-1.3.2/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 edudraw-1.3.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 edudraw-1.3.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 edudraw-1.3.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edudraw-1.3.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edudraw-1.3.2/src/EduDraw/__init__.py
+-rw-r--r--   0        0        0    38253 2020-02-02 00:00:00.000000 edudraw-1.3.2/src/EduDraw/edudraw.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 edudraw-1.3.2/src/EduDraw/requirements.txt
+-rw-r--r--   0        0        0    14696 2020-02-02 00:00:00.000000 edudraw-1.3.2/tests/edudraw_tests.py
+-rw-r--r--   0        0        0    27030 2020-02-02 00:00:00.000000 edudraw-1.3.2/LICENSE
+-rw-r--r--   0        0        0    32176 2020-02-02 00:00:00.000000 edudraw-1.3.2/README.md
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 edudraw-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0    31647 2020-02-02 00:00:00.000000 edudraw-1.3.2/PKG-INFO
```

### Comparing `edudraw-1.3/src/EduDraw/edudraw.py` & `edudraw-1.3.2/src/EduDraw/edudraw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import gc
 import time
 import copy
 import math
 
 import pygame
 from pygame import gfxdraw
 from threading import Thread
@@ -51,15 +50,14 @@
                 self.func()
 
             if self.interval > 0.005:
                 time.sleep(self.interval)
 
     def quit(self):
         self.flag = True
-        gc.collect()
 
 
 class _SimulationData:
     """
     Helper class to hold simulation data
     """
     def __init__(self):
@@ -167,15 +165,14 @@
         """
         Resets all variables to their default state
         """
 
         self.data = _SimulationData()
         self.data_stack = []
         self.data.custom_font_object = self.original_font_instance
-        gc.collect()
 
     def _proto_setup(self):
         self.setup()
 
     def timer_tick(self):
         """
         Function called every tick of the timer. Serves as the backbone of the draw() function
@@ -187,16 +184,14 @@
         self.frame_count += 1
 
         self.draw()
 
         if not self.null_mode:
             pygame.display.update()
 
-        gc.collect()
-
         if self.reset_after_loop:
             self._reset_variables()
 
     def _proto_draw(self):
         """
         Sets up environment for drawing
         """
@@ -495,15 +490,14 @@
 
     def pop(self):
         """
         Leaves temporary state
         """
         if len(self.data_stack) != 0:
             self.data_stack.pop()
-        gc.collect()
 
     def mouse_pos(self) -> tuple:
         """
         Retrieves the current mouse position relative to the top-left corner of the window
 
         :return: A (x, y) tuple with the positions
         """
@@ -707,14 +701,25 @@
         font_object.set_italic(italic)
         font_object.set_underline(underline)
 
         data = self._get_data_object()
         data.custom_font_object = font_object
 
     def change_default_font(self, new_font: str, font_size: int = 12, bold=False, italic=False, underline=False):
+        """
+        Changes the default font to be used when writing text. If you want to change the font only once
+        in your drawing, it's recommended that you use this method in setup() instead of using font() in
+        draw(), this is way better for performance.
+
+        :param new_font: The name of the new font to be used
+        :param font_size: The size of the font to be used
+        :param bold: Whether the font should be bold or not
+        :param italic: Whether the font should be italic or not
+        :param underline: Whether the font should have an underline or not
+        """
         font_path = pygame.font.match_font(new_font)
         font_object = pygame.font.Font(font_path, font_size)
 
         font_object.set_bold(bold)
         font_object.set_italic(italic)
         font_object.set_underline(underline)
 
@@ -736,15 +741,14 @@
 
     def reset_font(self):
         """
         Resets the font used to the default font
         """
         data = self._get_data_object()
         data.custom_font_object = None
-        data.custom_font = False
 
     def background(self, color: tuple):
         """
         Draws a background over current image. NOTE: Should be called before other drawings so they don't get
         erased by the background.
 
         :param color: The color to draw the background (a (R, G, B) tuple)
@@ -780,26 +784,26 @@
         :param y: The y coordinate to draw the ellipse
         :param width: The width of the x-axis of the ellipse
         :param height: The height of the y-axis of the ellipse
         """
 
         data = self._get_data_object()
 
-        width, height = self._apply_transformations_length(width, height)
-        width, height = int(width), int(height)
-
         if data.cumulative_rotation_angle == 0:
             has_rotation = False
         else:
             has_rotation = True
 
         pos_x, pos_y = self._get_circle_box(x, y, width, height, has_rotation)
         pos_x, pos_y = self._apply_transformations_coords(pos_x, pos_y)
         pos_x, pos_y = int(pos_x), int(pos_y)
 
+        width, height = self._apply_transformations_length(width, height)
+        width, height = int(width), int(height)
+
         stroke_color, fill_color, stroke_weight = self._get_stroke_fill_and_weight()
 
         if not has_rotation or width == height:
             if data.fill_state:
                 if data.anti_aliasing:
                     gfxdraw.filled_ellipse(self.screen, pos_x + width // 2, pos_y + height // 2, width // 2,
                                            height // 2, fill_color)
@@ -957,48 +961,53 @@
 
         if data.stroke_state:
             if data.anti_aliasing:
                 gfxdraw.aapolygon(self.screen, points, stroke_color)
             else:
                 pygame.draw.polygon(self.screen, stroke_color, points, stroke_weight)
 
-        # self.current_graphics.polygon(points, fill_color, stroke_color, stroke_weight)
-
-    def image(self, img: pygame.surface.Surface, x: int, y: int, width: int = None, height: int = None):
+    def image(self, img: pygame.surface.Surface, x: int, y: int, width: int = None, height: int = None,
+              force_transparency: bool = False):
         """
         Displays an image onto the screen on the (x,y) position.
         If specified a width or height, the image will be resized to those sizes, otherwise, the image will be drawn
         to it's original size.
 
         :param img: The Image to be displayed
         :param x: The x coordinate of the top-left corner of the image
         :param y: The y coordinate of the top-left corner of the image
         :param width: (Optional) The width to resize the image
         :param height: (Optional) The height to resize the image
+        :param force_transparency: (Optional) Whether or not to force transparency on non-rgba images.
         """
 
         size = img.get_size()
 
+        if force_transparency:
+            intermediary_surface = pygame.surface.Surface(size, flags=pygame.SRCALPHA)
+            intermediary_surface.blit(img, (0, 0))
+            img = intermediary_surface
+
         data = self._get_data_object()
 
         if width is None:
             width = size[0]
 
         if height is None:
             height = size[1]
 
         target_width, target_height = self._apply_transformations_length(width, height)
 
         if target_width == 0 or target_height == 0:
             return
 
-        if width < 0 or height < 0:
+        if target_width < 0 or target_height < 0:
             raise ValueError
 
-        img = pygame.transform.scale(img, (width, height))
+        img = pygame.transform.scale(img, (target_width, target_height))
         img = pygame.transform.rotate(img, -data.cumulative_rotation_angle)
 
         has_rotation = data.cumulative_rotation_angle != 0
 
         if not has_rotation:
             invert = False
         else:
@@ -1010,16 +1019,14 @@
         real_w, real_h = img.get_size()
 
         if not has_rotation:
             box = (int(x), int(y), real_w, real_h)
         else:
             box = (int(x - real_w//2), int(y - real_h//2), real_w, real_h)
 
-        # size = img.get_size()
-
         self.screen.blit(img, box)
 
     def frame_rate(self, fps: int):
         """
         Sets the desired frame rate. Note that EduDraw using python is slower than it's C# counterpart.
         :param fps: The desired FPS rate.
         """
```

### Comparing `edudraw-1.3/LICENSE.txt` & `edudraw-1.3.2/LICENSE`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,504 +1,504 @@
-                  GNU LESSER GENERAL PUBLIC LICENSE
-                       Version 2.1, February 1999
-
- Copyright (C) 1991, 1999 Free Software Foundation, Inc.
- 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-[This is the first released version of the Lesser GPL.  It also counts
- as the successor of the GNU Library Public License, version 2, hence
- the version number 2.1.]
-
-                            Preamble
-
-  The licenses for most software are designed to take away your
-freedom to share and change it.  By contrast, the GNU General Public
-Licenses are intended to guarantee your freedom to share and change
-free software--to make sure the software is free for all its users.
-
-  This license, the Lesser General Public License, applies to some
-specially designated software packages--typically libraries--of the
-Free Software Foundation and other authors who decide to use it.  You
-can use it too, but we suggest you first think carefully about whether
-this license or the ordinary General Public License is the better
-strategy to use in any particular case, based on the explanations below.
-
-  When we speak of free software, we are referring to freedom of use,
-not price.  Our General Public Licenses are designed to make sure that
-you have the freedom to distribute copies of free software (and charge
-for this service if you wish); that you receive source code or can get
-it if you want it; that you can change the software and use pieces of
-it in new free programs; and that you are informed that you can do
-these things.
-
-  To protect your rights, we need to make restrictions that forbid
-distributors to deny you these rights or to ask you to surrender these
-rights.  These restrictions translate to certain responsibilities for
-you if you distribute copies of the library or if you modify it.
-
-  For example, if you distribute copies of the library, whether gratis
-or for a fee, you must give the recipients all the rights that we gave
-you.  You must make sure that they, too, receive or can get the source
-code.  If you link other code with the library, you must provide
-complete object files to the recipients, so that they can relink them
-with the library after making changes to the library and recompiling
-it.  And you must show them these terms so they know their rights.
-
-  We protect your rights with a two-step method: (1) we copyright the
-library, and (2) we offer you this license, which gives you legal
-permission to copy, distribute and/or modify the library.
-
-  To protect each distributor, we want to make it very clear that
-there is no warranty for the free library.  Also, if the library is
-modified by someone else and passed on, the recipients should know
-that what they have is not the original version, so that the original
-author's reputation will not be affected by problems that might be
-introduced by others.
-
-  Finally, software patents pose a constant threat to the existence of
-any free program.  We wish to make sure that a company cannot
-effectively restrict the users of a free program by obtaining a
-restrictive license from a patent holder.  Therefore, we insist that
-any patent license obtained for a version of the library must be
-consistent with the full freedom of use specified in this license.
-
-  Most GNU software, including some libraries, is covered by the
-ordinary GNU General Public License.  This license, the GNU Lesser
-General Public License, applies to certain designated libraries, and
-is quite different from the ordinary General Public License.  We use
-this license for certain libraries in order to permit linking those
-libraries into non-free programs.
-
-  When a program is linked with a library, whether statically or using
-a shared library, the combination of the two is legally speaking a
-combined work, a derivative of the original library.  The ordinary
-General Public License therefore permits such linking only if the
-entire combination fits its criteria of freedom.  The Lesser General
-Public License permits more lax criteria for linking other code with
-the library.
-
-  We call this license the "Lesser" General Public License because it
-does Less to protect the user's freedom than the ordinary General
-Public License.  It also provides other free software developers Less
-of an advantage over competing non-free programs.  These disadvantages
-are the reason we use the ordinary General Public License for many
-libraries.  However, the Lesser license provides advantages in certain
-special circumstances.
-
-  For example, on rare occasions, there may be a special need to
-encourage the widest possible use of a certain library, so that it becomes
-a de-facto standard.  To achieve this, non-free programs must be
-allowed to use the library.  A more frequent case is that a free
-library does the same job as widely used non-free libraries.  In this
-case, there is little to gain by limiting the free library to free
-software only, so we use the Lesser General Public License.
-
-  In other cases, permission to use a particular library in non-free
-programs enables a greater number of people to use a large body of
-free software.  For example, permission to use the GNU C Library in
-non-free programs enables many more people to use the whole GNU
-operating system, as well as its variant, the GNU/Linux operating
-system.
-
-  Although the Lesser General Public License is Less protective of the
-users' freedom, it does ensure that the user of a program that is
-linked with the Library has the freedom and the wherewithal to run
-that program using a modified version of the Library.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.  Pay close attention to the difference between a
-"work based on the library" and a "work that uses the library".  The
-former contains code derived from the library, whereas the latter must
-be combined with the library in order to run.
-
-                  GNU LESSER GENERAL PUBLIC LICENSE
-   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
-
-  0. This License Agreement applies to any software library or other
-program which contains a notice placed by the copyright holder or
-other authorized party saying it may be distributed under the terms of
-this Lesser General Public License (also called "this License").
-Each licensee is addressed as "you".
-
-  A "library" means a collection of software functions and/or data
-prepared so as to be conveniently linked with application programs
-(which use some of those functions and data) to form executables.
-
-  The "Library", below, refers to any such software library or work
-which has been distributed under these terms.  A "work based on the
-Library" means either the Library or any derivative work under
-copyright law: that is to say, a work containing the Library or a
-portion of it, either verbatim or with modifications and/or translated
-straightforwardly into another language.  (Hereinafter, translation is
-included without limitation in the term "modification".)
-
-  "Source code" for a work means the preferred form of the work for
-making modifications to it.  For a library, complete source code means
-all the source code for all modules it contains, plus any associated
-interface definition files, plus the scripts used to control compilation
-and installation of the library.
-
-  Activities other than copying, distribution and modification are not
-covered by this License; they are outside its scope.  The act of
-running a program using the Library is not restricted, and output from
-such a program is covered only if its contents constitute a work based
-on the Library (independent of the use of the Library in a tool for
-writing it).  Whether that is true depends on what the Library does
-and what the program that uses the Library does.
-
-  1. You may copy and distribute verbatim copies of the Library's
-complete source code as you receive it, in any medium, provided that
-you conspicuously and appropriately publish on each copy an
-appropriate copyright notice and disclaimer of warranty; keep intact
-all the notices that refer to this License and to the absence of any
-warranty; and distribute a copy of this License along with the
-Library.
-
-  You may charge a fee for the physical act of transferring a copy,
-and you may at your option offer warranty protection in exchange for a
-fee.
-
-  2. You may modify your copy or copies of the Library or any portion
-of it, thus forming a work based on the Library, and copy and
-distribute such modifications or work under the terms of Section 1
-above, provided that you also meet all of these conditions:
-
-    a) The modified work must itself be a software library.
-
-    b) You must cause the files modified to carry prominent notices
-    stating that you changed the files and the date of any change.
-
-    c) You must cause the whole of the work to be licensed at no
-    charge to all third parties under the terms of this License.
-
-    d) If a facility in the modified Library refers to a function or a
-    table of data to be supplied by an application program that uses
-    the facility, other than as an argument passed when the facility
-    is invoked, then you must make a good faith effort to ensure that,
-    in the event an application does not supply such function or
-    table, the facility still operates, and performs whatever part of
-    its purpose remains meaningful.
-
-    (For example, a function in a library to compute square roots has
-    a purpose that is entirely well-defined independent of the
-    application.  Therefore, Subsection 2d requires that any
-    application-supplied function or table used by this function must
-    be optional: if the application does not supply it, the square
-    root function must still compute square roots.)
-
-These requirements apply to the modified work as a whole.  If
-identifiable sections of that work are not derived from the Library,
-and can be reasonably considered independent and separate works in
-themselves, then this License, and its terms, do not apply to those
-sections when you distribute them as separate works.  But when you
-distribute the same sections as part of a whole which is a work based
-on the Library, the distribution of the whole must be on the terms of
-this License, whose permissions for other licensees extend to the
-entire whole, and thus to each and every part regardless of who wrote
-it.
-
-Thus, it is not the intent of this section to claim rights or contest
-your rights to work written entirely by you; rather, the intent is to
-exercise the right to control the distribution of derivative or
-collective works based on the Library.
-
-In addition, mere aggregation of another work not based on the Library
-with the Library (or with a work based on the Library) on a volume of
-a storage or distribution medium does not bring the other work under
-the scope of this License.
-
-  3. You may opt to apply the terms of the ordinary GNU General Public
-License instead of this License to a given copy of the Library.  To do
-this, you must alter all the notices that refer to this License, so
-that they refer to the ordinary GNU General Public License, version 2,
-instead of to this License.  (If a newer version than version 2 of the
-ordinary GNU General Public License has appeared, then you can specify
-that version instead if you wish.)  Do not make any other change in
-these notices.
-
-  Once this change is made in a given copy, it is irreversible for
-that copy, so the ordinary GNU General Public License applies to all
-subsequent copies and derivative works made from that copy.
-
-  This option is useful when you wish to copy part of the code of
-the Library into a program that is not a library.
-
-  4. You may copy and distribute the Library (or a portion or
-derivative of it, under Section 2) in object code or executable form
-under the terms of Sections 1 and 2 above provided that you accompany
-it with the complete corresponding machine-readable source code, which
-must be distributed under the terms of Sections 1 and 2 above on a
-medium customarily used for software interchange.
-
-  If distribution of object code is made by offering access to copy
-from a designated place, then offering equivalent access to copy the
-source code from the same place satisfies the requirement to
-distribute the source code, even though third parties are not
-compelled to copy the source along with the object code.
-
-  5. A program that contains no derivative of any portion of the
-Library, but is designed to work with the Library by being compiled or
-linked with it, is called a "work that uses the Library".  Such a
-work, in isolation, is not a derivative work of the Library, and
-therefore falls outside the scope of this License.
-
-  However, linking a "work that uses the Library" with the Library
-creates an executable that is a derivative of the Library (because it
-contains portions of the Library), rather than a "work that uses the
-library".  The executable is therefore covered by this License.
-Section 6 states terms for distribution of such executables.
-
-  When a "work that uses the Library" uses material from a header file
-that is part of the Library, the object code for the work may be a
-derivative work of the Library even though the source code is not.
-Whether this is true is especially significant if the work can be
-linked without the Library, or if the work is itself a library.  The
-threshold for this to be true is not precisely defined by law.
-
-  If such an object file uses only numerical parameters, data
-structure layouts and accessors, and small macros and small inline
-functions (ten lines or less in length), then the use of the object
-file is unrestricted, regardless of whether it is legally a derivative
-work.  (Executables containing this object code plus portions of the
-Library will still fall under Section 6.)
-
-  Otherwise, if the work is a derivative of the Library, you may
-distribute the object code for the work under the terms of Section 6.
-Any executables containing that work also fall under Section 6,
-whether or not they are linked directly with the Library itself.
-
-  6. As an exception to the Sections above, you may also combine or
-link a "work that uses the Library" with the Library to produce a
-work containing portions of the Library, and distribute that work
-under terms of your choice, provided that the terms permit
-modification of the work for the customer's own use and reverse
-engineering for debugging such modifications.
-
-  You must give prominent notice with each copy of the work that the
-Library is used in it and that the Library and its use are covered by
-this License.  You must supply a copy of this License.  If the work
-during execution displays copyright notices, you must include the
-copyright notice for the Library among them, as well as a reference
-directing the user to the copy of this License.  Also, you must do one
-of these things:
-
-    a) Accompany the work with the complete corresponding
-    machine-readable source code for the Library including whatever
-    changes were used in the work (which must be distributed under
-    Sections 1 and 2 above); and, if the work is an executable linked
-    with the Library, with the complete machine-readable "work that
-    uses the Library", as object code and/or source code, so that the
-    user can modify the Library and then relink to produce a modified
-    executable containing the modified Library.  (It is understood
-    that the user who changes the contents of definitions files in the
-    Library will not necessarily be able to recompile the application
-    to use the modified definitions.)
-
-    b) Use a suitable shared library mechanism for linking with the
-    Library.  A suitable mechanism is one that (1) uses at run time a
-    copy of the library already present on the user's computer system,
-    rather than copying library functions into the executable, and (2)
-    will operate properly with a modified version of the library, if
-    the user installs one, as long as the modified version is
-    interface-compatible with the version that the work was made with.
-
-    c) Accompany the work with a written offer, valid for at
-    least three years, to give the same user the materials
-    specified in Subsection 6a, above, for a charge no more
-    than the cost of performing this distribution.
-
-    d) If distribution of the work is made by offering access to copy
-    from a designated place, offer equivalent access to copy the above
-    specified materials from the same place.
-
-    e) Verify that the user has already received a copy of these
-    materials or that you have already sent this user a copy.
-
-  For an executable, the required form of the "work that uses the
-Library" must include any data and utility programs needed for
-reproducing the executable from it.  However, as a special exception,
-the materials to be distributed need not include anything that is
-normally distributed (in either source or binary form) with the major
-components (compiler, kernel, and so on) of the operating system on
-which the executable runs, unless that component itself accompanies
-the executable.
-
-  It may happen that this requirement contradicts the license
-restrictions of other proprietary libraries that do not normally
-accompany the operating system.  Such a contradiction means you cannot
-use both them and the Library together in an executable that you
-distribute.
-
-  7. You may place library facilities that are a work based on the
-Library side-by-side in a single library together with other library
-facilities not covered by this License, and distribute such a combined
-library, provided that the separate distribution of the work based on
-the Library and of the other library facilities is otherwise
-permitted, and provided that you do these two things:
-
-    a) Accompany the combined library with a copy of the same work
-    based on the Library, uncombined with any other library
-    facilities.  This must be distributed under the terms of the
-    Sections above.
-
-    b) Give prominent notice with the combined library of the fact
-    that part of it is a work based on the Library, and explaining
-    where to find the accompanying uncombined form of the same work.
-
-  8. You may not copy, modify, sublicense, link with, or distribute
-the Library except as expressly provided under this License.  Any
-attempt otherwise to copy, modify, sublicense, link with, or
-distribute the Library is void, and will automatically terminate your
-rights under this License.  However, parties who have received copies,
-or rights, from you under this License will not have their licenses
-terminated so long as such parties remain in full compliance.
-
-  9. You are not required to accept this License, since you have not
-signed it.  However, nothing else grants you permission to modify or
-distribute the Library or its derivative works.  These actions are
-prohibited by law if you do not accept this License.  Therefore, by
-modifying or distributing the Library (or any work based on the
-Library), you indicate your acceptance of this License to do so, and
-all its terms and conditions for copying, distributing or modifying
-the Library or works based on it.
-
-  10. Each time you redistribute the Library (or any work based on the
-Library), the recipient automatically receives a license from the
-original licensor to copy, distribute, link with or modify the Library
-subject to these terms and conditions.  You may not impose any further
-restrictions on the recipients' exercise of the rights granted herein.
-You are not responsible for enforcing compliance by third parties with
-this License.
-
-  11. If, as a consequence of a court judgment or allegation of patent
-infringement or for any other reason (not limited to patent issues),
-conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot
-distribute so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you
-may not distribute the Library at all.  For example, if a patent
-license would not permit royalty-free redistribution of the Library by
-all those who receive copies directly or indirectly through you, then
-the only way you could satisfy both it and this License would be to
-refrain entirely from distribution of the Library.
-
-If any portion of this section is held invalid or unenforceable under any
-particular circumstance, the balance of the section is intended to apply,
-and the section as a whole is intended to apply in other circumstances.
-
-It is not the purpose of this section to induce you to infringe any
-patents or other property right claims or to contest validity of any
-such claims; this section has the sole purpose of protecting the
-integrity of the free software distribution system which is
-implemented by public license practices.  Many people have made
-generous contributions to the wide range of software distributed
-through that system in reliance on consistent application of that
-system; it is up to the author/donor to decide if he or she is willing
-to distribute software through any other system and a licensee cannot
-impose that choice.
-
-This section is intended to make thoroughly clear what is believed to
-be a consequence of the rest of this License.
-
-  12. If the distribution and/or use of the Library is restricted in
-certain countries either by patents or by copyrighted interfaces, the
-original copyright holder who places the Library under this License may add
-an explicit geographical distribution limitation excluding those countries,
-so that distribution is permitted only in or among countries not thus
-excluded.  In such case, this License incorporates the limitation as if
-written in the body of this License.
-
-  13. The Free Software Foundation may publish revised and/or new
-versions of the Lesser General Public License from time to time.
-Such new versions will be similar in spirit to the present version,
-but may differ in detail to address new problems or concerns.
-
-Each version is given a distinguishing version number.  If the Library
-specifies a version number of this License which applies to it and
-"any later version", you have the option of following the terms and
-conditions either of that version or of any later version published by
-the Free Software Foundation.  If the Library does not specify a
-license version number, you may choose any version ever published by
-the Free Software Foundation.
-
-  14. If you wish to incorporate parts of the Library into other free
-programs whose distribution conditions are incompatible with these,
-write to the author to ask for permission.  For software which is
-copyrighted by the Free Software Foundation, write to the Free
-Software Foundation; we sometimes make exceptions for this.  Our
-decision will be guided by the two goals of preserving the free status
-of all derivatives of our free software and of promoting the sharing
-and reuse of software generally.
-
-                            NO WARRANTY
-
-  15. BECAUSE THE LIBRARY IS LICENSED FREE OF CHARGE, THERE IS NO
-WARRANTY FOR THE LIBRARY, TO THE EXTENT PERMITTED BY APPLICABLE LAW.
-EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR
-OTHER PARTIES PROVIDE THE LIBRARY "AS IS" WITHOUT WARRANTY OF ANY
-KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE
-LIBRARY IS WITH YOU.  SHOULD THE LIBRARY PROVE DEFECTIVE, YOU ASSUME
-THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN
-WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY
-AND/OR REDISTRIBUTE THE LIBRARY AS PERMITTED ABOVE, BE LIABLE TO YOU
-FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR
-CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE
-LIBRARY (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING
-RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A
-FAILURE OF THE LIBRARY TO OPERATE WITH ANY OTHER SOFTWARE), EVEN IF
-SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH
-DAMAGES.
-
-                     END OF TERMS AND CONDITIONS
-
-           How to Apply These Terms to Your New Libraries
-
-  If you develop a new library, and you want it to be of the greatest
-possible use to the public, we recommend making it free software that
-everyone can redistribute and change.  You can do so by permitting
-redistribution under these terms (or, alternatively, under the terms of the
-ordinary General Public License).
-
-  To apply these terms, attach the following notices to the library.  It is
-safest to attach them to the start of each source file to most effectively
-convey the exclusion of warranty; and each file should have at least the
-"copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the library's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This library is free software; you can redistribute it and/or
-    modify it under the terms of the GNU Lesser General Public
-    License as published by the Free Software Foundation; either
-    version 2.1 of the License, or (at your option) any later version.
-
-    This library is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-    Lesser General Public License for more details.
-
-    You should have received a copy of the GNU Lesser General Public
-    License along with this library; if not, write to the Free Software
-    Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301
-    USA
-
-Also add information on how to contact you by electronic and paper mail.
-
-You should also get your employer (if you work as a programmer) or your
-school, if any, to sign a "copyright disclaimer" for the library, if
-necessary.  Here is a sample; alter the names:
-
-  Yoyodyne, Inc., hereby disclaims all copyright interest in the
-  library `Frob' (a library for tweaking knobs) written by James Random
-  Hacker.
-
-  <signature of Ty Coon>, 1 April 1990
-  Ty Coon, President of Vice
-
-That's all there is to it!
+                  GNU LESSER GENERAL PUBLIC LICENSE
+                       Version 2.1, February 1999
+
+ Copyright (C) 1991, 1999 Free Software Foundation, Inc.
+ 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+[This is the first released version of the Lesser GPL.  It also counts
+ as the successor of the GNU Library Public License, version 2, hence
+ the version number 2.1.]
+
+                            Preamble
+
+  The licenses for most software are designed to take away your
+freedom to share and change it.  By contrast, the GNU General Public
+Licenses are intended to guarantee your freedom to share and change
+free software--to make sure the software is free for all its users.
+
+  This license, the Lesser General Public License, applies to some
+specially designated software packages--typically libraries--of the
+Free Software Foundation and other authors who decide to use it.  You
+can use it too, but we suggest you first think carefully about whether
+this license or the ordinary General Public License is the better
+strategy to use in any particular case, based on the explanations below.
+
+  When we speak of free software, we are referring to freedom of use,
+not price.  Our General Public Licenses are designed to make sure that
+you have the freedom to distribute copies of free software (and charge
+for this service if you wish); that you receive source code or can get
+it if you want it; that you can change the software and use pieces of
+it in new free programs; and that you are informed that you can do
+these things.
+
+  To protect your rights, we need to make restrictions that forbid
+distributors to deny you these rights or to ask you to surrender these
+rights.  These restrictions translate to certain responsibilities for
+you if you distribute copies of the library or if you modify it.
+
+  For example, if you distribute copies of the library, whether gratis
+or for a fee, you must give the recipients all the rights that we gave
+you.  You must make sure that they, too, receive or can get the source
+code.  If you link other code with the library, you must provide
+complete object files to the recipients, so that they can relink them
+with the library after making changes to the library and recompiling
+it.  And you must show them these terms so they know their rights.
+
+  We protect your rights with a two-step method: (1) we copyright the
+library, and (2) we offer you this license, which gives you legal
+permission to copy, distribute and/or modify the library.
+
+  To protect each distributor, we want to make it very clear that
+there is no warranty for the free library.  Also, if the library is
+modified by someone else and passed on, the recipients should know
+that what they have is not the original version, so that the original
+author's reputation will not be affected by problems that might be
+introduced by others.
+
+  Finally, software patents pose a constant threat to the existence of
+any free program.  We wish to make sure that a company cannot
+effectively restrict the users of a free program by obtaining a
+restrictive license from a patent holder.  Therefore, we insist that
+any patent license obtained for a version of the library must be
+consistent with the full freedom of use specified in this license.
+
+  Most GNU software, including some libraries, is covered by the
+ordinary GNU General Public License.  This license, the GNU Lesser
+General Public License, applies to certain designated libraries, and
+is quite different from the ordinary General Public License.  We use
+this license for certain libraries in order to permit linking those
+libraries into non-free programs.
+
+  When a program is linked with a library, whether statically or using
+a shared library, the combination of the two is legally speaking a
+combined work, a derivative of the original library.  The ordinary
+General Public License therefore permits such linking only if the
+entire combination fits its criteria of freedom.  The Lesser General
+Public License permits more lax criteria for linking other code with
+the library.
+
+  We call this license the "Lesser" General Public License because it
+does Less to protect the user's freedom than the ordinary General
+Public License.  It also provides other free software developers Less
+of an advantage over competing non-free programs.  These disadvantages
+are the reason we use the ordinary General Public License for many
+libraries.  However, the Lesser license provides advantages in certain
+special circumstances.
+
+  For example, on rare occasions, there may be a special need to
+encourage the widest possible use of a certain library, so that it becomes
+a de-facto standard.  To achieve this, non-free programs must be
+allowed to use the library.  A more frequent case is that a free
+library does the same job as widely used non-free libraries.  In this
+case, there is little to gain by limiting the free library to free
+software only, so we use the Lesser General Public License.
+
+  In other cases, permission to use a particular library in non-free
+programs enables a greater number of people to use a large body of
+free software.  For example, permission to use the GNU C Library in
+non-free programs enables many more people to use the whole GNU
+operating system, as well as its variant, the GNU/Linux operating
+system.
+
+  Although the Lesser General Public License is Less protective of the
+users' freedom, it does ensure that the user of a program that is
+linked with the Library has the freedom and the wherewithal to run
+that program using a modified version of the Library.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.  Pay close attention to the difference between a
+"work based on the library" and a "work that uses the library".  The
+former contains code derived from the library, whereas the latter must
+be combined with the library in order to run.
+
+                  GNU LESSER GENERAL PUBLIC LICENSE
+   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
+
+  0. This License Agreement applies to any software library or other
+program which contains a notice placed by the copyright holder or
+other authorized party saying it may be distributed under the terms of
+this Lesser General Public License (also called "this License").
+Each licensee is addressed as "you".
+
+  A "library" means a collection of software functions and/or data
+prepared so as to be conveniently linked with application programs
+(which use some of those functions and data) to form executables.
+
+  The "Library", below, refers to any such software library or work
+which has been distributed under these terms.  A "work based on the
+Library" means either the Library or any derivative work under
+copyright law: that is to say, a work containing the Library or a
+portion of it, either verbatim or with modifications and/or translated
+straightforwardly into another language.  (Hereinafter, translation is
+included without limitation in the term "modification".)
+
+  "Source code" for a work means the preferred form of the work for
+making modifications to it.  For a library, complete source code means
+all the source code for all modules it contains, plus any associated
+interface definition files, plus the scripts used to control compilation
+and installation of the library.
+
+  Activities other than copying, distribution and modification are not
+covered by this License; they are outside its scope.  The act of
+running a program using the Library is not restricted, and output from
+such a program is covered only if its contents constitute a work based
+on the Library (independent of the use of the Library in a tool for
+writing it).  Whether that is true depends on what the Library does
+and what the program that uses the Library does.
+
+  1. You may copy and distribute verbatim copies of the Library's
+complete source code as you receive it, in any medium, provided that
+you conspicuously and appropriately publish on each copy an
+appropriate copyright notice and disclaimer of warranty; keep intact
+all the notices that refer to this License and to the absence of any
+warranty; and distribute a copy of this License along with the
+Library.
+
+  You may charge a fee for the physical act of transferring a copy,
+and you may at your option offer warranty protection in exchange for a
+fee.
+
+  2. You may modify your copy or copies of the Library or any portion
+of it, thus forming a work based on the Library, and copy and
+distribute such modifications or work under the terms of Section 1
+above, provided that you also meet all of these conditions:
+
+    a) The modified work must itself be a software library.
+
+    b) You must cause the files modified to carry prominent notices
+    stating that you changed the files and the date of any change.
+
+    c) You must cause the whole of the work to be licensed at no
+    charge to all third parties under the terms of this License.
+
+    d) If a facility in the modified Library refers to a function or a
+    table of data to be supplied by an application program that uses
+    the facility, other than as an argument passed when the facility
+    is invoked, then you must make a good faith effort to ensure that,
+    in the event an application does not supply such function or
+    table, the facility still operates, and performs whatever part of
+    its purpose remains meaningful.
+
+    (For example, a function in a library to compute square roots has
+    a purpose that is entirely well-defined independent of the
+    application.  Therefore, Subsection 2d requires that any
+    application-supplied function or table used by this function must
+    be optional: if the application does not supply it, the square
+    root function must still compute square roots.)
+
+These requirements apply to the modified work as a whole.  If
+identifiable sections of that work are not derived from the Library,
+and can be reasonably considered independent and separate works in
+themselves, then this License, and its terms, do not apply to those
+sections when you distribute them as separate works.  But when you
+distribute the same sections as part of a whole which is a work based
+on the Library, the distribution of the whole must be on the terms of
+this License, whose permissions for other licensees extend to the
+entire whole, and thus to each and every part regardless of who wrote
+it.
+
+Thus, it is not the intent of this section to claim rights or contest
+your rights to work written entirely by you; rather, the intent is to
+exercise the right to control the distribution of derivative or
+collective works based on the Library.
+
+In addition, mere aggregation of another work not based on the Library
+with the Library (or with a work based on the Library) on a volume of
+a storage or distribution medium does not bring the other work under
+the scope of this License.
+
+  3. You may opt to apply the terms of the ordinary GNU General Public
+License instead of this License to a given copy of the Library.  To do
+this, you must alter all the notices that refer to this License, so
+that they refer to the ordinary GNU General Public License, version 2,
+instead of to this License.  (If a newer version than version 2 of the
+ordinary GNU General Public License has appeared, then you can specify
+that version instead if you wish.)  Do not make any other change in
+these notices.
+
+  Once this change is made in a given copy, it is irreversible for
+that copy, so the ordinary GNU General Public License applies to all
+subsequent copies and derivative works made from that copy.
+
+  This option is useful when you wish to copy part of the code of
+the Library into a program that is not a library.
+
+  4. You may copy and distribute the Library (or a portion or
+derivative of it, under Section 2) in object code or executable form
+under the terms of Sections 1 and 2 above provided that you accompany
+it with the complete corresponding machine-readable source code, which
+must be distributed under the terms of Sections 1 and 2 above on a
+medium customarily used for software interchange.
+
+  If distribution of object code is made by offering access to copy
+from a designated place, then offering equivalent access to copy the
+source code from the same place satisfies the requirement to
+distribute the source code, even though third parties are not
+compelled to copy the source along with the object code.
+
+  5. A program that contains no derivative of any portion of the
+Library, but is designed to work with the Library by being compiled or
+linked with it, is called a "work that uses the Library".  Such a
+work, in isolation, is not a derivative work of the Library, and
+therefore falls outside the scope of this License.
+
+  However, linking a "work that uses the Library" with the Library
+creates an executable that is a derivative of the Library (because it
+contains portions of the Library), rather than a "work that uses the
+library".  The executable is therefore covered by this License.
+Section 6 states terms for distribution of such executables.
+
+  When a "work that uses the Library" uses material from a header file
+that is part of the Library, the object code for the work may be a
+derivative work of the Library even though the source code is not.
+Whether this is true is especially significant if the work can be
+linked without the Library, or if the work is itself a library.  The
+threshold for this to be true is not precisely defined by law.
+
+  If such an object file uses only numerical parameters, data
+structure layouts and accessors, and small macros and small inline
+functions (ten lines or less in length), then the use of the object
+file is unrestricted, regardless of whether it is legally a derivative
+work.  (Executables containing this object code plus portions of the
+Library will still fall under Section 6.)
+
+  Otherwise, if the work is a derivative of the Library, you may
+distribute the object code for the work under the terms of Section 6.
+Any executables containing that work also fall under Section 6,
+whether or not they are linked directly with the Library itself.
+
+  6. As an exception to the Sections above, you may also combine or
+link a "work that uses the Library" with the Library to produce a
+work containing portions of the Library, and distribute that work
+under terms of your choice, provided that the terms permit
+modification of the work for the customer's own use and reverse
+engineering for debugging such modifications.
+
+  You must give prominent notice with each copy of the work that the
+Library is used in it and that the Library and its use are covered by
+this License.  You must supply a copy of this License.  If the work
+during execution displays copyright notices, you must include the
+copyright notice for the Library among them, as well as a reference
+directing the user to the copy of this License.  Also, you must do one
+of these things:
+
+    a) Accompany the work with the complete corresponding
+    machine-readable source code for the Library including whatever
+    changes were used in the work (which must be distributed under
+    Sections 1 and 2 above); and, if the work is an executable linked
+    with the Library, with the complete machine-readable "work that
+    uses the Library", as object code and/or source code, so that the
+    user can modify the Library and then relink to produce a modified
+    executable containing the modified Library.  (It is understood
+    that the user who changes the contents of definitions files in the
+    Library will not necessarily be able to recompile the application
+    to use the modified definitions.)
+
+    b) Use a suitable shared library mechanism for linking with the
+    Library.  A suitable mechanism is one that (1) uses at run time a
+    copy of the library already present on the user's computer system,
+    rather than copying library functions into the executable, and (2)
+    will operate properly with a modified version of the library, if
+    the user installs one, as long as the modified version is
+    interface-compatible with the version that the work was made with.
+
+    c) Accompany the work with a written offer, valid for at
+    least three years, to give the same user the materials
+    specified in Subsection 6a, above, for a charge no more
+    than the cost of performing this distribution.
+
+    d) If distribution of the work is made by offering access to copy
+    from a designated place, offer equivalent access to copy the above
+    specified materials from the same place.
+
+    e) Verify that the user has already received a copy of these
+    materials or that you have already sent this user a copy.
+
+  For an executable, the required form of the "work that uses the
+Library" must include any data and utility programs needed for
+reproducing the executable from it.  However, as a special exception,
+the materials to be distributed need not include anything that is
+normally distributed (in either source or binary form) with the major
+components (compiler, kernel, and so on) of the operating system on
+which the executable runs, unless that component itself accompanies
+the executable.
+
+  It may happen that this requirement contradicts the license
+restrictions of other proprietary libraries that do not normally
+accompany the operating system.  Such a contradiction means you cannot
+use both them and the Library together in an executable that you
+distribute.
+
+  7. You may place library facilities that are a work based on the
+Library side-by-side in a single library together with other library
+facilities not covered by this License, and distribute such a combined
+library, provided that the separate distribution of the work based on
+the Library and of the other library facilities is otherwise
+permitted, and provided that you do these two things:
+
+    a) Accompany the combined library with a copy of the same work
+    based on the Library, uncombined with any other library
+    facilities.  This must be distributed under the terms of the
+    Sections above.
+
+    b) Give prominent notice with the combined library of the fact
+    that part of it is a work based on the Library, and explaining
+    where to find the accompanying uncombined form of the same work.
+
+  8. You may not copy, modify, sublicense, link with, or distribute
+the Library except as expressly provided under this License.  Any
+attempt otherwise to copy, modify, sublicense, link with, or
+distribute the Library is void, and will automatically terminate your
+rights under this License.  However, parties who have received copies,
+or rights, from you under this License will not have their licenses
+terminated so long as such parties remain in full compliance.
+
+  9. You are not required to accept this License, since you have not
+signed it.  However, nothing else grants you permission to modify or
+distribute the Library or its derivative works.  These actions are
+prohibited by law if you do not accept this License.  Therefore, by
+modifying or distributing the Library (or any work based on the
+Library), you indicate your acceptance of this License to do so, and
+all its terms and conditions for copying, distributing or modifying
+the Library or works based on it.
+
+  10. Each time you redistribute the Library (or any work based on the
+Library), the recipient automatically receives a license from the
+original licensor to copy, distribute, link with or modify the Library
+subject to these terms and conditions.  You may not impose any further
+restrictions on the recipients' exercise of the rights granted herein.
+You are not responsible for enforcing compliance by third parties with
+this License.
+
+  11. If, as a consequence of a court judgment or allegation of patent
+infringement or for any other reason (not limited to patent issues),
+conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot
+distribute so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you
+may not distribute the Library at all.  For example, if a patent
+license would not permit royalty-free redistribution of the Library by
+all those who receive copies directly or indirectly through you, then
+the only way you could satisfy both it and this License would be to
+refrain entirely from distribution of the Library.
+
+If any portion of this section is held invalid or unenforceable under any
+particular circumstance, the balance of the section is intended to apply,
+and the section as a whole is intended to apply in other circumstances.
+
+It is not the purpose of this section to induce you to infringe any
+patents or other property right claims or to contest validity of any
+such claims; this section has the sole purpose of protecting the
+integrity of the free software distribution system which is
+implemented by public license practices.  Many people have made
+generous contributions to the wide range of software distributed
+through that system in reliance on consistent application of that
+system; it is up to the author/donor to decide if he or she is willing
+to distribute software through any other system and a licensee cannot
+impose that choice.
+
+This section is intended to make thoroughly clear what is believed to
+be a consequence of the rest of this License.
+
+  12. If the distribution and/or use of the Library is restricted in
+certain countries either by patents or by copyrighted interfaces, the
+original copyright holder who places the Library under this License may add
+an explicit geographical distribution limitation excluding those countries,
+so that distribution is permitted only in or among countries not thus
+excluded.  In such case, this License incorporates the limitation as if
+written in the body of this License.
+
+  13. The Free Software Foundation may publish revised and/or new
+versions of the Lesser General Public License from time to time.
+Such new versions will be similar in spirit to the present version,
+but may differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number.  If the Library
+specifies a version number of this License which applies to it and
+"any later version", you have the option of following the terms and
+conditions either of that version or of any later version published by
+the Free Software Foundation.  If the Library does not specify a
+license version number, you may choose any version ever published by
+the Free Software Foundation.
+
+  14. If you wish to incorporate parts of the Library into other free
+programs whose distribution conditions are incompatible with these,
+write to the author to ask for permission.  For software which is
+copyrighted by the Free Software Foundation, write to the Free
+Software Foundation; we sometimes make exceptions for this.  Our
+decision will be guided by the two goals of preserving the free status
+of all derivatives of our free software and of promoting the sharing
+and reuse of software generally.
+
+                            NO WARRANTY
+
+  15. BECAUSE THE LIBRARY IS LICENSED FREE OF CHARGE, THERE IS NO
+WARRANTY FOR THE LIBRARY, TO THE EXTENT PERMITTED BY APPLICABLE LAW.
+EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR
+OTHER PARTIES PROVIDE THE LIBRARY "AS IS" WITHOUT WARRANTY OF ANY
+KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE
+LIBRARY IS WITH YOU.  SHOULD THE LIBRARY PROVE DEFECTIVE, YOU ASSUME
+THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN
+WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY
+AND/OR REDISTRIBUTE THE LIBRARY AS PERMITTED ABOVE, BE LIABLE TO YOU
+FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR
+CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE
+LIBRARY (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING
+RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A
+FAILURE OF THE LIBRARY TO OPERATE WITH ANY OTHER SOFTWARE), EVEN IF
+SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH
+DAMAGES.
+
+                     END OF TERMS AND CONDITIONS
+
+           How to Apply These Terms to Your New Libraries
+
+  If you develop a new library, and you want it to be of the greatest
+possible use to the public, we recommend making it free software that
+everyone can redistribute and change.  You can do so by permitting
+redistribution under these terms (or, alternatively, under the terms of the
+ordinary General Public License).
+
+  To apply these terms, attach the following notices to the library.  It is
+safest to attach them to the start of each source file to most effectively
+convey the exclusion of warranty; and each file should have at least the
+"copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the library's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This library is free software; you can redistribute it and/or
+    modify it under the terms of the GNU Lesser General Public
+    License as published by the Free Software Foundation; either
+    version 2.1 of the License, or (at your option) any later version.
+
+    This library is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+    Lesser General Public License for more details.
+
+    You should have received a copy of the GNU Lesser General Public
+    License along with this library; if not, write to the Free Software
+    Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301
+    USA
+
+Also add information on how to contact you by electronic and paper mail.
+
+You should also get your employer (if you work as a programmer) or your
+school, if any, to sign a "copyright disclaimer" for the library, if
+necessary.  Here is a sample; alter the names:
+
+  Yoyodyne, Inc., hereby disclaims all copyright interest in the
+  library `Frob' (a library for tweaking knobs) written by James Random
+  Hacker.
+
+  <signature of Ty Coon>, 1 April 1990
+  Ty Coon, President of Vice
+
+That's all there is to it!
```

### Comparing `edudraw-1.3/README.md` & `edudraw-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,58 @@
+Metadata-Version: 2.1
+Name: EduDraw
+Version: 1.3.2
+Summary: A simple interface for using 2D graphics in python
+Project-URL: Homepage, https://github.com/MuriloLCN/Edu-Draw-Python
+Project-URL: Bug Tracker, https://github.com/MuriloLCN/Edu-Draw-Python/issues
+Author-email: Murilo Luis Calvo Neves <muriloluiscalvoneves2004@hotmail.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # Edu-Draw-Python
 
 This is the Python version of EduDraw, for the C# version, please see [Edu Draw C#](https://github.com/MuriloLCN/Simple-Draw-Csharp)
 
 This project is aimed to provide an interface that allows for a simplified experience when using basic 2D graphics in the Python language. 
 
 The general design of the interface is heavily (if not all) inspired by the [P5.js](https://p5js.org/) library and the Processing library, and is intended to make simple graphical programs easy to do in the .NET environment in the shape of a Windows Forms app and/or in the Python language.
 
 The details of installation and documentation of the respective versions are below. 
 
 ## Installation
 
-In order to use the Python version you can simply download the ```edudraw.py``` and import it in your code like any other library. You'll also need the requirements, which can be installed from the ```requirements.txt``` file.
+You can install the package using PIP by typing the following command: `pip install edudraw`, and import it in your code like any other library.
+You'll need the pygame library as well, in case it doesn't get automatically installed.
 
 ## Setting up
 
 In order to begin using the EduDraw class to make your drawings, you need to do a few steps first:
   
-#### 1. Install the requirements
-
-You need to install the requirements from the requirements file, you can do this by adding the file on your directory and running the following command:
+#### 1. Install the library and the requirements
 
-    pip3 install -r requirements.txt
+The only requirement for this library is `pygame==2.1.2`.
 
-#### 2. Import the implementation file
+#### 2. Import the library
 
 You can do this by adding this to your imports:
 
-    from edudraw import EduDraw
+    from EduDraw import edudraw
 
 Make sure the file is in the same directory as the file from which you are using it from or that you properly add the path otherwise.
 
 #### 3. Create an instance of the EduDraw class
   
 This can be done by simply creating a new EduDraw instance like this:
     
     width, height = 500, 500  # Any size you want
-    s = EduDraw(width, height)
+    s = edudraw.EduDraw(width, height)
     
 #### 4. Create a ```setup()``` and a ```draw()``` function
 
 These functions are the core of your drawing. ```setup()``` runs once and before ```draw()```, and it is used to set up the environment for the drawings that you want to do. Some things (like the frame rate) must be set in here, before the drawing actually begins. 
   
 ```draw()```, on the other hand, runs every frame, and is where you will give life to your graphics. Here is where shapes and elements will get drawn to the screen.
 
@@ -47,36 +60,36 @@
  
 Once you run this method on the instance you made for the EduDraw class, the simulation will start and keep running until you give it a halt command or close the window.
 You need to pass the ```setup()``` and ```draw()``` functions you made, and also a ```window_title``` to give the running window a name.
 
 The general structure of your form code may look something like this:
 
 ```
-from eduraw import EduDraw
+from EduDraw import edudraw
 
 def setup():
     # Setting up goes here...
 
 def draw():
     # Drawing goes here...
 
-s = EduDraw(500, 500)
+s = edudraw.EduDraw(500, 500)
 s.start(setup, draw, "My cool window")
 ```
 
 And now you're ready to get onto some drawings :D
 
 ## Getting started (with a simple example)
 
 Now that you have your canvas ready for the show, it's time to actually draw something on the screen. To begin with,let's draw a circle on the screen with a white background. Our code might look something like this:
 
 ```
-from edudraw import EduDraw
+from EduDraw import edudraw
 
-s = EduDraw(500, 300)
+s = edudraw.EduDraw(500, 300)
 
 def setup():
     pass
 
 def draw():
     s.background((255, 255, 255))
     s.circle_mode('TOP_LEFT')
@@ -90,17 +103,17 @@
 
 ![img1](https://github.com/MuriloLCN/Simple-Draw-Python/assets/88753590/b6ec2e1f-9b75-4c02-88fc-d66ef73c6909)
 
 
 That's our circle! But this is not very interesting, so let's give it a red filling color, a blue outline and make it move around.
 
 ```
-from edudraw import EduDraw
+from EduDraw import edudraw
 
-s = EduDraw(500, 300)
+s = edudraw.EduDraw(500, 300)
 
 
 def setup():
     pass
 
 
 velocity = 5
@@ -123,17 +136,17 @@
 
 ![img2](https://github.com/MuriloLCN/Simple-Draw-Python/assets/88753590/b780f016-ef8f-4f66-8d29-120736602985)
 
 
 Now we have a moving red ball :D, but it leaves the screen fairly quickly, so let's make it bounce around.
 
 ```
-from edudraw import EduDraw
+from EduDraw import edudraw
 
-s = EduDraw(500, 300)
+s = edudraw.EduDraw(500, 300)
 
 width, height = 0, 0
 velocity = [5, 5]
 ball_position = [50, 50]
 
 
 def setup():
@@ -145,18 +158,18 @@
 def draw():
     global ball_position, velocity
     s.background((255, 255, 255))
     s.circle_mode('CENTER')
     s.fill((255, 0, 0))
     s.stroke((0, 0, 255))
 
-    if ball_position[1] < 0 or ball_position[1] + 42 > height:
+    if ball_position[1] < 24 or ball_position[1] + 24 > height:
         velocity[1] *= -1
 
-    if ball_position[0] < 0 or ball_position[0] + 42 > width:
+    if ball_position[0] < 24 or ball_position[0] + 24 > width:
         velocity[0] *= -1
 
     ball_position[0] += velocity[0]
     ball_position[1] += velocity[1]
 
     s.circle(ball_position[0], ball_position[1], 24)
 
@@ -1005,26 +1018,28 @@
 ```
 
 ![polygon](https://user-images.githubusercontent.com/88753590/233815221-2da1f919-571f-40a2-ad96-cb4e4084875b.png)
 
 
 ---
 
-### EduDraw.image(img: pygame.surface.Surface, x: int, y: int, width: int = None, height: int = None):
+### EduDraw.image(img: pygame.surface.Surface, x: int, y: int, width: int = None, height: int = None, force_transparency: bool = False):
     
 Displays an image onto the screen on the (x,y) position. If specified a width or height, the image will be resized to those sizes, otherwise, the image will be drawn to it's original size.
     
 Parameters:
 
 img: The image to be drawn onto the canvas
     
 x, y: The position to draw the image
     
 (Optional) width, height: The sizes to set the image to
 
+(Optional) force_transparency: Whether or not force transparency onto the image. See more details below:
+
 ```
 my_image = pygame.image.load('testimage.jpeg')
 
 def setup():
     pass
 
 def draw():
@@ -1032,14 +1047,20 @@
     s.background((0, 0, 0))
     s.rect_mode("CENTER")
     s.image(my_image, s.width // 2, s.height // 2, s.width // 2, s.height // 2)
 ```
 
 ![img](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/4dba8d75-7061-469d-a5fc-851908eb6d0f)
 
+Note that some images may not have transparency when transformed into `pygame.Surface` objects through the
+`pygame.image.load()` method. Should this be the case, like the one below, you can use the `force_transparency`
+parameter to force that.
+
+![example](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/c350c788-3cc4-491e-94f9-67c1a7aa8a78)
+
 
 ### EduDraw.frame_rate(fps: int)
 
 Changes the framerate of the simulation. Must be called in ```setup()```.
 Note that in the Python version the simulation does not run as fast as the C# one, to run the simulation as fast as possible set the EduDraw.deltatime to zero.
 
 Parameters:
@@ -1062,16 +1083,16 @@
 Null mode is a mode in which you can run an instance of a simulation without having it running directly onto the canvas. You can do this for many reasons, including using EduDraw in a different context or application, creating multiple drawings inside of one another, among other things.
 
 To initialize an EduDraw instance in null mode, you can use the optional parameter for it in the `start()` method.
 
 Example of null mode:
 
 ```
-s = EduDraw(500, 500) # Main instance
-d = EduDraw(250, 250, True) # Null mode ('inner') instance
+s = edudraw.EduDraw(500, 500) # Main instance
+d = edudraw.EduDraw(250, 250, True) # Null mode ('inner') instance
 
 def setup():
   {...}
 
 def draw():
   {...}
 
@@ -1088,16 +1109,16 @@
 In order to be able to visualize instance of null mode, you'll have to retrieve the images (`pygame.surface.Surface`) and use those in your drawing or any other desired output (whether that be an icon, a display, a file, etc.).
 
 You can retrieve the images with the `EduDraw.screen` variable. With that Surface object retrieved, you can use it wherever it's necessary, and you have much more flexibility for what to do with it.
 
 A good example of this is to run two instances of EduDraw, one normal and one null, and use the retrieved images from the null instance as an argument for EduDraw.image(), essentially creating a drawing inside of a drawing, like the example below:
 
 ```
-s = EduDraw(200, 200)
-d = EduDraw(100, 100, True)
+s = edudraw.EduDraw(200, 200)
+d = edudraw.EduDraw(100, 100, True)
 
 position = [d.width/2, d.height//2]
 velocity = [3, 4]
 
 # We don't need to setup anything in this case
 def setup():
     pass
```

### Comparing `edudraw-1.3/pyproject.toml` & `edudraw-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EduDraw"
-version = "1.3"
+version = "1.3.2"
 authors = [
   { name="Murilo Luis Calvo Neves", email="muriloluiscalvoneves2004@hotmail.com" },
 ]
 description = "A simple interface for using 2D graphics in python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `edudraw-1.3/PKG-INFO` & `edudraw-1.3.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,1146 +1,1139 @@
-Metadata-Version: 2.1
-Name: EduDraw
-Version: 1.3
-Summary: A simple interface for using 2D graphics in python
-Project-URL: Homepage, https://github.com/MuriloLCN/Edu-Draw-Python
-Project-URL: Bug Tracker, https://github.com/MuriloLCN/Edu-Draw-Python/issues
-Author-email: Murilo Luis Calvo Neves <muriloluiscalvoneves2004@hotmail.com>
-License-File: LICENSE.txt
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-# Edu-Draw-Python
-
-This is the Python version of EduDraw, for the C# version, please see [Edu Draw C#](https://github.com/MuriloLCN/Simple-Draw-Csharp)
-
-This project is aimed to provide an interface that allows for a simplified experience when using basic 2D graphics in the Python language. 
-
-The general design of the interface is heavily (if not all) inspired by the [P5.js](https://p5js.org/) library and the Processing library, and is intended to make simple graphical programs easy to do in the .NET environment in the shape of a Windows Forms app and/or in the Python language.
-
-The details of installation and documentation of the respective versions are below. 
-
-## Installation
-
-In order to use the Python version you can simply download the ```edudraw.py``` and import it in your code like any other library. You'll also need the requirements, which can be installed from the ```requirements.txt``` file.
-
-## Setting up
-
-In order to begin using the EduDraw class to make your drawings, you need to do a few steps first:
-  
-#### 1. Install the requirements
-
-You need to install the requirements from the requirements file, you can do this by adding the file on your directory and running the following command:
-
-    pip3 install -r requirements.txt
-
-#### 2. Import the implementation file
-
-You can do this by adding this to your imports:
-
-    from edudraw import EduDraw
-
-Make sure the file is in the same directory as the file from which you are using it from or that you properly add the path otherwise.
-
-#### 3. Create an instance of the EduDraw class
-  
-This can be done by simply creating a new EduDraw instance like this:
-    
-    width, height = 500, 500  # Any size you want
-    s = EduDraw(width, height)
-    
-#### 4. Create a ```setup()``` and a ```draw()``` function
-
-These functions are the core of your drawing. ```setup()``` runs once and before ```draw()```, and it is used to set up the environment for the drawings that you want to do. Some things (like the frame rate) must be set in here, before the drawing actually begins. 
-  
-```draw()```, on the other hand, runs every frame, and is where you will give life to your graphics. Here is where shapes and elements will get drawn to the screen.
-
-#### 5. Call ```s.start(setup, draw, window_title)``` 
- 
-Once you run this method on the instance you made for the EduDraw class, the simulation will start and keep running until you give it a halt command or close the window.
-You need to pass the ```setup()``` and ```draw()``` functions you made, and also a ```window_title``` to give the running window a name.
-
-The general structure of your form code may look something like this:
-
-```
-from eduraw import EduDraw
-
-def setup():
-    # Setting up goes here...
-
-def draw():
-    # Drawing goes here...
-
-s = EduDraw(500, 500)
-s.start(setup, draw, "My cool window")
-```
-
-And now you're ready to get onto some drawings :D
-
-## Getting started (with a simple example)
-
-Now that you have your canvas ready for the show, it's time to actually draw something on the screen. To begin with,let's draw a circle on the screen with a white background. Our code might look something like this:
-
-```
-from edudraw import EduDraw
-
-s = EduDraw(500, 300)
-
-def setup():
-    pass
-
-def draw():
-    s.background((255, 255, 255))
-    s.circle_mode('TOP_LEFT')
-    s.circle(s.width // 2, s.height // 2, 24)
-
-s.start(setup, draw, "My first drawing")
-```
-
-And our canvas looks like this:
-
-
-![img1](https://github.com/MuriloLCN/Simple-Draw-Python/assets/88753590/b6ec2e1f-9b75-4c02-88fc-d66ef73c6909)
-
-
-That's our circle! But this is not very interesting, so let's give it a red filling color, a blue outline and make it move around.
-
-```
-from edudraw import EduDraw
-
-s = EduDraw(500, 300)
-
-
-def setup():
-    pass
-
-
-velocity = 5
-ball_position = [50, 50]
-
-
-def draw():
-    global ball_position
-    s.background((255, 255, 255))
-    s.circle_mode('TOP_LEFT')
-    s.fill((255, 0, 0))
-    s.stroke((0, 0, 255))
-    ball_position[0] += velocity
-    ball_position[1] += velocity
-
-    s.circle(ball_position[0], ball_position[1], 24)
-
-s.start(setup, draw, "My first drawing")
-```
-
-![img2](https://github.com/MuriloLCN/Simple-Draw-Python/assets/88753590/b780f016-ef8f-4f66-8d29-120736602985)
-
-
-Now we have a moving red ball :D, but it leaves the screen fairly quickly, so let's make it bounce around.
-
-```
-from edudraw import EduDraw
-
-s = EduDraw(500, 300)
-
-width, height = 0, 0
-velocity = [5, 5]
-ball_position = [50, 50]
-
-
-def setup():
-    global width, height
-    width = s.width
-    height = s.height
-
-
-def draw():
-    global ball_position, velocity
-    s.background((255, 255, 255))
-    s.circle_mode('CENTER')
-    s.fill((255, 0, 0))
-    s.stroke((0, 0, 255))
-
-    if ball_position[1] < 0 or ball_position[1] + 42 > height:
-        velocity[1] *= -1
-
-    if ball_position[0] < 0 or ball_position[0] + 42 > width:
-        velocity[0] *= -1
-
-    ball_position[0] += velocity[0]
-    ball_position[1] += velocity[1]
-
-    s.circle(ball_position[0], ball_position[1], 24)
-
-
-s.start(setup, draw, "My first drawing")
-```
-
-![bouncing_ball](https://github.com/MuriloLCN/Simple-Draw-Python/assets/88753590/7ff0d89d-95c0-4cab-bd57-13fa8cee4f47)
-
-
-And just like that, we've got a ball that bounces around like a DVD screensaver (I wonder when it'll hit the corners...), you should try for yourself.
-
-This example was just to give you an idea of how you can work with this interface, and there is so much you can do with this, it's all up to you.
-
-# Documentation
-
-## State methods
-
-These methods don't directly draw onto the screen, but rather control aspects of the simulation.
-
-### EduDraw(width: int, height: int, null_mode: bool = False)
-
-Initializer for the EduDraw class.
-
-Parameters:
-
-width, height: The width and height of the window to be created
-
-null_mode: Whether null mode should be used or not. Default: False. See more about null mode at the end.
-
-Returns a new instance of the EduDraw class.
-
-### EduDraw.start(setup, draw, window_title: str)
-
-Starts the simulation.
-
-Parameters:
-
-setup: The setup() function written by the user
-
-draw: The draw() function written by the user
-
-window_title: A string to be used as a title for the window running the simulation. Note: This parameter is unused for null mode instances.
-
-### EduDraw.rect_mode(mode: str)
-
-Changes the current mode for drawing squares, rectangles and images.
-
-If ```mode``` is ```'TOP_LEFT'``` (which is the default), the (X,Y) coordinates passed in for the ```rect()``` and ```square()``` methods will represent the top left coordinate of the rectangle.
-
-On the other hand, if ```mode``` is ```'CENTER'```, the (X,Y) coordinates passed in for the methods above will represent the position of the center of the rectangle and the resulting position will be calculated based on it. 
-
-Example:
-```
-    def draw():
-        s.background((200, 200, 200))
-
-        s.no_fill()
-
-        s.stroke((255, 0, 0))
-        s.rect(50, 25, 100, 50) # Rectangle with RECT_MODE as TOP_LEFT
-
-        s.stroke((0, 0, 255))
-        s.rect_mode('CENTER')
-        s.rect(50, 25, 100, 50) # Same rectangle with RECT_MODE as CENTER
-
-        s.stroke((0,0,0))
-        s.stroke_weight(3)
-        s.point(50, 25)  # Point at the (x,y) coordinates passed in for the rectangles above
-    
-```
-
-![rectmode](https://user-images.githubusercontent.com/88753590/233815069-b4ab097a-52f3-4475-967c-9c4a65fa881c.png)
-
-
-### EduDraw.circle_mode(mode: str)
-
-Changes the current mode for drawing circles and ellipses.
-
-If ```mode``` is ```'TOP_LEFT'```, the (X,Y) coordinates passed in for the ```circle()``` and ```ellipse()``` methods will represent the top left coordinate of the rectangle which contains the ellipse. 
-
-On the other hand, if ```mode``` is ```'CENTER'``` (which is the default), the (X,Y) coordinates passed in for the methods above will represent the position of the center of the ellipse and the resulting position will be calculated based on it. 
-
-```
-def draw():
-    s.background((200, 200, 200))
-
-    s.no_fill()
-    s.stroke_weight(3)
-
-    # Three circles at the same starting pos. with circle_mode as TOP_LEFT
-    s.circle_mode('TOP_LEFT')
-
-    s.stroke((255, 0, 0))
-    s.circle(50, 50, 25)
-
-    s.stroke((0, 255, 0))
-    s.circle(50, 50, 18)
-
-    s.stroke((0, 0, 255))
-    s.circle(50, 50, 8)
-
-    # Three circles at the same starting pos. with circle_mode as CENTER
-    s.circle_mode('CENTER')
-
-    s.circle(150, 50, 25)
-    s.stroke((255, 0, 0))
-    s.circle(150, 50, 18)
-    s.stroke((0, 255, 0))
-    s.circle(150, 50, 8)
-
-    s.stroke((0, 0, 0))
-    s.point(150, 50)
-    s.point(50, 50)
-```
-
-![circlemode](https://user-images.githubusercontent.com/88753590/233815073-8bb60f23-9c03-4c0d-982e-fc4e8a2319fc.png)
-
-
----
-
-### EduDraw.fill(color: tuple)
-
-Makes all shapes drawn after this call to be filled in with a given color.
-
-Parameters:
-
-color: A tuple containing the (R, G, B) values of the color to fill the subsequent shapes.
-
-Example:
-```
-    def draw():
-        s.background((255, 255, 255))
-        
-        s.stroke_weight(2)
-        s.no_fill()
-        s.stroke((0, 255, 0))
-        s.square(50, 50, 50)
-
-        s.fill((255, 255, 0))
-        s.circle(100, 150, 25)
-```
-
-![fill](https://user-images.githubusercontent.com/88753590/233815075-ed143b96-8cae-4f8d-ba53-338467a036d9.png)
-
-### EduDraw.no_fill()
-
-Makes all shapes drawn after this call to not be filled in.
-
-### EduDraw.font(new_font: str, font_size: int = 12, bold=False, italic=False, underline=False)
-
-Changes the font to be used when writing text. When the font is changed, all text will have it's font size, so the parameter for size in the `text()` method is not used. Note: This is a costly method, if possible, it's recommended to use it once in `setup()` instead of every frame in `draw()`. If you need to change font mid-drawing, it's recommended to use `font_from_instance()` instead with a preloaded font.
-
-Parameters:
-
-new_font: The name of the font to be used. See [Pygame fonts](https://www.pygame.org/docs/ref/font.html#pygame.font.get_fonts)
-
-font_size: The size of the font to be used.
-
-bold: Whether the font should be bold or not. Default: False
-
-italic: Whether the font should be italic or not. Default: False
-
-underline: Whether the font should have an underline or not. Default: False
-
-### EduDraw.font_from_instance(new_font: pygame.font.Font)
-
-Sets the font to be used when writing text to a premade instance of a `pygame.font.Font` object. It is recommended that, if you need to change fonts mid-drawing, you preload those fonts once before in your program and use this method to change them, instead of using the normal `font()` method, since it's costly to keep creating new instances every frame and the effect this has on performance is noticeable.
-
-Parameters:
-
-new_font: A `pygame.font.Font` instance to be used for text.
-
-### EduDraw.change_default_font(new_font: str, font_size: int = 12, bold=False, italic=False, underline=False)
-
-Changes the default font to be used. This method is meant to be called in `setup()`, and is the preferred way of changing the font.
-The parameters are the same as `font()`.
-
-### EduDraw.reset_font()
-
-Resets the font used to the default one.
-
-### EduDraw.stroke(color: tuple)
-
-Makes all shapes drawn after this call to have their outlines drawn with a given color.
-
-Parameters:
-
-color: A tuple containing the (R, G, B) values of the color to draw the outlines of the subsequent shapes.
-
-Example:
-```
-def draw():
-    s.background((200, 200, 200))
-
-    s.stroke_weight(2)
-
-    s.fill((255, 0, 0))
-    s.no_stroke()
-
-    s.square(20, 30, 60)
-
-    s.fill((100, 100, 100))
-    s.stroke((0, 0, 255))
-
-    s.triangle(200, 200, 300, 300, 350, 150)
-```
-
-![stroke](https://user-images.githubusercontent.com/88753590/233815081-9336437f-1eb6-41d9-81a2-15ecfcc8d0b4.png)
-
-### EduDraw.no_stroke()
-
-Makes all subsequent shapes not have their outlines drawn. 
-
-### EduDraw.stroke_weight(new_weight: int)
-
-Changes how thick or thin the stroke lines are, smaller numbers means thinner outlines, bigger numbers mean thicker outlines.
-
-Note: Due to the way antialiasing works with `gfxdraw`, the stroke weight has NO effect when drawing antialiased primitives and is always 1px.
-
-Parameters:
-
-new_weight: The size (in px) of the stroking line.
-
-Example:
-```
-def draw():
-    s.background((200, 200, 200))
-
-    s.stroke_weight(1)
-    s.line(0, 20, s.width, 20)
-
-    s.stroke_weight(2)
-    s.line(0, 40, s.width, 40)
-
-    s.stroke_weight(4)
-    s.line(0, 60, s.width, 60)
-
-    s.stroke_weight(8)
-    s.line(0, 80, s.width, 80)
-```
-
-![strokeweight](https://user-images.githubusercontent.com/88753590/233815088-a628b74a-5d95-4188-bcd0-14c96c4ac359.png)
-
-
-### EduDraw.push() 
-
-Toggles the temporary state on. All color, font and weight changes made while this mode is on will be reverted once it is left.
-
-### EduDraw.pop()
-
-Toggles the temporary state off.
-
-Example:
-```
-    def draw():
-        s.background((200, 200, 200))
-        s.circle_mode('TOP_LEFT')
-
-        s.stroke_weight(2)
-
-        s.fill((255, 0, 0))
-        s.stroke((0, 0, 255))
-
-        s.square(50, 50, 50)
-        s.circle(100, 50, 25)
-
-        s.push()
-        s.fill((255, 255, 0))
-        s.square(100, 100, 50)
-        s.pop()
-
-        s.circle(50, 100, 25)
-```
-
-![pushpop](https://user-images.githubusercontent.com/88753590/233815098-cd98f137-5065-4fb5-89e8-8606ac9637a3.png)
-
-Example 2:
-```
-    def draw():
-        # Setting up visuals
-        s.circle_mode('TOP_LEFT')
-        s.stroke_weight(2)
-        s.background((255, 255, 255))
-        s.translate(50, 0)
-        s.stroke((0, 0, 255))
-
-        # Main state: Red circle
-        s.fill((255, 0, 0))
-        s.circle(0, 50, 25)
-
-        s.push()
-        # Second state: Green circle, translated 10px below main state
-        s.translate(0, 10)
-        s.fill((0, 255, 0))
-        s.circle(50, 50, 25)
-
-        s.push()
-        # Third state: Blue circle, translated 10px below second state (20px below main state - it's cumulative)
-        s.translate(0, 10)
-        s.fill((0, 0, 255))
-        s.circle(100, 50, 25)
-
-        s.pop()
-        # Leave third state
-        s.circle(150, 50, 25)
-
-        s.pop()
-        # Leave second state
-        s.circle(200, 50, 25)
-```
-
-![pushpop2](https://user-images.githubusercontent.com/88753590/236652838-d6181f0e-9349-4437-bf7e-9cc1ae241e12.png)
-
-
-
-### EduDraw.mouse_pos()-> tuple
-
-Gets the current mouse position (relative to the top left corner of the canvas).
-Returns a tuple with the X,Y position of the cursor.
-
-Returns:
-
-A tuple with the coordinates of the mouse relative to the canvas
-
-Example 1:
-```
-def draw():
-    s.background((200, 200, 200))
-
-    mouse_x, mouse_y = s.mouse_pos()
-    s.no_fill()
-
-    if 75 <= mouse_x <= 150:
-        if 75 <= mouse_y <= 150:
-            s.fill((255, 255, 0))
-
-    s.circle(mouse_x, mouse_y, 3)
-
-    s.square(75, 75, 75)
-
-    s.stroke((0, 255, 0))
-    s.text(f"X: {mouse_x}", 10, 10)
-    s.stroke((255, 0, 0))
-    s.text(f"Y: {mouse_y}", 10, 30)
-```
-
-![mousepos](https://user-images.githubusercontent.com/88753590/233815197-3eb81842-bb44-4e51-95ad-f4e4ffe52be4.gif)
-
-You can set whether this function should or not revert transformations to retrieve the perceived position by using
-`EduDraw.set_account_for_transformations(True)`, the example below illustrates the difference:
-
-Example 2:
-```
-    def draw():
-        s.set_account_for_transformations(False)
-        s.background((255, 255, 255))
-        s.stroke((200, 0, 200))
-
-        s.scale(1.1, 1.4)
-        s.rotate(s.frame_count)
-        s.translate(s.width // 2, s.height // 2)
-
-        # Line to illustrate rotation of the canvas
-        s.line(s.width // 2, s.height // 2, 0, 0)
-
-        no_account = s.mouse_pos()
-
-        s.set_account_for_transformations(True)
-
-        account = s.mouse_pos()
-
-        # Light blue circle where the perceived mouse position is
-        s.fill((150, 150, 255))
-        s.circle(account[0], account[1], 12)
-
-        # Red blue circle where the actual mouse position is
-        s.fill((255, 0, 0))
-        s.circle(no_account[0], no_account[1], 12)
-
-        s.line(0, 0, account[0], account[1])
-```
-
-![mouseaccount](https://user-images.githubusercontent.com/88753590/236652900-93e10e80-1e5a-4c06-8db6-00b7f9afd7bd.gif)
-
-
-### EduDraw.rotate(angle: int)
-
-Rotates the drawing clockwise by the defined amount of degrees.
-Note: Is cumulative with other rotations.
-
-Parameters:
-
-angle: The angle (in degrees) to rotate the drawing
-
-Example:
-```
-def draw():
-    s.background((255, 255, 255))
-    s.stroke((255, 0, 0))
-    s.line(50, 50, 100, 50)
-
-    s.rotate(10)
-    # Current angle: 10 degrees
-    
-    s.stroke((0, 0, 255))
-    s.line(50, 50, 100, 50)
-
-    s.rotate(10)
-    # Current angle: 20 degrees
-
-    s.stroke((100, 255, 100))
-    s.line(50, 50, 100, 50)
-
-    s.rotate(-15)
-    # Current angle: 5 degrees
-    
-    s.stroke((255, 200, 0))
-    s.line(50, 50, 100, 50)
-
-    s.rotate(-10)
-    # Current angle: -5 degrees (355 degrees)
-
-    s.stroke((0, 255, 255))
-    s.line(50, 50, 100, 50)
-```
-
-![rotation](https://user-images.githubusercontent.com/88753590/236652911-7dba1539-0b43-468c-a1ba-d707c20a8730.png)
-
-Example 2:
-
-```
-def draw():
-    s.background((255, 255, 255))
-    s.fill((0, 0, 0))
-    s.fill((255, 0, 0))
-    s.circle_mode('CENTER')
-    s.rotate(s.frame_count)
-    s.translate(s.width // 2, s.height // 2)
-    s.circle(0, 0, 10)
-    s.push()
-    s.fill((0, 255, 0))
-    s.reset_translation()
-    s.rotate(s.frame_count)
-    s.translate(s.width // 2, s.height // 2)
-    s.circle(20, 0, 10)
-    s.push()
-    s.fill((0, 0, 255))
-    s.reset_translation()
-    s.rotate(s.frame_count)
-    s.translate(s.width // 2, s.height // 2)
-    s.circle(40, 0, 10)
-    s.pop()
-    s.circle(60, 0, 10)
-    s.pop()
-    s.circle(80, 0, 10)
-```
-
-![advancedexample](https://user-images.githubusercontent.com/88753590/236653135-d38838d1-518c-4b70-a664-ea121cf71315.gif)
-
-
-
-### EduDraw.scale(scale_x: float, scale_y: float) 
-
-Scales the drawing's axis by the desired multipliers
-Note: Is cumulative with other scalars.
-
-Parameters:
-
-scale_x: The multiplier to apply in the x axis
-scale_y: The multiplier to apply in the y axis
-
-Example:
-```
- def draw():
-    s.background((255, 255, 255))
-    s.fill((200, 200, 0))
-
-    s.square(50, 50, 25)
-
-    s.scale(2, 0.5)
-
-    s.fill((0, 0, 200))
-    s.square(50, 50, 25)
-
-    s.reset_scaling()
-    s.scale(0.75, 1.25)
-
-    s.fill((255, 0, 0))
-    s.square(50, 50, 25)
-
-    s.reset_scaling()
-
-    s.fill((0, 255, 0))
-    s.square(75, 75, 25)
-```
-
-![scale](https://user-images.githubusercontent.com/88753590/236652949-f882daf2-fba5-4cd4-8e62-5d418b3fbfee.png)
-
-
-### EduDraw.translate(translate_x: int, translate_y: int)
-
-Changes the origin of the plane of drawing.
-Note: Is cumulative with other translations.
-
-Parameters:
-
-translate_x: The amount to translate in the x axis
-translate_y: The amount to translate in the y axis
-
-Example:
-```
-def draw():
-    s.translate(0, 0)
-    s.background((255, 255, 255))
-    s.fill((125, 125, 125))
-    s.square(50, 50, 50)
-
-    s.translate(-50, 50)
-    s.fill((200, 200, 0))
-    s.square(50, 50, 50)
-```
-
-![translate](https://user-images.githubusercontent.com/88753590/236652958-1b89304d-9cb0-4104-9806-82dc0c8e9f3c.png)
-
-
-### EduDraw.reset_transformations()
-
-Resets all transformations applied.
-
-### EduDraw.reset_scaling() 
-
-Resets all scaling transformations applied.
-
-### EduDraw.reset_translation() 
-
-Resets all translation transformations applied.
-
-### EduDraw.reset_rotation() 
-
-Resets all rotation transformations applied.
-
-### EduDraw.set_account_for_transformations(state: bool) 
-
-Changes wether `mouse_pos()` should yield the real or perceived position of the mouse.
-
-Parameters:
-
-state: The state to apply to this setting. `True` yields the perceived position, whereas `False` (the default) yields the real position.
-
-### EduDraw.set_controls(key_down=None, key_up=None, mouse_motion=None, mouse_button_up=None, mouse_button_down=None, mouse_wheel=None)
-
-Sets functions to be ran on each specific Pygame event. `None` means that nothing will occur on those events.
-Each function must have a parameter to receive a dictionary containing the data related to that event (such
-as which key was pressed, where the mouse is, etc.)
-
-Parameters:
-
-key_down: The function to be ran when a key is pressed down
-
-key_up: The function to be ran when a key is released
-
-mouse_motion: The function to be ran when the mouse is moved
-
-mouse_button_up: The function to be ran when a mouse button is released
-
-mouse_button_down: The function to be ran when a mouse button is pressed
-
-mouse_wheel: The function to be ran when the mouse wheel is scrolled
-        
-Example:
-
-```
-s = EduDraw(400, 400)
-
-bg_color = (200, 200, 200)
-text = ''
-
-def setup():
-    s.set_controls(mouse_button_down=do_stuff_on_click)
-
-def draw():
-    s.background(bg_color)
-    s.text(text, s.width // 2, s.height // 2)
-
-count = 0
-def do_stuff_on_click(data: dict):
-    global count, bg_color, text
-    if count % 2 == 0:
-        bg_color = (0, 0, 0)
-        text = ''
-    else:
-        bg_color = (255, 255, 255)
-        text = 'Clicked!'
-    count += 1
-
-s.start(setup, draw, 'Hello')
-```
-
-Example 2:
-
-```
-my_word = ''
-
-def setup():
-    s.set_controls(key_down=get_char)
-    s.change_default_font('times new roman', 30, italic=True)
-
-def draw():
-    s.fill((255, 255, 255))
-    s.background((0, 0, 0))
-    s.rect_mode("CENTER")
-    s.text(my_word, s.width // 2, s.height // 2)
-
-def get_char(data: dict):
-    global my_word
-    print(data)
-    unicode = data['unicode']
-    if unicode == '\x08':
-        my_word = my_word[:-1]
-    else:
-        my_word += data['unicode']
-```
-
-![keyexample](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/ddb1a44e-77a0-46f3-bf10-fff2d76989ec)
-
-
-### EduDraw.toggle_antialising()
-
-Toggles antialiasing on or off. It's off by default.
-
-Note: Antialiasing needs more processing, especially when the number of shapes and their complexity is higher. Also, antialised shapes do not take
-into account the stroke weight of the lines, and all lines are drawn with the weight of 1px.
-
-## Drawing methods
-
-These methods draw onto the canvas.
-
-### EduDraw.point(x: int, y: int)
-
-Draws a point at coordinates (x,y)
-
-Parameters:
-
-x, y: The x,y coordinates to draw the point onto.
-
-### EduDraw.text(string: str, x: int, y: int)
-
-Writes a string of text onto the screen.
-
-Parameters:
-
-string: The text to be written
-
-x, y: The coordinates of the top-left corner of the text if rect_mode is 'TOP_LEFT' or the middle of the text is rect_mode is 'CENTER'.
-
-
-### EduDraw.background(color: tuple)
-
-Sets a new background color and clears the canvas to it.
-
-Parameters:
-
-color: A tuple containing the (R, G, B) values of the desired color.
-
-### EduDraw.circle(x: int, y: int, radius: int)
-
-Draws a circle onto the screen.
-
-Parameters:
-
-x, y: The coordinates of the top-left part of the rectangle that contains the circle if circle_mode is 'TOP_LEFT', or the center of the circle if circle_mode is 'CENTER'.
-
-r: The radius of the circle.
-
-### EduDraw.ellipse(x: int, y: int, width: int, height: int)
-
-Draws an ellipse onto the screen.
-
-Parameters:
-
-x, y: The coordinates of the top-left part of the rectange that contains the ellipse if circle_mode is 'TOP_LEFT', or the center of the ellipse if circle_mode is 'CENTER'.
-
-w, h: The width and height of the rectangle that contains the ellipse.
-
-Example:
-```
-def draw():
-    s.background((200, 200, 200))
-
-    s.stroke_weight(3)
-    s.circle_mode('TOP_LEFT')
-
-    s.fill((100, 100, 100))
-    s.stroke((0, 0, 255))
-    s.ellipse(62, 40, 45, 70)
-
-    s.no_fill()
-    s.stroke((255, 0, 0))
-    s.ellipse(50, 50, 70, 30)
-```
-
-![ellipse](https://user-images.githubusercontent.com/88753590/233815202-95fc61d6-b328-4783-85ec-e5f7df4b153a.png)
-
-
-### EduDraw.line(x1: int, y1: int, x2: int, y2: int)
-
-Draws a line between two points.
-
-Parameters:
-
-x1, y1: The coordinates of the first point.
-
-x2, y2: The coordinates of the second point.
-
-Example:
-```
-def draw():
-    s.background((200, 200, 200))
-    s.stroke_weight(3)
-
-    s.line(0, 0, s.width, s.height)
-    s.stroke((0, 0, 255))
-    s.line(0, s.height // 2, s.width, s.height // 2)
-    s.stroke((255, 0, 0))
-    s.line(200, 300, 400, 250)
-```
-
-![line](https://user-images.githubusercontent.com/88753590/233815204-d355aed5-f9e0-42f3-88b2-90feaf1bfe11.png)
-
-
-### EduDraw.rect(x: int, y: int, width: int, height: int)
-
-Draws a rectangle onto the screen.
-
-Parameters:
-
-x, y: The coordinates of the top-left corner of the rectangle if rect_mode is 'TOP_LEFT', or the center of the rectangle if rect_mode is 'CENTER'.
-
-width, height: The width and height of the rectangle.
-
-Example:
-```
-def draw():
-    s.background((200, 200, 200))
-    s.stroke_weight(3)
-
-    x = 50
-    y = 60
-
-    dx = 5
-    dy = 5
-
-    s.no_fill()
-
-    s.rect(x, y, 50, 90)
-
-    s.stroke((255, 0, 0))
-    s.rect(y, x, 90, 50)
-
-    s.stroke((0, 0, 255))
-    s.rect(x + dx, y + dy, 50 - dx * 2, 90 - dy * 2)
-```
-
-![rect](https://user-images.githubusercontent.com/88753590/233815207-f7f8732b-88ae-4f17-92b7-16006b05237a.png)
-
-
-### EduDraw.square(x: int, y: int, side_size: int)
-
-Draws a square onto the screen.
-
-Parameters:
-
-x, y: The coordinates of the top-left corner of the square if rect_mode is 'TOP_LEFT', or the center of the square if rect_mode is 'CENTER'.
-
-side_size: The size of the sides of the square.
-
-Example:
-```
-def draw():
-    s.background((255, 255, 255))
-
-    s.no_stroke()
-    s.fill((0, 0, 0))
-
-    for i in range(0, s.width, 25):
-        for j in range(0, s.height, 25):
-            if ((i + j) % 2) == 0:
-                s.square(i, j, 25)
-```
-
-![square](https://user-images.githubusercontent.com/88753590/233815209-c043af52-74ed-4b87-939f-39024043e458.png)
-
-
-### EduDraw.triangle(x1: int, y1: int, x2: int, y2: int, x3: int, y3: int)
-
-Draws a triangle onto the screen.
-
-Parameters:
-
-x1,y1: The coordinates of the first vertex of the triangle.
-
-x2,y2: The coordinates of the second vertex of the triangle.
-
-x3,y3: The coordinates of the third vertex of the triangle.
-
-Example:
-```
-def draw():
-    s.background((200, 200, 200))
-
-    s.fill((255, 255, 0))
-
-    s.triangle(40, 40, 120, 40, 80, 120)
-    s.triangle(120, 40, 200, 40, 160, 120)
-    s.triangle(80, 120, 160, 120, 120, 200)
-```
-
-![triangle](https://user-images.githubusercontent.com/88753590/233815214-5f44f6b7-4d0a-41f8-88f8-3b384e1d117f.png)
-
-
-
-### EduDraw.polygon(points: list)
-
-Draws any polygon onto the screen.
-
-Parameters:
-
-points: An array containing tuples with all of the vertices of the polygon.
-
-Example:
-```
-def draw():
-    s.background((200, 200, 200))
-
-    s.fill((100, 255, 255))
-    points = [
-        (50, 50),
-        (100, 50),
-        (120, 100),
-        (75, 135),
-        (30, 100)
-    ]
-
-    s.polygon(points)
-```
-
-![polygon](https://user-images.githubusercontent.com/88753590/233815221-2da1f919-571f-40a2-ad96-cb4e4084875b.png)
-
-
----
-
-### EduDraw.image(img: pygame.surface.Surface, x: int, y: int, width: int = None, height: int = None):
-    
-Displays an image onto the screen on the (x,y) position. If specified a width or height, the image will be resized to those sizes, otherwise, the image will be drawn to it's original size.
-    
-Parameters:
-
-img: The image to be drawn onto the canvas
-    
-x, y: The position to draw the image
-    
-(Optional) width, height: The sizes to set the image to
-
-```
-my_image = pygame.image.load('testimage.jpeg')
-
-def setup():
-    pass
-
-def draw():
-    s.fill((255, 255, 255))
-    s.background((0, 0, 0))
-    s.rect_mode("CENTER")
-    s.image(my_image, s.width // 2, s.height // 2, s.width // 2, s.height // 2)
-```
-
-![img](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/4dba8d75-7061-469d-a5fc-851908eb6d0f)
-
-
-### EduDraw.frame_rate(fps: int)
-
-Changes the framerate of the simulation. Must be called in ```setup()```.
-Note that in the Python version the simulation does not run as fast as the C# one, to run the simulation as fast as possible set the EduDraw.deltatime to zero.
-
-Parameters:
-
-int frames: The number of FPS to set the simulation to.
-
-
-### EduDraw.save(filename: str)
-
-Saves the current frame as an image file.
-If filename is empty, the name will be the frame count of when the photo was saved.
-
-
-### EduDraw.quit()
-
-Quits the simulation.
-
-### Null mode
-
-Null mode is a mode in which you can run an instance of a simulation without having it running directly onto the canvas. You can do this for many reasons, including using EduDraw in a different context or application, creating multiple drawings inside of one another, among other things.
-
-To initialize an EduDraw instance in null mode, you can use the optional parameter for it in the `start()` method.
-
-Example of null mode:
-
-```
-s = EduDraw(500, 500) # Main instance
-d = EduDraw(250, 250, True) # Null mode ('inner') instance
-
-def setup():
-  {...}
-
-def draw():
-  {...}
-
-def inner_setup():
-  {...}
-
-def inner_draw():
-  {...}
-  
-s.start(setup, draw, "My window title")
-d.start(inner_setup, inner_draw, "This text is not shown")
-```
-
-In order to be able to visualize instance of null mode, you'll have to retrieve the images (`pygame.surface.Surface`) and use those in your drawing or any other desired output (whether that be an icon, a display, a file, etc.).
-
-You can retrieve the images with the `EduDraw.screen` variable. With that Surface object retrieved, you can use it wherever it's necessary, and you have much more flexibility for what to do with it.
-
-A good example of this is to run two instances of EduDraw, one normal and one null, and use the retrieved images from the null instance as an argument for EduDraw.image(), essentially creating a drawing inside of a drawing, like the example below:
-
-```
-s = EduDraw(200, 200)
-d = EduDraw(100, 100, True)
-
-position = [d.width/2, d.height//2]
-velocity = [3, 4]
-
-# We don't need to setup anything in this case
-def setup():
-    pass
-
-def inner_drawing():
-    global position, velocity
-    if position[0] < 0 or position[0] > d.width:
-        velocity[0] *= -1
-
-    if position[1] < 0 or position[1] > d.height:
-        velocity[1] *= -1
-
-    position[0] += velocity[0]
-    position[1] += velocity[1]
-
-    d.fill((255, 0, 0))
-    d.stroke((0, 0, 255))
-    d.circle(position[0], position[1], 5)
-
-def draw():
-    s.background((200, 200, 200))
-    s.rotate(s.frame_count)
-    s.rect_mode("CENTER")
-    s.translate(s.width // 2, s.height // 2)
-    s.image(d.screen, 0, 0)
-    
-d.start(setup, inner_drawing, "This does not appear")
-s.start(setup, draw, "My drawing :D")
-```
-
-![nullmode](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/5026c565-f081-49cf-8bfd-55fe487bada6)
-
+# Edu-Draw-Python
+
+This is the Python version of EduDraw, for the C# version, please see [Edu Draw C#](https://github.com/MuriloLCN/Simple-Draw-Csharp)
+
+This project is aimed to provide an interface that allows for a simplified experience when using basic 2D graphics in the Python language. 
+
+The general design of the interface is heavily (if not all) inspired by the [P5.js](https://p5js.org/) library and the Processing library, and is intended to make simple graphical programs easy to do in the .NET environment in the shape of a Windows Forms app and/or in the Python language.
+
+The details of installation and documentation of the respective versions are below. 
+
+## Installation
+
+You can install the package using PIP by typing the following command: `pip install edudraw`, and import it in your code like any other library.
+You'll need the pygame library as well, in case it doesn't get automatically installed.
+
+## Setting up
+
+In order to begin using the EduDraw class to make your drawings, you need to do a few steps first:
+  
+#### 1. Install the library and the requirements
+
+The only requirement for this library is `pygame==2.1.2`.
+
+#### 2. Import the library
+
+You can do this by adding this to your imports:
+
+    from EduDraw import edudraw
+
+Make sure the file is in the same directory as the file from which you are using it from or that you properly add the path otherwise.
+
+#### 3. Create an instance of the EduDraw class
+  
+This can be done by simply creating a new EduDraw instance like this:
+    
+    width, height = 500, 500  # Any size you want
+    s = edudraw.EduDraw(width, height)
+    
+#### 4. Create a ```setup()``` and a ```draw()``` function
+
+These functions are the core of your drawing. ```setup()``` runs once and before ```draw()```, and it is used to set up the environment for the drawings that you want to do. Some things (like the frame rate) must be set in here, before the drawing actually begins. 
+  
+```draw()```, on the other hand, runs every frame, and is where you will give life to your graphics. Here is where shapes and elements will get drawn to the screen.
+
+#### 5. Call ```s.start(setup, draw, window_title)``` 
+ 
+Once you run this method on the instance you made for the EduDraw class, the simulation will start and keep running until you give it a halt command or close the window.
+You need to pass the ```setup()``` and ```draw()``` functions you made, and also a ```window_title``` to give the running window a name.
+
+The general structure of your form code may look something like this:
+
+```
+from EduDraw import edudraw
+
+def setup():
+    # Setting up goes here...
+
+def draw():
+    # Drawing goes here...
+
+s = edudraw.EduDraw(500, 500)
+s.start(setup, draw, "My cool window")
+```
+
+And now you're ready to get onto some drawings :D
+
+## Getting started (with a simple example)
+
+Now that you have your canvas ready for the show, it's time to actually draw something on the screen. To begin with,let's draw a circle on the screen with a white background. Our code might look something like this:
+
+```
+from EduDraw import edudraw
+
+s = edudraw.EduDraw(500, 300)
+
+def setup():
+    pass
+
+def draw():
+    s.background((255, 255, 255))
+    s.circle_mode('TOP_LEFT')
+    s.circle(s.width // 2, s.height // 2, 24)
+
+s.start(setup, draw, "My first drawing")
+```
+
+And our canvas looks like this:
+
+
+![img1](https://github.com/MuriloLCN/Simple-Draw-Python/assets/88753590/b6ec2e1f-9b75-4c02-88fc-d66ef73c6909)
+
+
+That's our circle! But this is not very interesting, so let's give it a red filling color, a blue outline and make it move around.
+
+```
+from EduDraw import edudraw
+
+s = edudraw.EduDraw(500, 300)
+
+
+def setup():
+    pass
+
+
+velocity = 5
+ball_position = [50, 50]
+
+
+def draw():
+    global ball_position
+    s.background((255, 255, 255))
+    s.circle_mode('TOP_LEFT')
+    s.fill((255, 0, 0))
+    s.stroke((0, 0, 255))
+    ball_position[0] += velocity
+    ball_position[1] += velocity
+
+    s.circle(ball_position[0], ball_position[1], 24)
+
+s.start(setup, draw, "My first drawing")
+```
+
+![img2](https://github.com/MuriloLCN/Simple-Draw-Python/assets/88753590/b780f016-ef8f-4f66-8d29-120736602985)
+
+
+Now we have a moving red ball :D, but it leaves the screen fairly quickly, so let's make it bounce around.
+
+```
+from EduDraw import edudraw
+
+s = edudraw.EduDraw(500, 300)
+
+width, height = 0, 0
+velocity = [5, 5]
+ball_position = [50, 50]
+
+
+def setup():
+    global width, height
+    width = s.width
+    height = s.height
+
+
+def draw():
+    global ball_position, velocity
+    s.background((255, 255, 255))
+    s.circle_mode('CENTER')
+    s.fill((255, 0, 0))
+    s.stroke((0, 0, 255))
+
+    if ball_position[1] < 24 or ball_position[1] + 24 > height:
+        velocity[1] *= -1
+
+    if ball_position[0] < 24 or ball_position[0] + 24 > width:
+        velocity[0] *= -1
+
+    ball_position[0] += velocity[0]
+    ball_position[1] += velocity[1]
+
+    s.circle(ball_position[0], ball_position[1], 24)
+
+
+s.start(setup, draw, "My first drawing")
+```
+
+![bouncing_ball](https://github.com/MuriloLCN/Simple-Draw-Python/assets/88753590/7ff0d89d-95c0-4cab-bd57-13fa8cee4f47)
+
+
+And just like that, we've got a ball that bounces around like a DVD screensaver (I wonder when it'll hit the corners...), you should try for yourself.
+
+This example was just to give you an idea of how you can work with this interface, and there is so much you can do with this, it's all up to you.
+
+# Documentation
+
+## State methods
+
+These methods don't directly draw onto the screen, but rather control aspects of the simulation.
+
+### EduDraw(width: int, height: int, null_mode: bool = False)
+
+Initializer for the EduDraw class.
+
+Parameters:
+
+width, height: The width and height of the window to be created
+
+null_mode: Whether null mode should be used or not. Default: False. See more about null mode at the end.
+
+Returns a new instance of the EduDraw class.
+
+### EduDraw.start(setup, draw, window_title: str)
+
+Starts the simulation.
+
+Parameters:
+
+setup: The setup() function written by the user
+
+draw: The draw() function written by the user
+
+window_title: A string to be used as a title for the window running the simulation. Note: This parameter is unused for null mode instances.
+
+### EduDraw.rect_mode(mode: str)
+
+Changes the current mode for drawing squares, rectangles and images.
+
+If ```mode``` is ```'TOP_LEFT'``` (which is the default), the (X,Y) coordinates passed in for the ```rect()``` and ```square()``` methods will represent the top left coordinate of the rectangle.
+
+On the other hand, if ```mode``` is ```'CENTER'```, the (X,Y) coordinates passed in for the methods above will represent the position of the center of the rectangle and the resulting position will be calculated based on it. 
+
+Example:
+```
+    def draw():
+        s.background((200, 200, 200))
+
+        s.no_fill()
+
+        s.stroke((255, 0, 0))
+        s.rect(50, 25, 100, 50) # Rectangle with RECT_MODE as TOP_LEFT
+
+        s.stroke((0, 0, 255))
+        s.rect_mode('CENTER')
+        s.rect(50, 25, 100, 50) # Same rectangle with RECT_MODE as CENTER
+
+        s.stroke((0,0,0))
+        s.stroke_weight(3)
+        s.point(50, 25)  # Point at the (x,y) coordinates passed in for the rectangles above
+    
+```
+
+![rectmode](https://user-images.githubusercontent.com/88753590/233815069-b4ab097a-52f3-4475-967c-9c4a65fa881c.png)
+
+
+### EduDraw.circle_mode(mode: str)
+
+Changes the current mode for drawing circles and ellipses.
+
+If ```mode``` is ```'TOP_LEFT'```, the (X,Y) coordinates passed in for the ```circle()``` and ```ellipse()``` methods will represent the top left coordinate of the rectangle which contains the ellipse. 
+
+On the other hand, if ```mode``` is ```'CENTER'``` (which is the default), the (X,Y) coordinates passed in for the methods above will represent the position of the center of the ellipse and the resulting position will be calculated based on it. 
+
+```
+def draw():
+    s.background((200, 200, 200))
+
+    s.no_fill()
+    s.stroke_weight(3)
+
+    # Three circles at the same starting pos. with circle_mode as TOP_LEFT
+    s.circle_mode('TOP_LEFT')
+
+    s.stroke((255, 0, 0))
+    s.circle(50, 50, 25)
+
+    s.stroke((0, 255, 0))
+    s.circle(50, 50, 18)
+
+    s.stroke((0, 0, 255))
+    s.circle(50, 50, 8)
+
+    # Three circles at the same starting pos. with circle_mode as CENTER
+    s.circle_mode('CENTER')
+
+    s.circle(150, 50, 25)
+    s.stroke((255, 0, 0))
+    s.circle(150, 50, 18)
+    s.stroke((0, 255, 0))
+    s.circle(150, 50, 8)
+
+    s.stroke((0, 0, 0))
+    s.point(150, 50)
+    s.point(50, 50)
+```
+
+![circlemode](https://user-images.githubusercontent.com/88753590/233815073-8bb60f23-9c03-4c0d-982e-fc4e8a2319fc.png)
+
+
+---
+
+### EduDraw.fill(color: tuple)
+
+Makes all shapes drawn after this call to be filled in with a given color.
+
+Parameters:
+
+color: A tuple containing the (R, G, B) values of the color to fill the subsequent shapes.
+
+Example:
+```
+    def draw():
+        s.background((255, 255, 255))
+        
+        s.stroke_weight(2)
+        s.no_fill()
+        s.stroke((0, 255, 0))
+        s.square(50, 50, 50)
+
+        s.fill((255, 255, 0))
+        s.circle(100, 150, 25)
+```
+
+![fill](https://user-images.githubusercontent.com/88753590/233815075-ed143b96-8cae-4f8d-ba53-338467a036d9.png)
+
+### EduDraw.no_fill()
+
+Makes all shapes drawn after this call to not be filled in.
+
+### EduDraw.font(new_font: str, font_size: int = 12, bold=False, italic=False, underline=False)
+
+Changes the font to be used when writing text. When the font is changed, all text will have it's font size, so the parameter for size in the `text()` method is not used. Note: This is a costly method, if possible, it's recommended to use it once in `setup()` instead of every frame in `draw()`. If you need to change font mid-drawing, it's recommended to use `font_from_instance()` instead with a preloaded font.
+
+Parameters:
+
+new_font: The name of the font to be used. See [Pygame fonts](https://www.pygame.org/docs/ref/font.html#pygame.font.get_fonts)
+
+font_size: The size of the font to be used.
+
+bold: Whether the font should be bold or not. Default: False
+
+italic: Whether the font should be italic or not. Default: False
+
+underline: Whether the font should have an underline or not. Default: False
+
+### EduDraw.font_from_instance(new_font: pygame.font.Font)
+
+Sets the font to be used when writing text to a premade instance of a `pygame.font.Font` object. It is recommended that, if you need to change fonts mid-drawing, you preload those fonts once before in your program and use this method to change them, instead of using the normal `font()` method, since it's costly to keep creating new instances every frame and the effect this has on performance is noticeable.
+
+Parameters:
+
+new_font: A `pygame.font.Font` instance to be used for text.
+
+### EduDraw.change_default_font(new_font: str, font_size: int = 12, bold=False, italic=False, underline=False)
+
+Changes the default font to be used. This method is meant to be called in `setup()`, and is the preferred way of changing the font.
+The parameters are the same as `font()`.
+
+### EduDraw.reset_font()
+
+Resets the font used to the default one.
+
+### EduDraw.stroke(color: tuple)
+
+Makes all shapes drawn after this call to have their outlines drawn with a given color.
+
+Parameters:
+
+color: A tuple containing the (R, G, B) values of the color to draw the outlines of the subsequent shapes.
+
+Example:
+```
+def draw():
+    s.background((200, 200, 200))
+
+    s.stroke_weight(2)
+
+    s.fill((255, 0, 0))
+    s.no_stroke()
+
+    s.square(20, 30, 60)
+
+    s.fill((100, 100, 100))
+    s.stroke((0, 0, 255))
+
+    s.triangle(200, 200, 300, 300, 350, 150)
+```
+
+![stroke](https://user-images.githubusercontent.com/88753590/233815081-9336437f-1eb6-41d9-81a2-15ecfcc8d0b4.png)
+
+### EduDraw.no_stroke()
+
+Makes all subsequent shapes not have their outlines drawn. 
+
+### EduDraw.stroke_weight(new_weight: int)
+
+Changes how thick or thin the stroke lines are, smaller numbers means thinner outlines, bigger numbers mean thicker outlines.
+
+Note: Due to the way antialiasing works with `gfxdraw`, the stroke weight has NO effect when drawing antialiased primitives and is always 1px.
+
+Parameters:
+
+new_weight: The size (in px) of the stroking line.
+
+Example:
+```
+def draw():
+    s.background((200, 200, 200))
+
+    s.stroke_weight(1)
+    s.line(0, 20, s.width, 20)
+
+    s.stroke_weight(2)
+    s.line(0, 40, s.width, 40)
+
+    s.stroke_weight(4)
+    s.line(0, 60, s.width, 60)
+
+    s.stroke_weight(8)
+    s.line(0, 80, s.width, 80)
+```
+
+![strokeweight](https://user-images.githubusercontent.com/88753590/233815088-a628b74a-5d95-4188-bcd0-14c96c4ac359.png)
+
+
+### EduDraw.push() 
+
+Toggles the temporary state on. All color, font and weight changes made while this mode is on will be reverted once it is left.
+
+### EduDraw.pop()
+
+Toggles the temporary state off.
+
+Example:
+```
+    def draw():
+        s.background((200, 200, 200))
+        s.circle_mode('TOP_LEFT')
+
+        s.stroke_weight(2)
+
+        s.fill((255, 0, 0))
+        s.stroke((0, 0, 255))
+
+        s.square(50, 50, 50)
+        s.circle(100, 50, 25)
+
+        s.push()
+        s.fill((255, 255, 0))
+        s.square(100, 100, 50)
+        s.pop()
+
+        s.circle(50, 100, 25)
+```
+
+![pushpop](https://user-images.githubusercontent.com/88753590/233815098-cd98f137-5065-4fb5-89e8-8606ac9637a3.png)
+
+Example 2:
+```
+    def draw():
+        # Setting up visuals
+        s.circle_mode('TOP_LEFT')
+        s.stroke_weight(2)
+        s.background((255, 255, 255))
+        s.translate(50, 0)
+        s.stroke((0, 0, 255))
+
+        # Main state: Red circle
+        s.fill((255, 0, 0))
+        s.circle(0, 50, 25)
+
+        s.push()
+        # Second state: Green circle, translated 10px below main state
+        s.translate(0, 10)
+        s.fill((0, 255, 0))
+        s.circle(50, 50, 25)
+
+        s.push()
+        # Third state: Blue circle, translated 10px below second state (20px below main state - it's cumulative)
+        s.translate(0, 10)
+        s.fill((0, 0, 255))
+        s.circle(100, 50, 25)
+
+        s.pop()
+        # Leave third state
+        s.circle(150, 50, 25)
+
+        s.pop()
+        # Leave second state
+        s.circle(200, 50, 25)
+```
+
+![pushpop2](https://user-images.githubusercontent.com/88753590/236652838-d6181f0e-9349-4437-bf7e-9cc1ae241e12.png)
+
+
+
+### EduDraw.mouse_pos()-> tuple
+
+Gets the current mouse position (relative to the top left corner of the canvas).
+Returns a tuple with the X,Y position of the cursor.
+
+Returns:
+
+A tuple with the coordinates of the mouse relative to the canvas
+
+Example 1:
+```
+def draw():
+    s.background((200, 200, 200))
+
+    mouse_x, mouse_y = s.mouse_pos()
+    s.no_fill()
+
+    if 75 <= mouse_x <= 150:
+        if 75 <= mouse_y <= 150:
+            s.fill((255, 255, 0))
+
+    s.circle(mouse_x, mouse_y, 3)
+
+    s.square(75, 75, 75)
+
+    s.stroke((0, 255, 0))
+    s.text(f"X: {mouse_x}", 10, 10)
+    s.stroke((255, 0, 0))
+    s.text(f"Y: {mouse_y}", 10, 30)
+```
+
+![mousepos](https://user-images.githubusercontent.com/88753590/233815197-3eb81842-bb44-4e51-95ad-f4e4ffe52be4.gif)
+
+You can set whether this function should or not revert transformations to retrieve the perceived position by using
+`EduDraw.set_account_for_transformations(True)`, the example below illustrates the difference:
+
+Example 2:
+```
+    def draw():
+        s.set_account_for_transformations(False)
+        s.background((255, 255, 255))
+        s.stroke((200, 0, 200))
+
+        s.scale(1.1, 1.4)
+        s.rotate(s.frame_count)
+        s.translate(s.width // 2, s.height // 2)
+
+        # Line to illustrate rotation of the canvas
+        s.line(s.width // 2, s.height // 2, 0, 0)
+
+        no_account = s.mouse_pos()
+
+        s.set_account_for_transformations(True)
+
+        account = s.mouse_pos()
+
+        # Light blue circle where the perceived mouse position is
+        s.fill((150, 150, 255))
+        s.circle(account[0], account[1], 12)
+
+        # Red blue circle where the actual mouse position is
+        s.fill((255, 0, 0))
+        s.circle(no_account[0], no_account[1], 12)
+
+        s.line(0, 0, account[0], account[1])
+```
+
+![mouseaccount](https://user-images.githubusercontent.com/88753590/236652900-93e10e80-1e5a-4c06-8db6-00b7f9afd7bd.gif)
+
+
+### EduDraw.rotate(angle: int)
+
+Rotates the drawing clockwise by the defined amount of degrees.
+Note: Is cumulative with other rotations.
+
+Parameters:
+
+angle: The angle (in degrees) to rotate the drawing
+
+Example:
+```
+def draw():
+    s.background((255, 255, 255))
+    s.stroke((255, 0, 0))
+    s.line(50, 50, 100, 50)
+
+    s.rotate(10)
+    # Current angle: 10 degrees
+    
+    s.stroke((0, 0, 255))
+    s.line(50, 50, 100, 50)
+
+    s.rotate(10)
+    # Current angle: 20 degrees
+
+    s.stroke((100, 255, 100))
+    s.line(50, 50, 100, 50)
+
+    s.rotate(-15)
+    # Current angle: 5 degrees
+    
+    s.stroke((255, 200, 0))
+    s.line(50, 50, 100, 50)
+
+    s.rotate(-10)
+    # Current angle: -5 degrees (355 degrees)
+
+    s.stroke((0, 255, 255))
+    s.line(50, 50, 100, 50)
+```
+
+![rotation](https://user-images.githubusercontent.com/88753590/236652911-7dba1539-0b43-468c-a1ba-d707c20a8730.png)
+
+Example 2:
+
+```
+def draw():
+    s.background((255, 255, 255))
+    s.fill((0, 0, 0))
+    s.fill((255, 0, 0))
+    s.circle_mode('CENTER')
+    s.rotate(s.frame_count)
+    s.translate(s.width // 2, s.height // 2)
+    s.circle(0, 0, 10)
+    s.push()
+    s.fill((0, 255, 0))
+    s.reset_translation()
+    s.rotate(s.frame_count)
+    s.translate(s.width // 2, s.height // 2)
+    s.circle(20, 0, 10)
+    s.push()
+    s.fill((0, 0, 255))
+    s.reset_translation()
+    s.rotate(s.frame_count)
+    s.translate(s.width // 2, s.height // 2)
+    s.circle(40, 0, 10)
+    s.pop()
+    s.circle(60, 0, 10)
+    s.pop()
+    s.circle(80, 0, 10)
+```
+
+![advancedexample](https://user-images.githubusercontent.com/88753590/236653135-d38838d1-518c-4b70-a664-ea121cf71315.gif)
+
+
+
+### EduDraw.scale(scale_x: float, scale_y: float) 
+
+Scales the drawing's axis by the desired multipliers
+Note: Is cumulative with other scalars.
+
+Parameters:
+
+scale_x: The multiplier to apply in the x axis
+scale_y: The multiplier to apply in the y axis
+
+Example:
+```
+ def draw():
+    s.background((255, 255, 255))
+    s.fill((200, 200, 0))
+
+    s.square(50, 50, 25)
+
+    s.scale(2, 0.5)
+
+    s.fill((0, 0, 200))
+    s.square(50, 50, 25)
+
+    s.reset_scaling()
+    s.scale(0.75, 1.25)
+
+    s.fill((255, 0, 0))
+    s.square(50, 50, 25)
+
+    s.reset_scaling()
+
+    s.fill((0, 255, 0))
+    s.square(75, 75, 25)
+```
+
+![scale](https://user-images.githubusercontent.com/88753590/236652949-f882daf2-fba5-4cd4-8e62-5d418b3fbfee.png)
+
+
+### EduDraw.translate(translate_x: int, translate_y: int)
+
+Changes the origin of the plane of drawing.
+Note: Is cumulative with other translations.
+
+Parameters:
+
+translate_x: The amount to translate in the x axis
+translate_y: The amount to translate in the y axis
+
+Example:
+```
+def draw():
+    s.translate(0, 0)
+    s.background((255, 255, 255))
+    s.fill((125, 125, 125))
+    s.square(50, 50, 50)
+
+    s.translate(-50, 50)
+    s.fill((200, 200, 0))
+    s.square(50, 50, 50)
+```
+
+![translate](https://user-images.githubusercontent.com/88753590/236652958-1b89304d-9cb0-4104-9806-82dc0c8e9f3c.png)
+
+
+### EduDraw.reset_transformations()
+
+Resets all transformations applied.
+
+### EduDraw.reset_scaling() 
+
+Resets all scaling transformations applied.
+
+### EduDraw.reset_translation() 
+
+Resets all translation transformations applied.
+
+### EduDraw.reset_rotation() 
+
+Resets all rotation transformations applied.
+
+### EduDraw.set_account_for_transformations(state: bool) 
+
+Changes wether `mouse_pos()` should yield the real or perceived position of the mouse.
+
+Parameters:
+
+state: The state to apply to this setting. `True` yields the perceived position, whereas `False` (the default) yields the real position.
+
+### EduDraw.set_controls(key_down=None, key_up=None, mouse_motion=None, mouse_button_up=None, mouse_button_down=None, mouse_wheel=None)
+
+Sets functions to be ran on each specific Pygame event. `None` means that nothing will occur on those events.
+Each function must have a parameter to receive a dictionary containing the data related to that event (such
+as which key was pressed, where the mouse is, etc.)
+
+Parameters:
+
+key_down: The function to be ran when a key is pressed down
+
+key_up: The function to be ran when a key is released
+
+mouse_motion: The function to be ran when the mouse is moved
+
+mouse_button_up: The function to be ran when a mouse button is released
+
+mouse_button_down: The function to be ran when a mouse button is pressed
+
+mouse_wheel: The function to be ran when the mouse wheel is scrolled
+        
+Example:
+
+```
+s = EduDraw(400, 400)
+
+bg_color = (200, 200, 200)
+text = ''
+
+def setup():
+    s.set_controls(mouse_button_down=do_stuff_on_click)
+
+def draw():
+    s.background(bg_color)
+    s.text(text, s.width // 2, s.height // 2)
+
+count = 0
+def do_stuff_on_click(data: dict):
+    global count, bg_color, text
+    if count % 2 == 0:
+        bg_color = (0, 0, 0)
+        text = ''
+    else:
+        bg_color = (255, 255, 255)
+        text = 'Clicked!'
+    count += 1
+
+s.start(setup, draw, 'Hello')
+```
+
+Example 2:
+
+```
+my_word = ''
+
+def setup():
+    s.set_controls(key_down=get_char)
+    s.change_default_font('times new roman', 30, italic=True)
+
+def draw():
+    s.fill((255, 255, 255))
+    s.background((0, 0, 0))
+    s.rect_mode("CENTER")
+    s.text(my_word, s.width // 2, s.height // 2)
+
+def get_char(data: dict):
+    global my_word
+    print(data)
+    unicode = data['unicode']
+    if unicode == '\x08':
+        my_word = my_word[:-1]
+    else:
+        my_word += data['unicode']
+```
+
+![keyexample](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/ddb1a44e-77a0-46f3-bf10-fff2d76989ec)
+
+
+### EduDraw.toggle_antialising()
+
+Toggles antialiasing on or off. It's off by default.
+
+Note: Antialiasing needs more processing, especially when the number of shapes and their complexity is higher. Also, antialised shapes do not take
+into account the stroke weight of the lines, and all lines are drawn with the weight of 1px.
+
+## Drawing methods
+
+These methods draw onto the canvas.
+
+### EduDraw.point(x: int, y: int)
+
+Draws a point at coordinates (x,y)
+
+Parameters:
+
+x, y: The x,y coordinates to draw the point onto.
+
+### EduDraw.text(string: str, x: int, y: int)
+
+Writes a string of text onto the screen.
+
+Parameters:
+
+string: The text to be written
+
+x, y: The coordinates of the top-left corner of the text if rect_mode is 'TOP_LEFT' or the middle of the text is rect_mode is 'CENTER'.
+
+
+### EduDraw.background(color: tuple)
+
+Sets a new background color and clears the canvas to it.
+
+Parameters:
+
+color: A tuple containing the (R, G, B) values of the desired color.
+
+### EduDraw.circle(x: int, y: int, radius: int)
+
+Draws a circle onto the screen.
+
+Parameters:
+
+x, y: The coordinates of the top-left part of the rectangle that contains the circle if circle_mode is 'TOP_LEFT', or the center of the circle if circle_mode is 'CENTER'.
+
+r: The radius of the circle.
+
+### EduDraw.ellipse(x: int, y: int, width: int, height: int)
+
+Draws an ellipse onto the screen.
+
+Parameters:
+
+x, y: The coordinates of the top-left part of the rectange that contains the ellipse if circle_mode is 'TOP_LEFT', or the center of the ellipse if circle_mode is 'CENTER'.
+
+w, h: The width and height of the rectangle that contains the ellipse.
+
+Example:
+```
+def draw():
+    s.background((200, 200, 200))
+
+    s.stroke_weight(3)
+    s.circle_mode('TOP_LEFT')
+
+    s.fill((100, 100, 100))
+    s.stroke((0, 0, 255))
+    s.ellipse(62, 40, 45, 70)
+
+    s.no_fill()
+    s.stroke((255, 0, 0))
+    s.ellipse(50, 50, 70, 30)
+```
+
+![ellipse](https://user-images.githubusercontent.com/88753590/233815202-95fc61d6-b328-4783-85ec-e5f7df4b153a.png)
+
+
+### EduDraw.line(x1: int, y1: int, x2: int, y2: int)
+
+Draws a line between two points.
+
+Parameters:
+
+x1, y1: The coordinates of the first point.
+
+x2, y2: The coordinates of the second point.
+
+Example:
+```
+def draw():
+    s.background((200, 200, 200))
+    s.stroke_weight(3)
+
+    s.line(0, 0, s.width, s.height)
+    s.stroke((0, 0, 255))
+    s.line(0, s.height // 2, s.width, s.height // 2)
+    s.stroke((255, 0, 0))
+    s.line(200, 300, 400, 250)
+```
+
+![line](https://user-images.githubusercontent.com/88753590/233815204-d355aed5-f9e0-42f3-88b2-90feaf1bfe11.png)
+
+
+### EduDraw.rect(x: int, y: int, width: int, height: int)
+
+Draws a rectangle onto the screen.
+
+Parameters:
+
+x, y: The coordinates of the top-left corner of the rectangle if rect_mode is 'TOP_LEFT', or the center of the rectangle if rect_mode is 'CENTER'.
+
+width, height: The width and height of the rectangle.
+
+Example:
+```
+def draw():
+    s.background((200, 200, 200))
+    s.stroke_weight(3)
+
+    x = 50
+    y = 60
+
+    dx = 5
+    dy = 5
+
+    s.no_fill()
+
+    s.rect(x, y, 50, 90)
+
+    s.stroke((255, 0, 0))
+    s.rect(y, x, 90, 50)
+
+    s.stroke((0, 0, 255))
+    s.rect(x + dx, y + dy, 50 - dx * 2, 90 - dy * 2)
+```
+
+![rect](https://user-images.githubusercontent.com/88753590/233815207-f7f8732b-88ae-4f17-92b7-16006b05237a.png)
+
+
+### EduDraw.square(x: int, y: int, side_size: int)
+
+Draws a square onto the screen.
+
+Parameters:
+
+x, y: The coordinates of the top-left corner of the square if rect_mode is 'TOP_LEFT', or the center of the square if rect_mode is 'CENTER'.
+
+side_size: The size of the sides of the square.
+
+Example:
+```
+def draw():
+    s.background((255, 255, 255))
+
+    s.no_stroke()
+    s.fill((0, 0, 0))
+
+    for i in range(0, s.width, 25):
+        for j in range(0, s.height, 25):
+            if ((i + j) % 2) == 0:
+                s.square(i, j, 25)
+```
+
+![square](https://user-images.githubusercontent.com/88753590/233815209-c043af52-74ed-4b87-939f-39024043e458.png)
+
+
+### EduDraw.triangle(x1: int, y1: int, x2: int, y2: int, x3: int, y3: int)
+
+Draws a triangle onto the screen.
+
+Parameters:
+
+x1,y1: The coordinates of the first vertex of the triangle.
+
+x2,y2: The coordinates of the second vertex of the triangle.
+
+x3,y3: The coordinates of the third vertex of the triangle.
+
+Example:
+```
+def draw():
+    s.background((200, 200, 200))
+
+    s.fill((255, 255, 0))
+
+    s.triangle(40, 40, 120, 40, 80, 120)
+    s.triangle(120, 40, 200, 40, 160, 120)
+    s.triangle(80, 120, 160, 120, 120, 200)
+```
+
+![triangle](https://user-images.githubusercontent.com/88753590/233815214-5f44f6b7-4d0a-41f8-88f8-3b384e1d117f.png)
+
+
+
+### EduDraw.polygon(points: list)
+
+Draws any polygon onto the screen.
+
+Parameters:
+
+points: An array containing tuples with all of the vertices of the polygon.
+
+Example:
+```
+def draw():
+    s.background((200, 200, 200))
+
+    s.fill((100, 255, 255))
+    points = [
+        (50, 50),
+        (100, 50),
+        (120, 100),
+        (75, 135),
+        (30, 100)
+    ]
+
+    s.polygon(points)
+```
+
+![polygon](https://user-images.githubusercontent.com/88753590/233815221-2da1f919-571f-40a2-ad96-cb4e4084875b.png)
+
+
+---
+
+### EduDraw.image(img: pygame.surface.Surface, x: int, y: int, width: int = None, height: int = None, force_transparency: bool = False):
+    
+Displays an image onto the screen on the (x,y) position. If specified a width or height, the image will be resized to those sizes, otherwise, the image will be drawn to it's original size.
+    
+Parameters:
+
+img: The image to be drawn onto the canvas
+    
+x, y: The position to draw the image
+    
+(Optional) width, height: The sizes to set the image to
+
+(Optional) force_transparency: Whether or not force transparency onto the image. See more details below:
+
+```
+my_image = pygame.image.load('testimage.jpeg')
+
+def setup():
+    pass
+
+def draw():
+    s.fill((255, 255, 255))
+    s.background((0, 0, 0))
+    s.rect_mode("CENTER")
+    s.image(my_image, s.width // 2, s.height // 2, s.width // 2, s.height // 2)
+```
+
+![img](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/4dba8d75-7061-469d-a5fc-851908eb6d0f)
+
+Note that some images may not have transparency when transformed into `pygame.Surface` objects through the
+`pygame.image.load()` method. Should this be the case, like the one below, you can use the `force_transparency`
+parameter to force that.
+
+![example](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/c350c788-3cc4-491e-94f9-67c1a7aa8a78)
+
+
+### EduDraw.frame_rate(fps: int)
+
+Changes the framerate of the simulation. Must be called in ```setup()```.
+Note that in the Python version the simulation does not run as fast as the C# one, to run the simulation as fast as possible set the EduDraw.deltatime to zero.
+
+Parameters:
+
+int frames: The number of FPS to set the simulation to.
+
+
+### EduDraw.save(filename: str)
+
+Saves the current frame as an image file.
+If filename is empty, the name will be the frame count of when the photo was saved.
+
+
+### EduDraw.quit()
+
+Quits the simulation.
+
+### Null mode
+
+Null mode is a mode in which you can run an instance of a simulation without having it running directly onto the canvas. You can do this for many reasons, including using EduDraw in a different context or application, creating multiple drawings inside of one another, among other things.
+
+To initialize an EduDraw instance in null mode, you can use the optional parameter for it in the `start()` method.
+
+Example of null mode:
+
+```
+s = edudraw.EduDraw(500, 500) # Main instance
+d = edudraw.EduDraw(250, 250, True) # Null mode ('inner') instance
+
+def setup():
+  {...}
+
+def draw():
+  {...}
+
+def inner_setup():
+  {...}
+
+def inner_draw():
+  {...}
+  
+s.start(setup, draw, "My window title")
+d.start(inner_setup, inner_draw, "This text is not shown")
+```
+
+In order to be able to visualize instance of null mode, you'll have to retrieve the images (`pygame.surface.Surface`) and use those in your drawing or any other desired output (whether that be an icon, a display, a file, etc.).
+
+You can retrieve the images with the `EduDraw.screen` variable. With that Surface object retrieved, you can use it wherever it's necessary, and you have much more flexibility for what to do with it.
+
+A good example of this is to run two instances of EduDraw, one normal and one null, and use the retrieved images from the null instance as an argument for EduDraw.image(), essentially creating a drawing inside of a drawing, like the example below:
+
+```
+s = edudraw.EduDraw(200, 200)
+d = edudraw.EduDraw(100, 100, True)
+
+position = [d.width/2, d.height//2]
+velocity = [3, 4]
+
+# We don't need to setup anything in this case
+def setup():
+    pass
+
+def inner_drawing():
+    global position, velocity
+    if position[0] < 0 or position[0] > d.width:
+        velocity[0] *= -1
+
+    if position[1] < 0 or position[1] > d.height:
+        velocity[1] *= -1
+
+    position[0] += velocity[0]
+    position[1] += velocity[1]
+
+    d.fill((255, 0, 0))
+    d.stroke((0, 0, 255))
+    d.circle(position[0], position[1], 5)
+
+def draw():
+    s.background((200, 200, 200))
+    s.rotate(s.frame_count)
+    s.rect_mode("CENTER")
+    s.translate(s.width // 2, s.height // 2)
+    s.image(d.screen, 0, 0)
+    
+d.start(setup, inner_drawing, "This does not appear")
+s.start(setup, draw, "My drawing :D")
+```
+
+![nullmode](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/5026c565-f081-49cf-8bfd-55fe487bada6)
+
```

