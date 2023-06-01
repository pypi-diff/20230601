# Comparing `tmp/anywidget-0.3.1.tar.gz` & `tmp/anywidget-0.4.0.tar.gz`

## Comparing `anywidget-0.3.1.tar` & `anywidget-0.4.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 anywidget-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget.json
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 anywidget-0.3.1/package.json
--rw-r--r--   0        0        0   251374 2020-02-02 00:00:00.000000 anywidget-0.3.1/pnpm-lock.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.3.1/pnpm-workspace.yaml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.3.1/.changeset/config.json
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/__init__.py
--rw-r--r--   0        0        0    24407 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/_descriptor.py
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/_file_contents.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/_protocols.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/_util.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/py.typed
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/widget.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/labextension/package.json
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/labextension/static/138.71df560f1970e2814d80.js
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/labextension/static/326.ca449025cbc7a2514a5d.js
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/labextension/static/remoteEntry.2cfd77956dbb25c1a49d.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/nbextension/extension.js
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 anywidget-0.3.1/anywidget/nbextension/index.js
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/astro.config.mjs
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/package.json
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/tailwind.config.cjs
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/tsconfig.json
--rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/public/anywidget-overview.png
--rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/public/banner-dark.png
--rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/public/banner-light.png
--rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/public/banner-minimal.png
--rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/public/client-js-diagram.png
--rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/public/default-og-image.png
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/public/favicon.svg
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/public/make-scrollable-code-focusable.js
--rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/public/widget-overview.png
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/scripts/ipynb.mjs
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/scripts/render.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/scripts/utils.mjs
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/consts.ts
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/env.d.ts
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/languages.ts
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/util.ts
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/CodeHero.astro
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/ConfettiButton.astro
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Counter.astro
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/CounterButton.astro
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/HeadCommon.astro
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/HeadSEO.astro
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Hero.astro
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Footer/AvatarList.astro
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Footer/Footer.astro
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/AnyWidgetLogo.astro
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/AstroLogo.astro
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/Header.astro
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/HeaderButton.css
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/LanguageSelect.css
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/LanguageSelect.tsx
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/Search.css
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/Search.tsx
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/SidebarToggle.css
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/SidebarToggle.tsx
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/SkipToContent.astro
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/ThemeToggleButton.css
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/Header/ThemeToggleButton.tsx
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/LeftSidebar/LeftSidebar.astro
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/PageContent/PageContent.astro
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/RightSidebar/MoreMenu.astro
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/RightSidebar/RightSidebar.astro
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/RightSidebar/TableOfContents.tsx
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/components/examples/Counter.astro
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/layouts/MainLayout.astro
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/layouts/SplashLayout.astro
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/pages/index.astro
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/pages/blog/anywidget-02.md
--rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/pages/blog/introducing-anywidget.mdx
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/pages/en/bundling.md
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/pages/en/getting-started.mdx
--rw-r--r--   0        0        0    10644 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/pages/en/jupyter-widgets-the-good-parts.md
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/pages/en/notebooks/counter.ipynb
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/styles/index.css
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.3.1/docs/src/styles/theme.css
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 anywidget-0.3.1/examples/Counter.ipynb
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 anywidget-0.3.1/examples/minimal_example.ipynb
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 anywidget-0.3.1/packages/anywidget/CHANGELOG.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.3.1/packages/anywidget/build.mjs
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.3.1/packages/anywidget/package.json
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.3.1/packages/anywidget/src/index.js
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.3.1/packages/anywidget/src/plugin.js
--rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 anywidget-0.3.1/packages/anywidget/src/widget.js
--rw-r--r--   0        0        0     9118 2020-02-02 00:00:00.000000 anywidget-0.3.1/tests/test_descriptor.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.3.1/tests/test_file_contents.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.3.1/tests/test_protocols.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.3.1/tests/test_utils.py
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 anywidget-0.3.1/tests/test_widget.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.3.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.3.1/LICENSE
--rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 anywidget-0.3.1/README.md
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 anywidget-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 anywidget-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 anywidget-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget.json
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 anywidget-0.4.0/package.json
+-rw-r--r--   0        0        0   251374 2020-02-02 00:00:00.000000 anywidget-0.4.0/pnpm-lock.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.4.0/pnpm-workspace.yaml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.4.0/.changeset/config.json
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/__init__.py
+-rw-r--r--   0        0        0    25080 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/_descriptor.py
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/_file_contents.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/_protocols.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/_util.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/py.typed
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/widget.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/labextension/package.json
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/labextension/static/138.c787b75870b3f713865b.js
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/labextension/static/326.3de5744b11f9f83e61f3.js
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/labextension/static/remoteEntry.53667379a2ee93d6fe11.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/nbextension/extension.js
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 anywidget-0.4.0/anywidget/nbextension/index.js
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/astro.config.mjs
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/package.json
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/tailwind.config.cjs
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/tsconfig.json
+-rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/public/anywidget-overview.png
+-rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/public/banner-dark.png
+-rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/public/banner-light.png
+-rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/public/banner-minimal.png
+-rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/public/client-js-diagram.png
+-rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/public/default-og-image.png
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/public/favicon.svg
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/public/make-scrollable-code-focusable.js
+-rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/public/widget-overview.png
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/scripts/ipynb.mjs
+-rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/scripts/render.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/scripts/utils.mjs
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/consts.ts
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/env.d.ts
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/languages.ts
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/util.ts
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/CodeHero.astro
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/ConfettiButton.astro
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Counter.astro
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/CounterButton.astro
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/HeadCommon.astro
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/HeadSEO.astro
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Hero.astro
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Footer/AvatarList.astro
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Footer/Footer.astro
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/AnyWidgetLogo.astro
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/AstroLogo.astro
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/Header.astro
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/HeaderButton.css
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/LanguageSelect.css
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/LanguageSelect.tsx
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/Search.css
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/Search.tsx
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/SidebarToggle.css
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/SidebarToggle.tsx
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/SkipToContent.astro
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/ThemeToggleButton.css
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/Header/ThemeToggleButton.tsx
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/LeftSidebar/LeftSidebar.astro
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/PageContent/PageContent.astro
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/RightSidebar/MoreMenu.astro
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/RightSidebar/RightSidebar.astro
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/RightSidebar/TableOfContents.tsx
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/components/examples/Counter.astro
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/layouts/MainLayout.astro
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/layouts/SplashLayout.astro
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/pages/index.astro
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/pages/blog/anywidget-02.md
+-rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/pages/blog/introducing-anywidget.mdx
+-rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/pages/en/bundling.md
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/pages/en/getting-started.mdx
+-rw-r--r--   0        0        0    10644 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/pages/en/jupyter-widgets-the-good-parts.md
+-rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/pages/en/notebooks/counter.ipynb
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/styles/index.css
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.4.0/docs/src/styles/theme.css
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 anywidget-0.4.0/examples/Counter.ipynb
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 anywidget-0.4.0/examples/minimal_example.ipynb
+-rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 anywidget-0.4.0/packages/anywidget/CHANGELOG.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.4.0/packages/anywidget/build.mjs
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.4.0/packages/anywidget/package.json
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.4.0/packages/anywidget/src/index.js
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.4.0/packages/anywidget/src/plugin.js
+-rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 anywidget-0.4.0/packages/anywidget/src/widget.js
+-rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 anywidget-0.4.0/tests/test_descriptor.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.4.0/tests/test_file_contents.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.4.0/tests/test_protocols.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.4.0/tests/test_utils.py
+-rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 anywidget-0.4.0/tests/test_widget.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 anywidget-0.4.0/README.md
+-rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 anywidget-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 anywidget-0.4.0/PKG-INFO
```

### Comparing `anywidget-0.3.1/.pre-commit-config.yaml` & `anywidget-0.4.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -33,7 +33,8 @@
         exclude: tests|docs
         # packages in the pre-commit env will determine what can be type checked
         # it does NOT automatically include all packages required by the project
         additional_dependencies:
           - pydantic
           - psygnal
           - watchfiles
