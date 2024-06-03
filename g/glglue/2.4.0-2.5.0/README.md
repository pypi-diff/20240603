# Comparing `tmp/glglue-2.4.0.tar.gz` & `tmp/glglue-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glglue-2.4.0.tar", last modified: Mon May 13 04:07:41 2024, max compression
+gzip compressed data, was "glglue-2.5.0.tar", last modified: Mon Jun  3 07:08:56 2024, max compression
```

## Comparing `glglue-2.4.0.tar` & `glglue-2.5.0.tar`

### file list

```diff
@@ -1,129 +1,140 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:41.309191 glglue-2.4.0/
--rw-rw-rw-   0        0        0      321 2024-05-07 04:24:13.000000 glglue-2.4.0/.clang-format
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.010920 glglue-2.4.0/.github/
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.120323 glglue-2.4.0/.github/workflows/
--rw-rw-rw-   0        0        0     1321 2024-05-07 09:21:29.000000 glglue-2.4.0/.github/workflows/docusaurus.yml
--rw-rw-rw-   0        0        0       86 2024-05-08 10:16:01.000000 glglue-2.4.0/.gitignore
--rw-rw-rw-   0        0        0       75 2024-05-07 04:24:13.000000 glglue-2.4.0/.remarkrc
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.182803 glglue-2.4.0/.vscode/
--rw-rw-rw-   0        0        0     3074 2024-05-13 04:07:01.000000 glglue-2.4.0/.vscode/launch.json
--rw-rw-rw-   0        0        0      602 2024-05-07 04:24:13.000000 glglue-2.4.0/.vscode/settings.json
--rw-rw-rw-   0        0        0      555 2024-05-07 04:24:13.000000 glglue-2.4.0/.vscode/tasks.json
--rw-rw-rw-   0        0        0     1065 2024-05-07 04:24:13.000000 glglue-2.4.0/LICENSE
--rw-rw-rw-   0        0        0     1884 2024-05-13 04:07:41.309191 glglue-2.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1259 2024-05-07 09:19:11.000000 glglue-2.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.323957 glglue-2.4.0/docs/
--rw-rw-rw-   0        0        0      233 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/.gitignore
--rw-rw-rw-   0        0        0      768 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/README.md
--rw-rw-rw-   0        0        0       89 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/babel.config.js
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.417819 glglue-2.4.0/docs/blog/
--rw-rw-rw-   0        0        0      389 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/blog/2019-05-28-first-blog-post.md
--rw-rw-rw-   0        0        0     3116 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/blog/2019-05-29-long-blog-post.md
--rw-rw-rw-   0        0        0      439 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/blog/2021-08-01-mdx-blog-post.mdx
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.417819 glglue-2.4.0/docs/blog/2021-08-26-welcome/
--rw-rw-rw-   0        0        0    96122 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg
--rw-rw-rw-   0        0        0      783 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/blog/2021-08-26-welcome/index.md
--rw-rw-rw-   0        0        0      447 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/blog/authors.yml
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.433348 glglue-2.4.0/docs/docs/
--rw-rw-rw-   0        0        0      875 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/docs/index.md
--rw-rw-rw-   0        0        0     3760 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/docusaurus.config.ts
--rw-rw-rw-   0        0        0   570118 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/package-lock.json
--rw-rw-rw-   0        0        0     1150 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/package.json
--rw-rw-rw-   0        0        0      645 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/sidebars.ts
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.026454 glglue-2.4.0/docs/src/
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.010920 glglue-2.4.0/docs/src/components/
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.449008 glglue-2.4.0/docs/src/components/HomepageFeatures/
--rw-rw-rw-   0        0        0     1889 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/src/components/HomepageFeatures/index.tsx
--rw-rw-rw-   0        0        0      138 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/src/components/HomepageFeatures/styles.module.css
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.464702 glglue-2.4.0/docs/src/css/
--rw-rw-rw-   0        0        0     1042 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/src/css/custom.css
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.495942 glglue-2.4.0/docs/src/pages/
--rw-rw-rw-   0        0        0      365 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/src/pages/index.module.css
--rw-rw-rw-   0        0        0     1343 2024-05-07 09:25:04.000000 glglue-2.4.0/docs/src/pages/index.tsx
--rw-rw-rw-   0        0        0      118 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/src/pages/markdown-page.md
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.495942 glglue-2.4.0/docs/static/
--rw-rw-rw-   0        0        0        0 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/static/.nojekyll
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.558453 glglue-2.4.0/docs/static/img/
--rw-rw-rw-   0        0        0    55746 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/static/img/docusaurus-social-card.jpg
--rw-rw-rw-   0        0        0     5142 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/static/img/docusaurus.png
--rw-rw-rw-   0        0        0     3626 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/static/img/favicon.ico
--rw-rw-rw-   0        0        0     6438 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/static/img/logo.svg
--rw-rw-rw-   0        0        0    31486 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/static/img/undraw_docusaurus_mountain.svg
--rw-rw-rw-   0        0        0    36002 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/static/img/undraw_docusaurus_react.svg
--rw-rw-rw-   0        0        0    11887 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/static/img/undraw_docusaurus_tree.svg
--rw-rw-rw-   0        0        0      176 2024-05-07 09:19:11.000000 glglue-2.4.0/docs/tsconfig.json
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.026454 glglue-2.4.0/examples/
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.620945 glglue-2.4.0/examples/basic/
--rw-rw-rw-   0        0        0      533 2024-05-07 09:19:11.000000 glglue-2.4.0/examples/basic/freeglut_sample.py
--rw-rw-rw-   0        0        0      394 2024-05-07 09:19:11.000000 glglue-2.4.0/examples/basic/glfw_sample.py
--rw-rw-rw-   0        0        0      632 2024-05-07 04:24:13.000000 glglue-2.4.0/examples/basic/gtk3_sample.py
--rw-rw-rw-   0        0        0      776 2024-05-07 04:24:13.000000 glglue-2.4.0/examples/basic/gtk4_sample.py
--rw-rw-rw-   0        0        0      391 2024-05-07 09:19:11.000000 glglue-2.4.0/examples/basic/pysdl2_sample.py
--rw-rw-rw-   0        0        0      591 2024-05-07 09:19:11.000000 glglue-2.4.0/examples/basic/pyside6_sample.py
--rw-rw-rw-   0        0        0      657 2024-05-07 04:24:13.000000 glglue-2.4.0/examples/basic/wgl_sample.py
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.636579 glglue-2.4.0/examples/gui/
--rw-rw-rw-   0        0        0     2630 2024-05-08 11:56:08.000000 glglue-2.4.0/examples/gui/pyside6_gui.py
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.652196 glglue-2.4.0/examples/scene/
--rw-rw-rw-   0        0        0     3832 2024-05-13 04:07:01.000000 glglue-2.4.0/examples/scene/pyside6_texture.py
--rw-rw-rw-   0        0        0      816 2024-05-07 09:19:11.000000 glglue-2.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 04:07:41.309191 glglue-2.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.026454 glglue-2.4.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:40.933448 glglue-2.4.0/src/glglue/
--rw-rw-rw-   0        0        0       67 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/__init__.py
--rw-rw-rw-   0        0        0      427 2024-05-13 04:07:39.000000 glglue-2.4.0/src/glglue/_version.py
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:41.011580 glglue-2.4.0/src/glglue/assets/
--rw-rw-rw-   0        0        0   471984 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/assets/Utah_teapot_(solid).stl
--rw-rw-rw-   0        0        0      103 2024-05-10 10:42:28.000000 glglue-2.4.0/src/glglue/assets/line.frag
--rw-rw-rw-   0        0        0      261 2024-05-10 10:43:01.000000 glglue-2.4.0/src/glglue/assets/line.vert
--rw-rw-rw-   0        0        0      103 2024-05-10 10:39:30.000000 glglue-2.4.0/src/glglue/assets/mesh.frag
--rw-rw-rw-   0        0        0      462 2024-05-10 10:40:21.000000 glglue-2.4.0/src/glglue/assets/mesh.vert
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:41.042821 glglue-2.4.0/src/glglue/camera/
--rw-rw-rw-   0        0        0      279 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/camera/__init__.py
--rw-rw-rw-   0        0        0     7991 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/camera/camera.py
--rw-rw-rw-   0        0        0      891 2024-05-08 09:14:56.000000 glglue-2.4.0/src/glglue/camera/mouse_camera.py
--rw-rw-rw-   0        0        0     4730 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/camera/mouse_event.py
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:41.168456 glglue-2.4.0/src/glglue/drawable/
--rw-rw-rw-   0        0        0       55 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/drawable/__init__.py
--rw-rw-rw-   0        0        0     1097 2024-05-08 13:11:26.000000 glglue-2.4.0/src/glglue/drawable/axes.py
--rw-rw-rw-   0        0        0     1816 2024-05-13 04:07:01.000000 glglue-2.4.0/src/glglue/drawable/cube.py
--rw-rw-rw-   0        0        0     1374 2024-05-10 10:51:55.000000 glglue-2.4.0/src/glglue/drawable/drawable.py
--rw-rw-rw-   0        0        0      892 2024-05-08 13:10:38.000000 glglue-2.4.0/src/glglue/drawable/grid.py
--rw-rw-rw-   0        0        0     1045 2024-05-08 12:56:37.000000 glglue-2.4.0/src/glglue/drawable/line_builder.py
--rw-rw-rw-   0        0        0     1335 2024-05-13 04:07:01.000000 glglue-2.4.0/src/glglue/drawable/mesh_builder.py
--rw-rw-rw-   0        0        0     2949 2024-05-13 04:07:01.000000 glglue-2.4.0/src/glglue/drawable/teapot.py
--rw-rw-rw-   0        0        0      509 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/frame_input.py
--rw-rw-rw-   0        0        0     5210 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/glfw.py
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:41.246630 glglue-2.4.0/src/glglue/glo/
--rw-rw-rw-   0        0        0      470 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/glo/__init__.py
--rw-rw-rw-   0        0        0     2461 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/glo/fbo.py
--rw-rw-rw-   0        0        0     6071 2024-05-13 04:07:01.000000 glglue-2.4.0/src/glglue/glo/shader.py
--rw-rw-rw-   0        0        0     2263 2024-05-13 04:07:01.000000 glglue-2.4.0/src/glglue/glo/texture.py
--rw-rw-rw-   0        0        0     1707 2024-05-13 04:07:01.000000 glglue-2.4.0/src/glglue/glo/vao.py
--rw-rw-rw-   0        0        0     3228 2024-05-13 04:07:01.000000 glglue-2.4.0/src/glglue/glo/vbo.py
--rw-rw-rw-   0        0        0     3755 2024-05-08 09:43:52.000000 glglue-2.4.0/src/glglue/glo/vertex_layout.py
--rw-rw-rw-   0        0        0     3144 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/glut.py
--rw-rw-rw-   0        0        0     2659 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/gtk3.py
--rw-rw-rw-   0        0        0     3156 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/gtk4.py
--rw-rw-rw-   0        0        0     3625 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/pysdl2.py
--rw-rw-rw-   0        0        0     4672 2024-05-08 11:20:04.000000 glglue-2.4.0/src/glglue/pyside6.py
--rw-rw-rw-   0        0        0     2443 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/qgl4.py
--rw-rw-rw-   0        0        0     2452 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/qgl5.py
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:41.262326 glglue-2.4.0/src/glglue/scene/
--rw-rw-rw-   0        0        0     2999 2024-05-13 04:07:01.000000 glglue-2.4.0/src/glglue/scene/sample.py
--rw-rw-rw-   0        0        0      962 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/sdl.py
--rw-rw-rw-   0        0        0     2885 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/togl.py
--rw-rw-rw-   0        0        0     1475 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/util.py
--rw-rw-rw-   0        0        0    21812 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/wgl.py
--rw-rw-rw-   0        0        0   122098 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/win32con.py
--rw-rw-rw-   0        0        0      529 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/windowconfig.py
--rw-rw-rw-   0        0        0     3190 2024-05-07 09:19:11.000000 glglue-2.4.0/src/glglue/wxglcanvas.py
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:41.309191 glglue-2.4.0/src/glglue.egg-info/
--rw-rw-rw-   0        0        0     1884 2024-05-13 04:07:39.000000 glglue-2.4.0/src/glglue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2687 2024-05-13 04:07:40.000000 glglue-2.4.0/src/glglue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 04:07:39.000000 glglue-2.4.0/src/glglue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-13 04:07:39.000000 glglue-2.4.0/src/glglue.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-13 04:07:39.000000 glglue-2.4.0/src/glglue.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 04:07:41.309191 glglue-2.4.0/tests/
--rw-rw-rw-   0        0        0     1410 2024-05-07 04:24:13.000000 glglue-2.4.0/tests/test_numpy.py
--rw-rw-rw-   0        0        0      287 2024-05-07 09:19:11.000000 glglue-2.4.0/tests/test_py.py
--rw-rw-rw-   0        0        0      221 2024-05-07 09:19:11.000000 glglue-2.4.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.337304 glglue-2.5.0/
+-rw-rw-rw-   0        0        0      321 2024-05-07 04:24:13.000000 glglue-2.5.0/.clang-format
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.247666 glglue-2.5.0/.github/
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.256665 glglue-2.5.0/.github/workflows/
+-rw-rw-rw-   0        0        0     1321 2024-05-07 09:21:29.000000 glglue-2.5.0/.github/workflows/docusaurus.yml
+-rw-rw-rw-   0        0        0       86 2024-05-08 10:16:01.000000 glglue-2.5.0/.gitignore
+-rw-rw-rw-   0        0        0       75 2024-05-07 04:24:13.000000 glglue-2.5.0/.remarkrc
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.258387 glglue-2.5.0/.vscode/
+-rw-rw-rw-   0        0        0     4340 2024-05-30 12:46:16.000000 glglue-2.5.0/.vscode/launch.json
+-rw-rw-rw-   0        0        0      602 2024-05-07 04:24:13.000000 glglue-2.5.0/.vscode/settings.json
+-rw-rw-rw-   0        0        0      555 2024-05-07 04:24:13.000000 glglue-2.5.0/.vscode/tasks.json
+-rw-rw-rw-   0        0        0     1065 2024-05-07 04:24:13.000000 glglue-2.5.0/LICENSE
+-rw-rw-rw-   0        0        0     2052 2024-06-03 07:08:56.337304 glglue-2.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1418 2024-06-03 07:06:29.000000 glglue-2.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.262743 glglue-2.5.0/docs/
+-rw-rw-rw-   0        0        0      233 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/.gitignore
+-rw-rw-rw-   0        0        0      768 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/README.md
+-rw-rw-rw-   0        0        0       89 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/babel.config.js
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.265743 glglue-2.5.0/docs/blog/
+-rw-rw-rw-   0        0        0      389 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/blog/2019-05-28-first-blog-post.md
+-rw-rw-rw-   0        0        0     3116 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/blog/2019-05-29-long-blog-post.md
+-rw-rw-rw-   0        0        0      439 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/blog/2021-08-01-mdx-blog-post.mdx
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.266743 glglue-2.5.0/docs/blog/2021-08-26-welcome/
+-rw-rw-rw-   0        0        0    96122 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg
+-rw-rw-rw-   0        0        0      783 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/blog/2021-08-26-welcome/index.md
+-rw-rw-rw-   0        0        0      447 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/blog/authors.yml
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.266743 glglue-2.5.0/docs/docs/
+-rw-rw-rw-   0        0        0      875 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/docs/index.md
+-rw-rw-rw-   0        0        0     3760 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/docusaurus.config.ts
+-rw-rw-rw-   0        0        0   570118 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/package-lock.json
+-rw-rw-rw-   0        0        0     1150 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/package.json
+-rw-rw-rw-   0        0        0      645 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/sidebars.ts
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.250665 glglue-2.5.0/docs/src/
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.249665 glglue-2.5.0/docs/src/components/
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.268743 glglue-2.5.0/docs/src/components/HomepageFeatures/
+-rw-rw-rw-   0        0        0     1889 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/src/components/HomepageFeatures/index.tsx
+-rw-rw-rw-   0        0        0      138 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/src/components/HomepageFeatures/styles.module.css
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.268743 glglue-2.5.0/docs/src/css/
+-rw-rw-rw-   0        0        0     1042 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/src/css/custom.css
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.270743 glglue-2.5.0/docs/src/pages/
+-rw-rw-rw-   0        0        0      365 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/src/pages/index.module.css
+-rw-rw-rw-   0        0        0     1343 2024-05-07 09:25:04.000000 glglue-2.5.0/docs/src/pages/index.tsx
+-rw-rw-rw-   0        0        0      118 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/src/pages/markdown-page.md
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.270743 glglue-2.5.0/docs/static/
+-rw-rw-rw-   0        0        0        0 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/static/.nojekyll
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.274781 glglue-2.5.0/docs/static/img/
+-rw-rw-rw-   0        0        0    55746 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/static/img/docusaurus-social-card.jpg
+-rw-rw-rw-   0        0        0     5142 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/static/img/docusaurus.png
+-rw-rw-rw-   0        0        0     3626 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/static/img/favicon.ico
+-rw-rw-rw-   0        0        0     6438 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/static/img/logo.svg
+-rw-rw-rw-   0        0        0    31486 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/static/img/undraw_docusaurus_mountain.svg
+-rw-rw-rw-   0        0        0    36002 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/static/img/undraw_docusaurus_react.svg
+-rw-rw-rw-   0        0        0    11887 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/static/img/undraw_docusaurus_tree.svg
+-rw-rw-rw-   0        0        0      176 2024-05-07 09:19:11.000000 glglue-2.5.0/docs/tsconfig.json
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.251665 glglue-2.5.0/examples/
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.280212 glglue-2.5.0/examples/basic/
+-rw-rw-rw-   0        0        0      533 2024-05-07 09:19:11.000000 glglue-2.5.0/examples/basic/freeglut_sample.py
+-rw-rw-rw-   0        0        0      394 2024-05-07 09:19:11.000000 glglue-2.5.0/examples/basic/glfw_sample.py
+-rw-rw-rw-   0        0        0      632 2024-05-07 04:24:13.000000 glglue-2.5.0/examples/basic/gtk3_sample.py
+-rw-rw-rw-   0        0        0      878 2024-05-27 07:34:56.000000 glglue-2.5.0/examples/basic/gtk4_sample.py
+-rw-rw-rw-   0        0        0     1388 2024-05-30 12:48:24.000000 glglue-2.5.0/examples/basic/pyopengltk_sample.py
+-rw-rw-rw-   0        0        0      391 2024-05-07 09:19:11.000000 glglue-2.5.0/examples/basic/pysdl2_sample.py
+-rw-rw-rw-   0        0        0      591 2024-05-07 09:19:11.000000 glglue-2.5.0/examples/basic/pyside6_sample.py
+-rw-rw-rw-   0        0        0      657 2024-05-07 04:24:13.000000 glglue-2.5.0/examples/basic/wgl_sample.py
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.281212 glglue-2.5.0/examples/gui/
+-rw-rw-rw-   0        0        0     1393 2024-05-30 11:21:47.000000 glglue-2.5.0/examples/gui/pyside6_gizmo.py
+-rw-rw-rw-   0        0        0     2630 2024-05-08 11:56:08.000000 glglue-2.5.0/examples/gui/pyside6_gui.py
+-rw-rw-rw-   0        0        0     4512 2024-05-30 11:21:47.000000 glglue-2.5.0/examples/gui/scene.py
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.281212 glglue-2.5.0/examples/scene/
+-rw-rw-rw-   0        0        0     3832 2024-05-13 04:07:01.000000 glglue-2.5.0/examples/scene/pyside6_texture.py
+-rw-rw-rw-   0        0        0      816 2024-05-07 09:19:11.000000 glglue-2.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-03 07:08:56.337304 glglue-2.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.252665 glglue-2.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.308140 glglue-2.5.0/src/glglue/
+-rw-rw-rw-   0        0        0       67 2024-05-07 09:19:11.000000 glglue-2.5.0/src/glglue/__init__.py
+-rw-rw-rw-   0        0        0      427 2024-06-03 07:08:56.000000 glglue-2.5.0/src/glglue/_version.py
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.323390 glglue-2.5.0/src/glglue/assets/
+-rw-rw-rw-   0        0        0   471984 2024-05-07 09:19:11.000000 glglue-2.5.0/src/glglue/assets/Utah_teapot_(solid).stl
+-rw-rw-rw-   0        0        0      103 2024-05-10 10:42:28.000000 glglue-2.5.0/src/glglue/assets/line.frag
+-rw-rw-rw-   0        0        0      261 2024-05-10 10:43:01.000000 glglue-2.5.0/src/glglue/assets/line.vert
+-rw-rw-rw-   0        0        0      313 2024-05-27 07:34:56.000000 glglue-2.5.0/src/glglue/assets/mesh.frag
+-rw-rw-rw-   0        0        0      492 2024-05-27 07:34:56.000000 glglue-2.5.0/src/glglue/assets/mesh.vert
+-rw-rw-rw-   0        0        0      103 2024-05-27 07:34:56.000000 glglue-2.5.0/src/glglue/assets/vertex_color.frag
+-rw-rw-rw-   0        0        0      462 2024-05-27 07:34:56.000000 glglue-2.5.0/src/glglue/assets/vertex_color.vert
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.325287 glglue-2.5.0/src/glglue/camera/
+-rw-rw-rw-   0        0        0      279 2024-05-07 09:19:11.000000 glglue-2.5.0/src/glglue/camera/__init__.py
+-rw-rw-rw-   0        0        0     8033 2024-05-27 07:34:56.000000 glglue-2.5.0/src/glglue/camera/camera.py
+-rw-rw-rw-   0        0        0      891 2024-05-08 09:14:56.000000 glglue-2.5.0/src/glglue/camera/mouse_camera.py
+-rw-rw-rw-   0        0        0     4928 2024-05-30 12:32:23.000000 glglue-2.5.0/src/glglue/camera/mouse_event.py
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.329306 glglue-2.5.0/src/glglue/drawable/
+-rw-rw-rw-   0        0        0      169 2024-05-30 11:21:47.000000 glglue-2.5.0/src/glglue/drawable/__init__.py
+-rw-rw-rw-   0        0        0     1097 2024-05-08 13:11:26.000000 glglue-2.5.0/src/glglue/drawable/axes.py
+-rw-rw-rw-   0        0        0     1816 2024-05-13 04:07:01.000000 glglue-2.5.0/src/glglue/drawable/cube.py
+-rw-rw-rw-   0        0        0     1374 2024-05-10 10:51:55.000000 glglue-2.5.0/src/glglue/drawable/drawable.py
+-rw-rw-rw-   0        0        0      892 2024-05-08 13:10:38.000000 glglue-2.5.0/src/glglue/drawable/grid.py
+-rw-rw-rw-   0        0        0     1045 2024-05-08 12:56:37.000000 glglue-2.5.0/src/glglue/drawable/line_builder.py
+-rw-rw-rw-   0        0        0     1335 2024-05-13 04:07:01.000000 glglue-2.5.0/src/glglue/drawable/mesh_builder.py
+-rw-rw-rw-   0        0        0     2949 2024-05-13 04:07:01.000000 glglue-2.5.0/src/glglue/drawable/teapot.py
+-rw-rw-rw-   0        0        0      509 2024-05-07 09:19:11.000000 glglue-2.5.0/src/glglue/frame_input.py
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.330309 glglue-2.5.0/src/glglue/gl_stubgen/
+-rw-rw-rw-   0        0        0     1411 2024-05-27 07:34:56.000000 glglue-2.5.0/src/glglue/gl_stubgen/__main__.py
+-rw-rw-rw-   0        0        0     5210 2024-05-07 09:19:11.000000 glglue-2.5.0/src/glglue/glfw.py
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.333306 glglue-2.5.0/src/glglue/glo/
+-rw-rw-rw-   0        0        0      470 2024-05-07 09:19:11.000000 glglue-2.5.0/src/glglue/glo/__init__.py
+-rw-rw-rw-   0        0        0     2461 2024-05-07 09:19:11.000000 glglue-2.5.0/src/glglue/glo/fbo.py
+-rw-rw-rw-   0        0        0     6071 2024-05-13 04:07:01.000000 glglue-2.5.0/src/glglue/glo/shader.py
+-rw-rw-rw-   0        0        0     2263 2024-05-13 04:07:01.000000 glglue-2.5.0/src/glglue/glo/texture.py
+-rw-rw-rw-   0        0        0     1642 2024-05-27 07:34:56.000000 glglue-2.5.0/src/glglue/glo/vao.py
+-rw-rw-rw-   0        0        0     3341 2024-05-27 07:34:56.000000 glglue-2.5.0/src/glglue/glo/vbo.py
+-rw-rw-rw-   0        0        0     3755 2024-05-08 09:43:52.000000 glglue-2.5.0/src/glglue/glo/vertex_layout.py
+-rw-rw-rw-   0        0        0     3144 2024-05-07 09:19:11.000000 glglue-2.5.0/src/glglue/glut.py
+-rw-rw-rw-   0        0        0     2659 2024-05-07 09:19:11.000000 glglue-2.5.0/src/glglue/gtk3.py
+-rw-rw-rw-   0        0        0     3156 2024-05-07 09:19:11.000000 glglue-2.5.0/src/glglue/gtk4.py
+-rw-rw-rw-   0        0        0     3625 2024-05-07 09:19:11.000000 glglue-2.5.0/src/glglue/pysdl2.py
+-rw-rw-rw-   0        0        0     4672 2024-05-08 11:20:04.000000 glglue-2.5.0/src/glglue/pyside6.py
+-rw-rw-rw-   0        0        0     2443 2024-05-07 09:19:11.000000 glglue-2.5.0/src/glglue/qgl4.py
+-rw-rw-rw-   0        0        0     2452 2024-05-07 09:19:11.000000 glglue-2.5.0/src/glglue/qgl5.py
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.333306 glglue-2.5.0/src/glglue/scene/
+-rw-rw-rw-   0        0        0     3007 2024-05-27 07:34:56.000000 glglue-2.5.0/src/glglue/scene/sample.py
+-rw-rw-rw-   0        0        0      962 2024-05-07 09:19:11.000000 glglue-2.5.0/src/glglue/sdl.py
+-rw-rw-rw-   0        0        0     5689 2024-05-31 04:12:47.000000 glglue-2.5.0/src/glglue/tk_frame.py
+-rw-rw-rw-   0        0        0     2885 2024-05-07 09:19:11.000000 glglue-2.5.0/src/glglue/togl.py
+-rw-rw-rw-   0        0        0     1475 2024-05-07 09:19:11.000000 glglue-2.5.0/src/glglue/util.py
+-rw-rw-rw-   0        0        0    21812 2024-05-07 09:19:11.000000 glglue-2.5.0/src/glglue/wgl.py
+-rw-rw-rw-   0        0        0   122098 2024-05-07 09:19:11.000000 glglue-2.5.0/src/glglue/win32con.py
+-rw-rw-rw-   0        0        0      529 2024-05-07 09:19:11.000000 glglue-2.5.0/src/glglue/windowconfig.py
+-rw-rw-rw-   0        0        0     3190 2024-05-07 09:19:11.000000 glglue-2.5.0/src/glglue/wxglcanvas.py
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.336304 glglue-2.5.0/src/glglue.egg-info/
+-rw-rw-rw-   0        0        0     2052 2024-06-03 07:08:56.000000 glglue-2.5.0/src/glglue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2926 2024-06-03 07:08:56.000000 glglue-2.5.0/src/glglue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 07:08:56.000000 glglue-2.5.0/src/glglue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-06-03 07:08:56.000000 glglue-2.5.0/src/glglue.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-06-03 07:08:56.000000 glglue-2.5.0/src/glglue.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.335305 glglue-2.5.0/tests/
+-rw-rw-rw-   0        0        0     1410 2024-05-07 04:24:13.000000 glglue-2.5.0/tests/test_numpy.py
+-rw-rw-rw-   0        0        0      287 2024-05-07 09:19:11.000000 glglue-2.5.0/tests/test_py.py
+-rw-rw-rw-   0        0        0      221 2024-05-07 09:19:11.000000 glglue-2.5.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.253665 glglue-2.5.0/typings/
+drwxrwxrwx   0        0        0        0 2024-06-03 07:08:56.335305 glglue-2.5.0/typings/OpenGL/
+-rw-rw-rw-   0        0        0   140412 2024-05-27 07:34:56.000000 glglue-2.5.0/typings/OpenGL/GL.pyi
```

### Comparing `glglue-2.4.0/.github/workflows/docusaurus.yml` & `glglue-2.5.0/.github/workflows/docusaurus.yml`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/.vscode/settings.json` & `glglue-2.5.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/.vscode/tasks.json` & `glglue-2.5.0/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/LICENSE` & `glglue-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/PKG-INFO` & `glglue-2.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glglue
-Version: 2.4.0
+Version: 2.5.0
 Summary: The glue code which mediates between OpenGL and some GUI
 Author-email: ousttrue <ousttrue@gmail.com>
 Project-URL: HomePage, https://ousttrue.github.io/glglue/
 Project-URL: Repository, https://github.com/ousttrue/glglue/
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling
@@ -38,16 +38,25 @@
 
 ## Requirements
 
 - Python 3.11
 
 ## status
 
-| platform | status | comment                                  |
-| -------- | ------ | ---------------------------------------- |
-| glut     | ok     | windows11, PATH to freeglut64.vc.dll     |
-| glfw     | ok     | windows11, pip install glfw              |
-| gtk3     | ?      | require gtk3 self build                  |
-| gtk4     | ?      | require gtk4 self build                  |
-| sdl2     | ok     | windows11, pip install pysdl2 pysdl2-dll |
-| qt6      | ok     | windows11, pip install pyside6)          |
-| win32    | ok     | windows11                                |
+| platform   | status | comment                                  |
+| ---------- | ------ | ---------------------------------------- |
+| win32      | ok     | windows11                                |
+| glut       | ok     | windows11, PATH to freeglut64.vc.dll     |
+| glfw       | ok     | windows11, pip install glfw              |
+| gtk3       | ?      | require gtk3 self build                  |
+| gtk4       | ok     | require gtk4 self build                  |
+| sdl2       | ok     | windows11, pip install pysdl2 pysdl2-dll |
+| qt6        | ok     | windows11, pip install pyside6           |
+| pyopengltk | ok     | windows11, pip install pyopengltk        |
+
+## upload
+
+```sh
+rm -rf dist
+py -m build --sdist
+twine upload dist/*
+```
```

### Comparing `glglue-2.4.0/README.md` & `glglue-2.5.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -22,16 +22,25 @@
 
 ## Requirements
 
 - Python 3.11
 
 ## status
 
-| platform | status | comment                                  |
-| -------- | ------ | ---------------------------------------- |
-| glut     | ok     | windows11, PATH to freeglut64.vc.dll     |
-| glfw     | ok     | windows11, pip install glfw              |
-| gtk3     | ?      | require gtk3 self build                  |
-| gtk4     | ?      | require gtk4 self build                  |
-| sdl2     | ok     | windows11, pip install pysdl2 pysdl2-dll |
-| qt6      | ok     | windows11, pip install pyside6)          |
-| win32    | ok     | windows11                                |
+| platform   | status | comment                                  |
+| ---------- | ------ | ---------------------------------------- |
+| win32      | ok     | windows11                                |
+| glut       | ok     | windows11, PATH to freeglut64.vc.dll     |
+| glfw       | ok     | windows11, pip install glfw              |
+| gtk3       | ?      | require gtk3 self build                  |
+| gtk4       | ok     | require gtk4 self build                  |
+| sdl2       | ok     | windows11, pip install pysdl2 pysdl2-dll |
+| qt6        | ok     | windows11, pip install pyside6           |
+| pyopengltk | ok     | windows11, pip install pyopengltk        |
+
+## upload
+
+```sh
+rm -rf dist
+py -m build --sdist
+twine upload dist/*
+```
```

### Comparing `glglue-2.4.0/docs/README.md` & `glglue-2.5.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/docs/blog/2019-05-29-long-blog-post.md` & `glglue-2.5.0/docs/blog/2019-05-29-long-blog-post.md`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg` & `glglue-2.5.0/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/docs/blog/2021-08-26-welcome/index.md` & `glglue-2.5.0/docs/blog/2021-08-26-welcome/index.md`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/docs/docs/index.md` & `glglue-2.5.0/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/docs/docusaurus.config.ts` & `glglue-2.5.0/docs/docusaurus.config.ts`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/docs/package-lock.json` & `glglue-2.5.0/docs/package-lock.json`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/docs/package.json` & `glglue-2.5.0/docs/package.json`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/docs/sidebars.ts` & `glglue-2.5.0/docs/sidebars.ts`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/docs/src/components/HomepageFeatures/index.tsx` & `glglue-2.5.0/docs/src/components/HomepageFeatures/index.tsx`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/docs/src/css/custom.css` & `glglue-2.5.0/docs/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/docs/src/pages/index.tsx` & `glglue-2.5.0/docs/src/pages/index.tsx`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/docs/static/img/docusaurus-social-card.jpg` & `glglue-2.5.0/docs/static/img/docusaurus-social-card.jpg`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/docs/static/img/docusaurus.png` & `glglue-2.5.0/docs/static/img/docusaurus.png`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/docs/static/img/favicon.ico` & `glglue-2.5.0/docs/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/docs/static/img/logo.svg` & `glglue-2.5.0/docs/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/docs/static/img/undraw_docusaurus_mountain.svg` & `glglue-2.5.0/docs/static/img/undraw_docusaurus_mountain.svg`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/docs/static/img/undraw_docusaurus_react.svg` & `glglue-2.5.0/docs/static/img/undraw_docusaurus_react.svg`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/docs/static/img/undraw_docusaurus_tree.svg` & `glglue-2.5.0/docs/static/img/undraw_docusaurus_tree.svg`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/examples/basic/freeglut_sample.py` & `glglue-2.5.0/examples/basic/freeglut_sample.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/examples/basic/gtk3_sample.py` & `glglue-2.5.0/examples/basic/gtk3_sample.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/examples/basic/gtk4_sample.py` & `glglue-2.5.0/examples/basic/gtk4_sample.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-import gi
+import os
+import pathlib
 import traceback
 
+os.add_dll_directory(pathlib.Path(os.environ["USERPROFILE"]) / "gtk/bin")
+
+import gi
+
 gi.require_version("Gtk", "4.0")
 from gi.repository import Gtk
 
 
 class Window(Gtk.ApplicationWindow):
     def __init__(self, app):
         super().__init__(application=app)  # type: ignore
 
         from glglue.scene.sample import SampleScene
+
         self.scene = SampleScene()
 
         import glglue.gtk4
 
         self.glWidget = glglue.gtk4.GLArea(self.scene.render)
         self.set_child(self.glWidget)
```

### Comparing `glglue-2.4.0/examples/basic/pyside6_sample.py` & `glglue-2.5.0/examples/basic/pyside6_sample.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/examples/basic/wgl_sample.py` & `glglue-2.5.0/examples/basic/wgl_sample.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/examples/gui/pyside6_gui.py` & `glglue-2.5.0/examples/gui/pyside6_gui.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/examples/scene/pyside6_texture.py` & `glglue-2.5.0/examples/scene/pyside6_texture.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/pyproject.toml` & `glglue-2.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/assets/Utah_teapot_(solid).stl` & `glglue-2.5.0/src/glglue/assets/Utah_teapot_(solid).stl`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/camera/camera.py` & `glglue-2.5.0/src/glglue/camera/camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,16 @@
         self.matrix = glm.perspectiveRH(
             self.fov_y, self.aspect, self.z_near, self.z_far
         )
 
     def resize(self, w: int, h: int) -> bool:
         if self.width == w and self.height == h:
             return False
+        if h==0:
+            return False
         self.width = w
         self.height = h
         self.aspect = float(w) / h
         self.update_matrix()
         return True
```

### Comparing `glglue-2.4.0/src/glglue/camera/mouse_camera.py` & `glglue-2.5.0/src/glglue/camera/mouse_camera.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/camera/mouse_event.py` & `glglue-2.5.0/src/glglue/camera/mouse_event.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,19 @@
 
 Callback: TypeAlias = Callable[[FrameInput, Optional[FrameInput]], None]
 BeginEndCallback: TypeAlias = Callable[[FrameInput], None]
 DragCallback: TypeAlias = Callable[[FrameInput, int, int], None]
 
 
 class DragInterface(Protocol):
-    def begin(self, mouse_input: FrameInput):
-        ...
+    def begin(self, mouse_input: FrameInput): ...
 
-    def drag(self, mouse_input: FrameInput, dx: int, dy: int):
-        ...
+    def drag(self, mouse_input: FrameInput, dx: int, dy: int): ...
 
-    def end(self, mouse_input: FrameInput):
-        ...
+    def end(self, mouse_input: FrameInput): ...
 
 
 class MouseEvent:
     def __init__(self) -> None:
         self.callbacks: List[Callback] = []
         self.last_input: Optional[FrameInput] = None
 
@@ -74,23 +71,27 @@
                 not self.last_input or not self.last_input.mouse_middle
             ) and current.mouse_middle:
                 self.middle_active = (current.mouse_x, current.mouse_y)
                 for callback in self.middle_pressed:
                     callback(current)
         # drag
         if current.is_active:
-            if current.mouse_left:
+            if (self.last_input and self.last_input.mouse_left) and current.mouse_left:
                 # self.left_active = True
                 for callback in self.left_drag:
                     callback(current, dx, dy)
-            if current.mouse_right:
+            if (
+                self.last_input and self.last_input.mouse_right
+            ) and current.mouse_right:
                 # self.right_active = True
                 for callback in self.right_drag:
                     callback(current, dx, dy)
-            if current.mouse_middle:
+            if (
+                self.last_input and self.last_input.mouse_middle
+            ) and current.mouse_middle:
                 # self.middle_active = True
                 for callback in self.middle_drag:
                     callback(current, dx, dy)
         # released
         if self.left_active and not current.mouse_left:
             for callback in self.left_released:
                 callback(current)
```

### Comparing `glglue-2.4.0/src/glglue/drawable/axes.py` & `glglue-2.5.0/src/glglue/drawable/axes.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/drawable/cube.py` & `glglue-2.5.0/src/glglue/drawable/cube.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/drawable/drawable.py` & `glglue-2.5.0/src/glglue/drawable/drawable.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/drawable/grid.py` & `glglue-2.5.0/src/glglue/drawable/grid.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/drawable/line_builder.py` & `glglue-2.5.0/src/glglue/drawable/line_builder.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/drawable/mesh_builder.py` & `glglue-2.5.0/src/glglue/drawable/mesh_builder.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/drawable/teapot.py` & `glglue-2.5.0/src/glglue/drawable/teapot.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/glfw.py` & `glglue-2.5.0/src/glglue/glfw.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/glo/fbo.py` & `glglue-2.5.0/src/glglue/glo/fbo.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/glo/shader.py` & `glglue-2.5.0/src/glglue/glo/shader.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/glo/texture.py` & `glglue-2.5.0/src/glglue/glo/texture.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/glo/vao.py` & `glglue-2.5.0/src/glglue/glo/vao.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 from typing import Iterable
-from OpenGL import GL  # type: ignore
+from OpenGL import GL
 from .vbo import Vbo, Ibo
 from .vertex_layout import VertexLayout
 import ctypes
 
 
 class Vao:
     def __init__(
         self,
         vbo: Vbo,
         layouts: Iterable[VertexLayout],
         ibo: Ibo | None = None,
         *,
-        topology: int = GL.GL_TRIANGLES,  # type: ignore
+        topology: int = GL.GL_TRIANGLES,
     ) -> None:
         self.topology = topology
         self.vao: int = GL.glGenVertexArrays(1)
         self.vbo = vbo
         self.bind()
         vbo.bind()
         for layout in layouts:
-            GL.glEnableVertexAttribArray(layout.attribute.location)  # type: ignore
+            GL.glEnableVertexAttribArray(layout.attribute.location)
             GL.glVertexAttribPointer(
                 layout.attribute.location,
                 layout.item_count,
-                GL.GL_FLOAT,  # type: ignore
-                GL.GL_FALSE,  # type: ignore
+                GL.GL_FLOAT,
+                GL.GL_FALSE,
                 layout.stride,
                 ctypes.c_void_p(layout.byte_offset),
             )
         self.ibo = None
         if ibo:
             self.ibo = ibo
             ibo.bind()
         self.unbind()
 
     def __del__(self) -> None:
         GL.glDeleteVertexArrays(1, [self.vao])
 
     def bind(self) -> None:
-        GL.glBindVertexArray(self.vao)  # type: ignore
+        GL.glBindVertexArray(self.vao)
 
     def unbind(self) -> None:
-        GL.glBindVertexArray(0)  # type: ignore
+        GL.glBindVertexArray(0)
 
     def draw(self, count: int, offset: int = 0, *, topology: int | None = None) -> None:
         if topology == None:
             topology = self.topology
 
         self.bind()
         if self.ibo:
-            GL.glDrawElements(topology, count, self.ibo.format, ctypes.c_void_p(offset * self.ibo.stride))  # type: ignore
+            GL.glDrawElements(
+                topology,
+                count,
+                self.ibo.format,
+                ctypes.c_void_p(offset * self.ibo.stride),
+            )
         else:
-            GL.glDrawArrays(topology, offset, count)  # type: ignore
+            GL.glDrawArrays(topology, offset, count)
         self.unbind()
```

### Comparing `glglue-2.4.0/src/glglue/glo/vbo.py` & `glglue-2.5.0/src/glglue/glo/vbo.py`

 * *Files 13% similar despite different names*

```diff
@@ -78,22 +78,26 @@
             indices,
             GL.GL_DYNAMIC_DRAW if is_dynamic else GL.GL_STATIC_DRAW,  # type: ignore
         )
         self.unbind()
 
     def set_indices(
         self,
-        indices: ctypes.Array[ctypes.c_ushort] | ctypes.Array[ctypes.c_uint],
+        indices: (
+            ctypes.Array[ctypes.c_uint16]
+            | ctypes.Array[ctypes.c_ushort]
+            | ctypes.Array[ctypes.c_uint]
+        ),
         *,
         is_dynamic: bool = False,
     ):
         match indices._type_:
-            case ctypes.c_ushort:
+            case ctypes.c_ushort | ctypes.c_uint16:
                 self.set_bytes(bytes(indices), 2, is_dynamic=is_dynamic)
-            case ctypes.c_uint:
+            case ctypes.c_uint | ctypes.c_int:
                 self.set_bytes(bytes(indices), 4, is_dynamic=is_dynamic)
             case _:
                 raise NotImplementedError()
 
     def update(
         self,
         indices: ctypes.Array[ctypes.c_ushort] | ctypes.Array[ctypes.c_uint],
```

### Comparing `glglue-2.4.0/src/glglue/glo/vertex_layout.py` & `glglue-2.5.0/src/glglue/glo/vertex_layout.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/glut.py` & `glglue-2.5.0/src/glglue/glut.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/gtk3.py` & `glglue-2.5.0/src/glglue/gtk3.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/gtk4.py` & `glglue-2.5.0/src/glglue/gtk4.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/pysdl2.py` & `glglue-2.5.0/src/glglue/pysdl2.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/pyside6.py` & `glglue-2.5.0/src/glglue/pyside6.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/qgl4.py` & `glglue-2.5.0/src/glglue/qgl4.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/qgl5.py` & `glglue-2.5.0/src/glglue/qgl5.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/scene/sample.py` & `glglue-2.5.0/src/glglue/scene/sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.end_render()
 
     def draw(self):
         if not self.initialized:
             self.initialized = True
 
             # shader
-            mesh_shader = glo.Shader.load_from_pkg("glglue", "assets/mesh")
+            mesh_shader = glo.Shader.load_from_pkg("glglue", "assets/vertex_color")
             self.drawables.append(
                 cube.create(
                     mesh_shader,
                     mesh_shader.create_props(self.mouse_camera.camera, self.cube_node),
                 )
             )
             self.drawables.append(
```

### Comparing `glglue-2.4.0/src/glglue/sdl.py` & `glglue-2.5.0/src/glglue/sdl.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/togl.py` & `glglue-2.5.0/src/glglue/togl.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/util.py` & `glglue-2.5.0/src/glglue/util.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/wgl.py` & `glglue-2.5.0/src/glglue/wgl.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/win32con.py` & `glglue-2.5.0/src/glglue/win32con.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/windowconfig.py` & `glglue-2.5.0/src/glglue/windowconfig.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue/wxglcanvas.py` & `glglue-2.5.0/src/glglue/wxglcanvas.py`

 * *Files identical despite different names*

### Comparing `glglue-2.4.0/src/glglue.egg-info/PKG-INFO` & `glglue-2.5.0/src/glglue.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glglue
-Version: 2.4.0
+Version: 2.5.0
 Summary: The glue code which mediates between OpenGL and some GUI
 Author-email: ousttrue <ousttrue@gmail.com>
 Project-URL: HomePage, https://ousttrue.github.io/glglue/
 Project-URL: Repository, https://github.com/ousttrue/glglue/
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling
@@ -38,16 +38,25 @@
 
 ## Requirements
 
 - Python 3.11
 
 ## status
 
-| platform | status | comment                                  |
-| -------- | ------ | ---------------------------------------- |
-| glut     | ok     | windows11, PATH to freeglut64.vc.dll     |
-| glfw     | ok     | windows11, pip install glfw              |
-| gtk3     | ?      | require gtk3 self build                  |
-| gtk4     | ?      | require gtk4 self build                  |
-| sdl2     | ok     | windows11, pip install pysdl2 pysdl2-dll |
-| qt6      | ok     | windows11, pip install pyside6)          |
-| win32    | ok     | windows11                                |
+| platform   | status | comment                                  |
+| ---------- | ------ | ---------------------------------------- |
+| win32      | ok     | windows11                                |
+| glut       | ok     | windows11, PATH to freeglut64.vc.dll     |
+| glfw       | ok     | windows11, pip install glfw              |
+| gtk3       | ?      | require gtk3 self build                  |
+| gtk4       | ok     | require gtk4 self build                  |
+| sdl2       | ok     | windows11, pip install pysdl2 pysdl2-dll |
+| qt6        | ok     | windows11, pip install pyside6           |
+| pyopengltk | ok     | windows11, pip install pyopengltk        |
+
+## upload
+
+```sh
+rm -rf dist
+py -m build --sdist
+twine upload dist/*
+```
```

### Comparing `glglue-2.4.0/src/glglue.egg-info/SOURCES.txt` & `glglue-2.5.0/src/glglue.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -37,31 +37,35 @@
 docs/static/img/undraw_docusaurus_mountain.svg
 docs/static/img/undraw_docusaurus_react.svg
 docs/static/img/undraw_docusaurus_tree.svg
 examples/basic/freeglut_sample.py
 examples/basic/glfw_sample.py
 examples/basic/gtk3_sample.py
 examples/basic/gtk4_sample.py
+examples/basic/pyopengltk_sample.py
 examples/basic/pysdl2_sample.py
 examples/basic/pyside6_sample.py
 examples/basic/wgl_sample.py
+examples/gui/pyside6_gizmo.py
 examples/gui/pyside6_gui.py
+examples/gui/scene.py
 examples/scene/pyside6_texture.py
 src/glglue/__init__.py
 src/glglue/_version.py
 src/glglue/frame_input.py
 src/glglue/glfw.py
 src/glglue/glut.py
 src/glglue/gtk3.py
 src/glglue/gtk4.py
 src/glglue/pysdl2.py
 src/glglue/pyside6.py
 src/glglue/qgl4.py
 src/glglue/qgl5.py
 src/glglue/sdl.py
+src/glglue/tk_frame.py
 src/glglue/togl.py
 src/glglue/util.py
 src/glglue/wgl.py
 src/glglue/win32con.py
 src/glglue/windowconfig.py
 src/glglue/wxglcanvas.py
 src/glglue.egg-info/PKG-INFO
@@ -70,30 +74,34 @@
 src/glglue.egg-info/requires.txt
 src/glglue.egg-info/top_level.txt
 src/glglue/assets/Utah_teapot_(solid).stl
 src/glglue/assets/line.frag
 src/glglue/assets/line.vert
 src/glglue/assets/mesh.frag
 src/glglue/assets/mesh.vert
+src/glglue/assets/vertex_color.frag
+src/glglue/assets/vertex_color.vert
 src/glglue/camera/__init__.py
 src/glglue/camera/camera.py
 src/glglue/camera/mouse_camera.py
 src/glglue/camera/mouse_event.py
 src/glglue/drawable/__init__.py
 src/glglue/drawable/axes.py
 src/glglue/drawable/cube.py
 src/glglue/drawable/drawable.py
 src/glglue/drawable/grid.py
 src/glglue/drawable/line_builder.py
 src/glglue/drawable/mesh_builder.py
 src/glglue/drawable/teapot.py
+src/glglue/gl_stubgen/__main__.py
 src/glglue/glo/__init__.py
 src/glglue/glo/fbo.py
 src/glglue/glo/shader.py
 src/glglue/glo/texture.py
 src/glglue/glo/vao.py
 src/glglue/glo/vbo.py
 src/glglue/glo/vertex_layout.py
 src/glglue/scene/sample.py
 tests/test_numpy.py
 tests/test_py.py
-tests/test_utils.py
+tests/test_utils.py
+typings/OpenGL/GL.pyi
```

### Comparing `glglue-2.4.0/tests/test_numpy.py` & `glglue-2.5.0/tests/test_numpy.py`

 * *Files identical despite different names*