+          - msgspec
```

### Comparing `anywidget-0.3.1/package.json` & `anywidget-0.4.0/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/pnpm-lock.yaml` & `anywidget-0.4.0/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/anywidget/_descriptor.py` & `anywidget-0.4.0/anywidget/_descriptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     remove_buffers,
     try_file_contents,
 )
 from ._version import __version__
 
 if TYPE_CHECKING:  # pragma: no cover
     import comm
+    import msgspec
     import psygnal
     import pydantic
     import traitlets
     from typing_extensions import TypeAlias, TypeGuard
 
     from ._protocols import CommMessage
 
@@ -481,14 +482,17 @@
 
     if _is_traitlets_object(obj):
         return _get_traitlets_state
 
     if _is_pydantic_model(obj):
         return _get_pydantic_state
 
+    if _is_msgspec_struct(obj):
+        return _get_msgspec_state
+
     # pickle protocol ... probably not type-safe enough for our purposes
     # https://docs.python.org/3/library/pickle.html#object.__getstate__
     # if hasattr(type(obj), "__getstate__"):
     #     return type(obj).__getstate__
 
     raise TypeError(  # pragma: no cover
         f"Cannot determine a state-getting method for {obj!r}. "
@@ -638,7 +642,26 @@
     """Get the state of a pydantic BaseModel instance.
 
     To take advantage of pydantic's support for custom encoders (with json_encoders)
     we call obj.json() here, and then cast back to a dict (which is what the comm
     expects.)
     """
     return json.loads(obj.json())
+
+
+# ------------- msgspec support --------------
+
+
+def _is_msgspec_struct(obj: Any) -> TypeGuard[msgspec.Struct]:
+    """Return `True` if an object is an instance of msgspec.Struct."""
+    msgspec = sys.modules.get("msgspec")
+    return isinstance(obj, msgspec.Struct) if msgspec is not None else False
+
+
+def _get_msgspec_state(obj: msgspec.Struct) -> dict:
+    """Get the state of a msgspec.Struct instance."""
+    import msgspec
+
+    # FIXME:
+    # see discussion here:
+    # https://github.com/manzt/anywidget/pull/64/files#r1129327721
+    return cast(dict, msgspec.to_builtins(obj))
```

### Comparing `anywidget-0.3.1/anywidget/_file_contents.py` & `anywidget-0.4.0/anywidget/_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/anywidget/_protocols.py` & `anywidget-0.4.0/anywidget/_protocols.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/anywidget/_util.py` & `anywidget-0.4.0/anywidget/_util.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/anywidget/widget.py` & `anywidget-0.4.0/anywidget/widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/anywidget/labextension/package.json` & `anywidget-0.4.0/anywidget/labextension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95703125%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.53667379a2ee93d6fe11.js'}}",*

 * * "'version'": "'0.4.0'"}*

```diff
@@ -22,15 +22,15 @@
     },
     "files": [
         "dist"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.2cfd77956dbb25c1a49d.js"
+            "load": "static/remoteEntry.53667379a2ee93d6fe11.js"
         },
         "extension": "src/plugin",
         "outputDir": "../../anywidget/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -42,9 +42,9 @@
     "name": "anywidget",
     "publishConfig": {
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs"
     },
-    "version": "0.3.1"
+    "version": "0.4.0"
 }
```

### Comparing `anywidget-0.3.1/anywidget/labextension/static/138.71df560f1970e2814d80.js` & `anywidget-0.4.0/anywidget/labextension/static/138.c787b75870b3f713865b.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -92,11 +92,11 @@
                 return {
                     AnyModel: t,
                     AnyView: i
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.3.1"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.4.0"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.3.1/anywidget/labextension/static/326.ca449025cbc7a2514a5d.js` & `anywidget-0.4.0/anywidget/labextension/static/326.3de5744b11f9f83e61f3.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -110,11 +110,11 @@
                 return {
                     AnyModel: t,
                     AnyView: i
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.3.1"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.4.0"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.3.1/anywidget/labextension/static/remoteEntry.2cfd77956dbb25c1a49d.js` & `anywidget-0.4.0/anywidget/labextension/static/remoteEntry.53667379a2ee93d6fe11.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -22,109 +22,109 @@
                     get: () => o,
                     init: () => a
                 })
             }
         },
         g = {};
 
-    function m(e) {
+    function b(e) {
         var r = g[e];
         if (void 0 !== r) return r.exports;
         var t = g[e] = {
             exports: {}
         };
-        return v[e](t, t.exports, m), t.exports
+        return v[e](t, t.exports, b), t.exports
     }
-    m.m = v, m.c = g, m.n = e => {
+    b.m = v, b.c = g, b.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return m.d(r, {
+        return b.d(r, {
             a: r
         }), r
-    }, m.d = (e, r) => {
-        for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
+    }, b.d = (e, r) => {
+        for (var t in r) b.o(r, t) && !b.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        138: "71df560f1970e2814d80",
-        326: "ca449025cbc7a2514a5d"
+    }, b.f = {}, b.e = e => Promise.all(Object.keys(b.f).reduce(((r, t) => (b.f[t](e, r), r)), [])), b.u = e => e + "." + {
+        138: "c787b75870b3f713865b",
+        326: "3de5744b11f9f83e61f3"
     } [e] + ".js?v=" + {
-        138: "71df560f1970e2814d80",
-        326: "ca449025cbc7a2514a5d"
-    } [e], m.g = function() {
+        138: "c787b75870b3f713865b",
+        326: "3de5744b11f9f83e61f3"
+    } [e], b.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", m.l = (t, n, o, a) => {
+    }(), b.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", b.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
                 for (var f = document.getElementsByTagName("script"), l = 0; l < f.length; l++) {
                     var s = f[l];
                     if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
                         i = s;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, b.nc && i.setAttribute("nonce", b.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
                 c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, m.r = e => {
+    }, b.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        m.S = {};
+        b.S = {};
         var e = {},
             r = {};
-        m.I = (t, n) => {
+        b.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                m.o(m.S, t) || (m.S[t] = {});
-                var a = m.S[t],
+                b.o(b.S, t) || (b.S[t] = {});
+                var a = b.S[t],
                     i = "anywidget",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => m.e(138).then((() => () => m(138))),
+                        get: () => b.e(138).then((() => () => b(138))),
                         from: i,
                         eager: !1
                     })
-                })("anywidget", "0.3.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("anywidget", "0.4.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        m.g.importScripts && (e = m.g.location + "");
-        var r = m.g.document;
+        b.g.importScripts && (e = b.g.location + "");
+        var r = b.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             t.length && (e = t[t.length - 1].src)
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), m.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), b.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -190,85 +190,85 @@
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
         return !!p()
     }, i = (e, r) => {
-        var t = m.S[e];
-        if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = b.S[e];
+        if (!t || !b.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", l = (e, r, t, n) => {
         var o = u(e, t);
         return a(n, o) || "undefined" != typeof console && console.warn && console.warn(f(e, t, o, n)), s(e[t][o])
     }, s = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
-        var a = m.I(r);
-        return a && a.then ? a.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
+        var a = b.I(r);
+        return a && a.then ? a.then(e.bind(e, r, b.S[r], t, n, o)) : e(r, b.S[r], t, n)
     })(((e, r, t, n) => (i(e, t), l(r, 0, t, n)))), c = {}, p = {
         395: () => d("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1, 1
         ])
     }, h = {
         326: [395]
-    }, m.f.consumes = (e, r) => {
-        m.o(h, e) && h[e].forEach((e => {
-            if (m.o(c, e)) return r.push(c[e]);
+    }, b.f.consumes = (e, r) => {
+        b.o(h, e) && h[e].forEach((e => {
+            if (b.o(c, e)) return r.push(c[e]);
             var t = r => {
-                    c[e] = 0, m.m[e] = t => {
-                        delete m.c[e], t.exports = r()
+                    c[e] = 0, b.m[e] = t => {
+                        delete b.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete c[e], m.m[e] = t => {
-                        throw delete m.c[e], r
+                    delete c[e], b.m[e] = t => {
+                        throw delete b.c[e], r
                     }
                 };
             try {
                 var o = p[e]();
                 o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             957: 0
         };
-        m.f.j = (r, t) => {
-            var n = m.o(e, r) ? e[r] : void 0;
+        b.f.j = (r, t) => {
+            var n = b.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var o = new Promise(((t, o) => n = e[r] = [t, o]));
                     t.push(n[2] = o);
-                    var a = m.p + m.u(r),
+                    var a = b.p + b.u(r),
                         i = new Error;
-                    m.l(a, (t => {
-                        if (m.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                    b.l(a, (t => {
+                        if (b.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var o = t && ("load" === t.type ? "missing" : t.type),
                                 a = t && t.target && t.target.src;
                             i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, o, [a, i, u] = t,
                     f = 0;
                 if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) m.o(i, n) && (m.m[n] = i[n]);
-                    u && u(m)
+                    for (n in i) b.o(i, n) && (b.m[n] = i[n]);
+                    u && u(b)
                 }
-                for (r && r(t); f < a.length; f++) o = a[f], m.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); f < a.length; f++) o = a[f], b.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkanywidget = self.webpackChunkanywidget || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var b = m(408);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = b
+    var m = b(408);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = m
 })();
```

### Comparing `anywidget-0.3.1/anywidget/nbextension/index.js` & `anywidget-0.4.0/anywidget/nbextension/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 // package.json
 var name = "anywidget";
-var version = "0.3.1";
+var version = "0.4.0";
 
 // src/widget.js
 function is_href(str) {
     return str.startsWith("http://") || str.startsWith("https://");
 }
 async function load_css_href(href, anywidget_id) {
     let prev = document.querySelector(`link[id='${anywidget_id}']`);
```

### Comparing `anywidget-0.3.1/docs/README.md` & `anywidget-0.4.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/astro.config.mjs` & `anywidget-0.4.0/docs/astro.config.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/package.json` & `anywidget-0.4.0/docs/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/public/anywidget-overview.png` & `anywidget-0.4.0/docs/public/anywidget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/public/banner-dark.png` & `anywidget-0.4.0/docs/public/banner-dark.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/public/banner-light.png` & `anywidget-0.4.0/docs/public/banner-light.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/public/banner-minimal.png` & `anywidget-0.4.0/docs/public/banner-minimal.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/public/client-js-diagram.png` & `anywidget-0.4.0/docs/public/client-js-diagram.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/public/default-og-image.png` & `anywidget-0.4.0/docs/public/default-og-image.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/public/favicon.svg` & `anywidget-0.4.0/docs/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/public/widget-overview.png` & `anywidget-0.4.0/docs/public/widget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/scripts/ipynb.mjs` & `anywidget-0.4.0/docs/scripts/ipynb.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/scripts/utils.mjs` & `anywidget-0.4.0/docs/scripts/utils.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/consts.ts` & `anywidget-0.4.0/docs/src/consts.ts`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/CodeHero.astro` & `anywidget-0.4.0/docs/src/components/CodeHero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/CounterButton.astro` & `anywidget-0.4.0/docs/src/components/CounterButton.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/HeadCommon.astro` & `anywidget-0.4.0/docs/src/components/HeadCommon.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/HeadSEO.astro` & `anywidget-0.4.0/docs/src/components/HeadSEO.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/Hero.astro` & `anywidget-0.4.0/docs/src/components/Hero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/Footer/AvatarList.astro` & `anywidget-0.4.0/docs/src/components/Footer/AvatarList.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/Header/AnyWidgetLogo.astro` & `anywidget-0.4.0/docs/src/components/Header/AnyWidgetLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/Header/AstroLogo.astro` & `anywidget-0.4.0/docs/src/components/Header/AstroLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/Header/Header.astro` & `anywidget-0.4.0/docs/src/components/Header/Header.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/Header/HeaderButton.css` & `anywidget-0.4.0/docs/src/components/Header/HeaderButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/Header/LanguageSelect.css` & `anywidget-0.4.0/docs/src/components/Header/LanguageSelect.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/Header/LanguageSelect.tsx` & `anywidget-0.4.0/docs/src/components/Header/LanguageSelect.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/Header/Search.css` & `anywidget-0.4.0/docs/src/components/Header/Search.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/Header/Search.tsx` & `anywidget-0.4.0/docs/src/components/Header/Search.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/Header/SidebarToggle.tsx` & `anywidget-0.4.0/docs/src/components/Header/SidebarToggle.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/Header/ThemeToggleButton.css` & `anywidget-0.4.0/docs/src/components/Header/ThemeToggleButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/Header/ThemeToggleButton.tsx` & `anywidget-0.4.0/docs/src/components/Header/ThemeToggleButton.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/LeftSidebar/LeftSidebar.astro` & `anywidget-0.4.0/docs/src/components/LeftSidebar/LeftSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/PageContent/PageContent.astro` & `anywidget-0.4.0/docs/src/components/PageContent/PageContent.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/RightSidebar/MoreMenu.astro` & `anywidget-0.4.0/docs/src/components/RightSidebar/MoreMenu.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/RightSidebar/RightSidebar.astro` & `anywidget-0.4.0/docs/src/components/RightSidebar/RightSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/RightSidebar/TableOfContents.tsx` & `anywidget-0.4.0/docs/src/components/RightSidebar/TableOfContents.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/components/examples/Counter.astro` & `anywidget-0.4.0/docs/src/components/examples/Counter.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/layouts/MainLayout.astro` & `anywidget-0.4.0/docs/src/layouts/MainLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/layouts/SplashLayout.astro` & `anywidget-0.4.0/docs/src/layouts/SplashLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/pages/blog/anywidget-02.md` & `anywidget-0.4.0/docs/src/pages/blog/anywidget-02.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/pages/blog/introducing-anywidget.mdx` & `anywidget-0.4.0/docs/src/pages/blog/introducing-anywidget.mdx`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/pages/en/bundling.md` & `anywidget-0.4.0/docs/src/pages/en/bundling.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description: Docs bundling
 layout: ../../layouts/MainLayout.astro
 ---
 
 Often the ESM required to connect a JavaScript library to Python with
 **anywidget** is minimal and can easily be inlined _within_ the Python module as
 a string. This feature allows Python developers to be productive with
-**anywidget** without requiring intimite knowledge or the overhead of frontend
+**anywidget** without requiring intimate knowledge or the overhead of frontend
 tooling (e.g., `npm`/`yarn`/`pnpm`, Webpack/Vite/esbuild).
 
 As **anywidget** projects mature, however, it is recommended to organize the
 JavaScript source into separate files which can be merged together into a single
 optimized ESM file. This merging process is called _bundling_ and is required by
 popular fontend frameworks (e.g., React, Vue, Solid, Svelte) which use
 unsupported browser syntax.
@@ -85,15 +85,15 @@
 ```
 
 
 ## Vite
 
 Our [Vite](https://vitejs.dev/) plugin offers a more fully featured development
 experience compared to **anywidget**'s builtin HMR, but at the cost of added
-project complexity and tooling. Vite is a good choice if you are want to
+project complexity and tooling. Vite is a good choice if you want to
 use a front-end framework like Svelte or Vue or need more fine grain control
 over your bundling.
 
 ### Project Setup
 
 From the root of the project structure above.
 
@@ -132,15 +132,15 @@
 │  ├── index.js
 │  └── styles.css
 └── vite.config.js
 ```
 
 ### Build
 
-We can now bundle the assets into `hellow_widget/static` with Vite, just like
+We can now bundle the assets into `hello_widget/static` with Vite, just like
 esbuild. Again, make sure the final bundled assets are loaded by the Python
 module.
 
 ```bash
 npx vite build
 # vite v4.0.4 building for production...
 # ✓ 2 modules transformed.
@@ -210,9 +210,9 @@
 
 class HelloWidget(anywidget.AnyWidget):
   _esm = ESM
   _css = CSS
   name = traitlets.Unicode().tag(sync=True)
 ```
 
-Any changes to `src/*` will now be updated immediate in active output cells with
-for this widget. Happy coding!
+Any changes to `src/*` will now be updated immediately in active output cells with
+this widget. Happy coding!
```

### Comparing `anywidget-0.3.1/docs/src/pages/en/getting-started.mdx` & `anywidget-0.4.0/docs/src/pages/en/getting-started.mdx`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/pages/en/jupyter-widgets-the-good-parts.md` & `anywidget-0.4.0/docs/src/pages/en/jupyter-widgets-the-good-parts.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/pages/en/notebooks/counter.ipynb` & `anywidget-0.4.0/docs/src/pages/en/notebooks/counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/styles/index.css` & `anywidget-0.4.0/docs/src/styles/index.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/docs/src/styles/theme.css` & `anywidget-0.4.0/docs/src/styles/theme.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/examples/Counter.ipynb` & `anywidget-0.4.0/examples/Counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/examples/minimal_example.ipynb` & `anywidget-0.4.0/examples/minimal_example.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/packages/anywidget/CHANGELOG.md` & `anywidget-0.4.0/packages/anywidget/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,28 @@
 # anywidget
 
+## 0.4.0
+
+### Minor Changes
+
+- feat: Add support for evented msgspec.Struct objects ([#64](https://github.com/manzt/anywidget/pull/64))
+
+  Our experimental descriptor API can now work with [`msgspec`](https://jcristharif.com/msgspec/), a fast and efficient serialization library, similar to `pydantic` but with a stronger emphasis on ser/de, and less on runtime casting of Python types.
+
+  ```python
+  from anywidget._descriptor import MimeBundleDescriptor
+  import psygnal
+  import msgspec
+
+  @psygnal.evented
+  class Counter(msgspec.Struct, weakref=True):
+      value: int = 0
+      _repr_mimebundle_: ClassVar = MimeBundleDescriptor(_esm="index.js", autodetect_observer=False)
+  ```
+
 ## 0.3.1
 
 ### Patch Changes
 
 - fix: properly cache cleanup function for HMR ([#122](https://github.com/manzt/anywidget/pull/122))
 
 ## 0.3.0
```

### Comparing `anywidget-0.3.1/packages/anywidget/build.mjs` & `anywidget-0.4.0/packages/anywidget/build.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/packages/anywidget/package.json` & `anywidget-0.4.0/packages/anywidget/package.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'0.4.0'"}*

```diff
@@ -38,9 +38,9 @@
     "name": "anywidget",
     "publishConfig": {
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs"
     },
-    "version": "0.3.1"
+    "version": "0.4.0"
 }
```

### Comparing `anywidget-0.3.1/packages/anywidget/src/widget.js` & `anywidget-0.4.0/packages/anywidget/src/widget.js`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/tests/test_descriptor.py` & `anywidget-0.4.0/tests/test_descriptor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import pathlib
 import time
 import weakref
 from dataclasses import dataclass
-from typing import ClassVar
+from typing import TYPE_CHECKING, ClassVar
 from unittest.mock import MagicMock, patch
 
 import anywidget._descriptor
 import pytest
 import watchfiles
 from anywidget._descriptor import (
     _COMMS,
     _WIDGET_MIME_TYPE,
     MimeBundleDescriptor,
     ReprMimeBundle,
 )
 from anywidget._file_contents import FileContents
 from watchfiles import Change
 
+if TYPE_CHECKING:
+    from anywidget._protocols import AnywidgetProtocol
+    from ipykernel.comm import Comm
+
 
 class MockComm(MagicMock):
     # The only thing we need to do is to be able to relay messages back to
     # msg_callback, which is set by the descriptor using the on_msg method.
 
     msg_callback = None
 
@@ -38,14 +42,31 @@
     comm = MockComm()
     assert not _COMMS
     with patch.object(anywidget._descriptor, "open_comm", return_value=comm):
         yield comm
     assert not _COMMS
 
 
+def _send_value(comm: "Comm", value: int) -> int:
+    # test that the object responds to incoming messages
+    comm.handle_msg(
+        {"content": {"data": {"method": "update", "state": {"value": value}}}}
+    )
+    return value
+
+
+def _assert_sends_update(wdg: "AnywidgetProtocol", comm: MagicMock, expect: int):
+    # test that the comm sends update messages
+    wdg._repr_mimebundle_.send_state({"value"})
+    comm.send.assert_called_with(
+        data={"method": "update", "state": {"value": expect}, "buffer_paths": []},
+        buffers=[],
+    )
+
+
 def test_descriptor(mock_comm: MagicMock) -> None:
     """Test that the descriptor decorator makes a comm, and gets/sets state."""
 
     VAL = 1
 
     class Foo:
         _repr_mimebundle_ = MimeBundleDescriptor(autodetect_observer=False)
@@ -61,26 +82,18 @@
     mock_comm.send.assert_called_once()
     assert isinstance(repr_method, ReprMimeBundle)
     bundle = repr_method()
     assert _WIDGET_MIME_TYPE in bundle[0]  # we can call it as usual
     assert len(bundle[1]) == 0
 
     # test that the comm sends update messages
-    foo._repr_mimebundle_.send_state({"value"})
-    mock_comm.send.assert_called_with(
-        data={"method": "update", "state": {"value": VAL}, "buffer_paths": []},
-        buffers=[],
-    )
+    _assert_sends_update(foo, mock_comm, VAL)
 
     # test that the object responds to incoming messages
-    NEW_VAL = 3
-    mock_comm.handle_msg(
-        {"content": {"data": {"method": "update", "state": {"value": NEW_VAL}}}}
-    )
-    assert foo.value == NEW_VAL
+    assert _send_value(mock_comm, 3) == foo.value
 
     mock_comm.send.reset_mock()
     mock_comm.handle_msg({"content": {"data": {"method": "request_state"}}})
     mock_comm.send.assert_called()
 
 
 def test_state_setter(mock_comm: MagicMock):
@@ -187,40 +200,60 @@
 
     assert repr_obj._disconnectors
     del foo
     assert not repr_obj._disconnectors
 
 
 def test_descriptor_with_pydantic(mock_comm: MagicMock):
-    pydantic = pytest.importorskip("pydantic")
+    if TYPE_CHECKING:
+        import pydantic
+    else:
+        pydantic = pytest.importorskip("pydantic")
 
     VAL = 1
 
     class Foo(pydantic.BaseModel):
         __slots__ = ("__weakref__",)
         value: int = VAL
 
         _repr_mimebundle_: ClassVar = MimeBundleDescriptor(autodetect_observer=False)
 
     foo = Foo()
     foo._repr_mimebundle_  # create the comm
 
     # test that the comm sends update messages
-    foo._repr_mimebundle_.send_state({"value"})
-    mock_comm.send.assert_called_with(
-        data={"method": "update", "state": {"value": VAL}, "buffer_paths": []},
-        buffers=[],
-    )
+    _assert_sends_update(foo, mock_comm, VAL)
 
     # test that the object responds to incoming messages
-    NEW_VAL = 3
-    mock_comm.handle_msg(
-        {"content": {"data": {"method": "update", "state": {"value": NEW_VAL}}}}
-    )
-    assert foo.value == NEW_VAL
+    assert _send_value(mock_comm, 3) == foo.value
+
+
+def test_descriptor_with_msgspec(mock_comm: MagicMock):
+    if TYPE_CHECKING:
+        import msgspec
+        import psygnal
+    else:
+        psygnal = pytest.importorskip("psygnal")
+        msgspec = pytest.importorskip("msgspec")
+
+    VAL = 1
+
+    @psygnal.evented
+    class Foo(msgspec.Struct, weakref=True):
+        value: int = VAL
+        _repr_mimebundle_: ClassVar = MimeBundleDescriptor(autodetect_observer=False)
+
+    foo = Foo()
+    foo._repr_mimebundle_  # create the comm
+
+    # test that the comm sends update messages
+    _assert_sends_update(foo, mock_comm, VAL)
+
+    # test that the object responds to incoming messages
+    assert _send_value(mock_comm, 3) == foo.value
 
 
 def test_descriptor_with_traitlets(mock_comm: MagicMock):
     import traitlets
 
     class Foo(traitlets.HasTraits):
         value = traitlets.Int(0).tag(sync=True)
```

### Comparing `anywidget-0.3.1/tests/test_file_contents.py` & `anywidget-0.4.0/tests/test_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/tests/test_utils.py` & `anywidget-0.4.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/tests/test_widget.py` & `anywidget-0.4.0/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/LICENSE` & `anywidget-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/README.md` & `anywidget-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.3.1/pyproject.toml` & `anywidget-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 [project.optional-dependencies]
 test = [
     "black[jupyter]",
     "pydantic",
     "pytest",
     "pytest-cov",
     "ruff",
+    "ipython<8.13; python_version < '3.9'",
 ]
 dev = [
     "comm>=0.1.0",
     "watchfiles>=0.18.0",
 ]
 
 [project.urls]
```

### Comparing `anywidget-0.3.1/PKG-INFO` & `anywidget-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anywidget
-Version: 0.3.1
+Version: 0.4.0
 Summary: custom jupyter widgets made easy
 Project-URL: homepage, https://github.com/manzt/anywidget
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: importlib-metadata; python_version < '3.8'
@@ -12,14 +12,15 @@
 Requires-Dist: psygnal>=0.8.1
 Requires-Dist: typing-extensions>=4.2.0
 Provides-Extra: dev
 Requires-Dist: comm>=0.1.0; extra == 'dev'
 Requires-Dist: watchfiles>=0.18.0; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: black[jupyter]; extra == 'test'
+Requires-Dist: ipython<8.13; python_version < '3.9' and extra == 'test'
 Requires-Dist: pydantic; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: ruff; extra == 'test'
 Description-Content-Type: text/markdown
 
 # anywidget <a href="https://github.com/manzt/anywidget"><img align="right" src="https://raw.githubusercontent.com/manzt/anywidget/main/docs/public/favicon.svg" height="38"></img></a>
```

