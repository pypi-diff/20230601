# Comparing `tmp/markata-0.7.0.dev5.tar.gz` & `tmp/markata-0.7.0.dev6.tar.gz`

## Comparing `markata-0.7.0.dev5.tar` & `markata-0.7.0.dev6.tar`

### file list

```diff
@@ -1,150 +1,151 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.markataignore
--rw-r--r--   0        0        0    17369 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/CHANGELOG.md
--rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/contributing.md
--rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata.toml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/1e69785050fd2c22
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/20eff344600dde07
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/24fbff1ddd04ec29
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/29c4d58b8315fe7
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/2a8c5b68d2f97df6
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/2db5fbf8536d61c8
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/34a658c3bca2be01
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/35719d79e8c04614
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/35c0e5dd90e9935e
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/362b7b38f7dd9584
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/383e2af8ad57a880
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/3eb26de4e6ce99a9
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/403cd3cd55046689
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/47ae7a7fff438a0d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/4c9fd647c7ee95f4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/4e095fd64e47625e
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/5331f80eed96d382
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/59cad1605f1af3e5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/5a1e19cb6d7f7dad
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/5ac2f908f7fe3e24
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/5b7a1f63fc38e03d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/66d8b82b56eb500
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/6f014ef899de75b8
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/70bc721b5aef832c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/7149a3e726874711
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/7414a3142f98f09a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/78d964febbc793b6
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/78e4f510470a816d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/79195e87c9b30787
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/7b0e96c06746aa61
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/7d99ecc9c87ed5f0
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/80a8cf59b4bc17e1
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/86dc7a48d3e9f55f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/89374bb2f512f7f6
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/99b23d496a02699d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/99ff118692cde90c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/a6996a6d25c48ddf
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/b0011511774c7dca
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/b1f840327e835f52
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/b2cd8e7293d4f4b9
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/b5c378e121358265
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/bb5999702a60d48b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/be76182c3e5eb829
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/d29fbd67f3100dc5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/d5ae70b2eca37fb3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/deefb80c5e63805
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/e1477e95ab98702d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/e14d0ae02634c6e4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/e2255c9643e910d2
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/e3036bdc181a2d74
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/e525c6e61701df76
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/e91605f11dc6030
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/f017a558be8a1865
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.ruff_cache/content/f3849d1b74b057b2
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/docs/404.md
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/docs/color-theme.md
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/docs/home-page.md
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/docs/index.md
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/docs/nav.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/docs/project-gallery/markata_dev.md
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/docs/project-gallery/waylonwalker.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/__about__.py
--rw-r--r--   0        0        0    15949 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/__main__.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/background.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/errors.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/hookspec.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/lifecycle.py
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/standard_config.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/cli/__init__.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/cli/__main__.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/cli/cli.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/cli/header.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/cli/plugins.py
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/cli/runner.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/cli/server.py
--rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/cli/summary.py
--rw-r--r--   0        0        0    38304 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/Karla-Regular.ttf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/__init__.py
--rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/auto_description.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/auto_title.py
--rw-r--r--   0        0        0    16607 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/base_cli.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/copy_assets.py
--rw-r--r--   0        0        0     7472 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/covers.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/create_covers.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/datetime.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/default_doc_template.md
--rw-r--r--   0        0        0    13176 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/default_log_template.html
--rw-r--r--   0        0        0    21666 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/default_post_template.html
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/default_redirect_template.html
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/default_service_worker_template.js
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/docs.py
--rw-r--r--   0        0        0    12989 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/feeds.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/flat_slug.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/generator.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/glob.py
--rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/heading_link.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/icon_resize.py
--rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/jinja_md.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/load.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/manifest.py
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/md_it_highlight_code.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/md_it_wikilinks.py
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/mdit_details.py
--rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/post_template.py
--rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/prevnext.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/prevnext_template.html
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/publish_dev_to_source.py
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/publish_html.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/publish_source.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/pyinstrument.py
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/redirects.py
--rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/render_markdown.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/rss.py
--rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/seo.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/service_worker.py
--rw-r--r--   0        0        0     6580 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/setup_logging.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/sitemap.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/subroute.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/to_json.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/plugins/tui.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/markata/scripts/migrate_to_slugify.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/static/_redirects
--rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/static/favicon.ico
--rw-r--r--   0        0        0    52806 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/static/markata.dev_.webp
--rw-r--r--   0        0        0    37044 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/static/markata.dev_markata_plugins_base-cli_.webp
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/static/robots.txt
--rw-r--r--   0        0        0    63534 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/static/waylonwalker.com.webp
--rw-r--r--   0        0        0    77848 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/static/waylonwalker.com_archive.webp
--rw-r--r--   0        0        0    41986 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/static/waylonwalker.com_markata-configure-head.webp
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/tests/test_doc_page.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/tests/test_feeds.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/tests/test_one_default_page.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/tests/test_one_default_page_with_path_prefix.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/tests/plugins/conftest.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/tests/plugins/test_default_post_template.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/tests/plugins/test_flat_slug.py
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/tests/plugins/test_redirects.py
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/LICENSE
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/README.md
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/pyproject.toml
--rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 markata-0.7.0.dev5/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.markataignore
+-rw-r--r--   0        0        0    17519 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/CHANGELOG.md
+-rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/SECURITY.md
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/contributing.md
+-rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata.toml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/18e5fed179aac834
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/1947c9dd163fbab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/1c8c657d31571f2b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/1e6195f0f556a42e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/1fef90e6ba0a501c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/20a63539f8602f82
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/221b1125a61bda8b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/22a18ba7cc9fb850
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/239402204189564e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/2a0c9f9ce28bd115
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/2a74278113d326e4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/2b479232aeec2e0f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/2cf644392d18f778
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/2f4cc97a43f64ad2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/38a44902f99a2b64
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/3fe3f5a578f241c7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/4519367557838479
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/4e4bb1ac8c291212
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/519333a9d3863a62
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/527818f6c7e61ec4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/55692a735d162b5b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/55a0b11a5a1a43c6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/570e609cc55f9e8a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/6032cab98234c712
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/606c5b624b26f73
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/63bd291162e5ad77
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/6da20bcb740f5bfb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/6f6d6797263b7a2a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/7993652b3f669c06
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/7b8163ab0e203fef
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/813642e0473afef8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/84bc728e6f77eb53
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/8706cfb90ba2ba6e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/8cda362e601dc1c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/9e4a574b76d331e4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/a7dcadf5d2b721ad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/ae7e5c7addcf2938
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/b14e99dc43135fb7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/b9298e40379614c4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/c4f6eb4619bcd5dc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/cd63ed8c48765d61
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/cf3ed4a895962fb2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/cf91dee4aad1ddec
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/d95eea7afa795f01
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/d9be4185f8f397f2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/d9d0bf889fa7baf1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/e9220d130f9a4f9f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/ed74b3ea99c7de8b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/eeb31b4beff77af5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/f3951464a78fe60a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/f662d283a302c99b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/fb2cd83781512729
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/fe3ada26eb2fe4a5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.ruff_cache/content/fee8cb9fe8378525
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/docs/404.md
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/docs/color-theme.md
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/docs/home-page.md
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/docs/index.md
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/docs/nav.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/docs/project-gallery/markata_dev.md
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/docs/project-gallery/waylonwalker.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/__about__.py
+-rw-r--r--   0        0        0    15949 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/__main__.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/background.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/errors.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/hookspec.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/lifecycle.py
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/standard_config.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/cli/__init__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/cli/__main__.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/cli/cli.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/cli/header.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/cli/plugins.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/cli/runner.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/cli/server.py
+-rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/cli/summary.py
+-rw-r--r--   0        0        0    38304 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/Karla-Regular.ttf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/__init__.py
+-rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/auto_description.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/auto_title.py
+-rw-r--r--   0        0        0    17051 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/base_cli.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/copy_assets.py
+-rw-r--r--   0        0        0     7472 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/covers.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/create_covers.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/datetime.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/default_doc_template.md
+-rw-r--r--   0        0        0    13176 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/default_log_template.html
+-rw-r--r--   0        0        0    21666 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/default_post_template.html
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/default_redirect_template.html
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/default_service_worker_template.js
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/docs.py
+-rw-r--r--   0        0        0    12989 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/feeds.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/flat_slug.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/generator.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/glob.py
+-rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/heading_link.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/icon_resize.py
+-rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/jinja_md.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/load.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/manifest.py
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/md_it_highlight_code.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/md_it_wikilinks.py
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/mdit_details.py
+-rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/post_template.py
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/prevnext.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/prevnext_template.html
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/publish_dev_to_source.py
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/publish_html.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/publish_source.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/pyinstrument.py
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/redirects.py
+-rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/render_markdown.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/rss.py
+-rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/seo.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/service_worker.py
+-rw-r--r--   0        0        0     6580 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/setup_logging.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/sitemap.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/subroute.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/to_json.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/plugins/tui.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/markata/scripts/migrate_to_slugify.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/static/_redirects
+-rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/static/favicon.ico
+-rw-r--r--   0        0        0    52806 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/static/markata.dev_.webp
+-rw-r--r--   0        0        0    37044 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/static/markata.dev_markata_plugins_base-cli_.webp
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/static/robots.txt
+-rw-r--r--   0        0        0    63534 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/static/waylonwalker.com.webp
+-rw-r--r--   0        0        0    77848 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/static/waylonwalker.com_archive.webp
+-rw-r--r--   0        0        0    41986 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/static/waylonwalker.com_markata-configure-head.webp
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/tests/test_doc_page.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/tests/test_feeds.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/tests/test_one_default_page.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/tests/test_one_default_page_with_path_prefix.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/tests/plugins/conftest.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/tests/plugins/test_default_post_template.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/tests/plugins/test_flat_slug.py
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/tests/plugins/test_redirects.py
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/LICENSE
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/README.md
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/pyproject.toml
+-rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 markata-0.7.0.dev6/PKG-INFO
```

### Comparing `markata-0.7.0.dev5/CHANGELOG.md` & `markata-0.7.0.dev6/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 # Markata Changelog
 
 ## 0.7.0
 
 - Adopt ruff linter 0.7.0.dev1 #142
+- add trogon tui support 0.7.0.dev0
+
+### trogon tui support
+
+install with pip
+
+```bash
+pip install 'markata[tui]'
+```
+
+usage
+
+```bash
+markata tui
+```
 
 ## 0.6.1
 
 - Fix: allow feeds to be used from within markdown
 
 ### Feeds in markdown
```

### Comparing `markata-0.7.0.dev5/CODE_OF_CONDUCT.md` & `markata-0.7.0.dev6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/contributing.md` & `markata-0.7.0.dev6/contributing.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata.toml` & `markata-0.7.0.dev6/markata.toml`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/docs/color-theme.md` & `markata-0.7.0.dev6/docs/color-theme.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/docs/home-page.md` & `markata-0.7.0.dev6/docs/home-page.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/docs/index.md` & `markata-0.7.0.dev6/docs/index.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/docs/nav.md` & `markata-0.7.0.dev6/docs/nav.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/docs/project-gallery/markata_dev.md` & `markata-0.7.0.dev6/docs/project-gallery/markata_dev.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/docs/project-gallery/waylonwalker.md` & `markata-0.7.0.dev6/docs/project-gallery/waylonwalker.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/__init__.py` & `markata-0.7.0.dev6/markata/__init__.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/background.py` & `markata-0.7.0.dev6/markata/background.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/hookspec.py` & `markata-0.7.0.dev6/markata/hookspec.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/lifecycle.py` & `markata-0.7.0.dev6/markata/lifecycle.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/standard_config.py` & `markata-0.7.0.dev6/markata/standard_config.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/cli/__main__.py` & `markata-0.7.0.dev6/markata/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/cli/cli.py` & `markata-0.7.0.dev6/markata/cli/cli.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/cli/plugins.py` & `markata-0.7.0.dev6/markata/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/cli/runner.py` & `markata-0.7.0.dev6/markata/cli/runner.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/cli/server.py` & `markata-0.7.0.dev6/markata/cli/server.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/cli/summary.py` & `markata-0.7.0.dev6/markata/cli/summary.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/Karla-Regular.ttf` & `markata-0.7.0.dev6/markata/plugins/Karla-Regular.ttf`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/auto_description.py` & `markata-0.7.0.dev6/markata/plugins/auto_description.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/base_cli.py` & `markata-0.7.0.dev6/markata/plugins/base_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,14 +124,28 @@
     """
     Markata hook to implement base cli commands.
     """
 
     plugins_app = typer.Typer()
     app.add_typer(plugins_app)
 
+    @app.command()
+    def tui(ctx: typer.Context) -> None:
+        try:
+            from trogon import Trogon
+            from typer.main import get_group
+        except ImportError:
+            typer.echo("trogon not installed")
+            typer.echo(
+                "install markata with optional tui group to use tui `pip install 'markata[tui]'`"
+            )
+            return
+
+        Trogon(get_group(app), click_context=ctx).run()
+
     @plugins_app.callback()
     def plugins():
         "create new things from templates"
 
     @plugins_app.command()
     def show() -> None:
         rich_print(markata.plugins)
```

### Comparing `markata-0.7.0.dev5/markata/plugins/copy_assets.py` & `markata-0.7.0.dev6/markata/plugins/copy_assets.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/covers.py` & `markata-0.7.0.dev6/markata/plugins/covers.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/create_covers.py` & `markata-0.7.0.dev6/markata/plugins/create_covers.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/datetime.py` & `markata-0.7.0.dev6/markata/plugins/datetime.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/default_doc_template.md` & `markata-0.7.0.dev6/markata/plugins/default_doc_template.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/default_log_template.html` & `markata-0.7.0.dev6/markata/plugins/default_log_template.html`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/default_post_template.html` & `markata-0.7.0.dev6/markata/plugins/default_post_template.html`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/default_redirect_template.html` & `markata-0.7.0.dev6/markata/plugins/default_redirect_template.html`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/default_service_worker_template.js` & `markata-0.7.0.dev6/markata/plugins/default_service_worker_template.js`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/docs.py` & `markata-0.7.0.dev6/markata/plugins/docs.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/feeds.py` & `markata-0.7.0.dev6/markata/plugins/feeds.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/flat_slug.py` & `markata-0.7.0.dev6/markata/plugins/flat_slug.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/generator.py` & `markata-0.7.0.dev6/markata/plugins/generator.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/glob.py` & `markata-0.7.0.dev6/markata/plugins/glob.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/heading_link.py` & `markata-0.7.0.dev6/markata/plugins/heading_link.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/icon_resize.py` & `markata-0.7.0.dev6/markata/plugins/icon_resize.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/jinja_md.py` & `markata-0.7.0.dev6/markata/plugins/jinja_md.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/load.py` & `markata-0.7.0.dev6/markata/plugins/load.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/manifest.py` & `markata-0.7.0.dev6/markata/plugins/manifest.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/md_it_highlight_code.py` & `markata-0.7.0.dev6/markata/plugins/md_it_highlight_code.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/md_it_wikilinks.py` & `markata-0.7.0.dev6/markata/plugins/md_it_wikilinks.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/mdit_details.py` & `markata-0.7.0.dev6/markata/plugins/mdit_details.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/post_template.py` & `markata-0.7.0.dev6/markata/plugins/post_template.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/prevnext.py` & `markata-0.7.0.dev6/markata/plugins/prevnext.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/prevnext_template.html` & `markata-0.7.0.dev6/markata/plugins/prevnext_template.html`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/publish_dev_to_source.py` & `markata-0.7.0.dev6/markata/plugins/publish_dev_to_source.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/publish_html.py` & `markata-0.7.0.dev6/markata/plugins/publish_html.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/publish_source.py` & `markata-0.7.0.dev6/markata/plugins/publish_source.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/pyinstrument.py` & `markata-0.7.0.dev6/markata/plugins/pyinstrument.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/redirects.py` & `markata-0.7.0.dev6/markata/plugins/redirects.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/render_markdown.py` & `markata-0.7.0.dev6/markata/plugins/render_markdown.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/rss.py` & `markata-0.7.0.dev6/markata/plugins/rss.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/seo.py` & `markata-0.7.0.dev6/markata/plugins/seo.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/service_worker.py` & `markata-0.7.0.dev6/markata/plugins/service_worker.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/setup_logging.py` & `markata-0.7.0.dev6/markata/plugins/setup_logging.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/sitemap.py` & `markata-0.7.0.dev6/markata/plugins/sitemap.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/subroute.py` & `markata-0.7.0.dev6/markata/plugins/subroute.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/markata/plugins/tui.py` & `markata-0.7.0.dev6/markata/plugins/tui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,68 @@
 import subprocess
 
 from rich.console import RenderableType
-from textual.app import App
-from textual.widget import Widget
-from textual.widgets import Footer
 
 from markata import Markata
 from markata.hookspec import hook_impl
 
+try:
+    from textual.app import App
+    from textual.widget import Widget
+    from textual.widgets import Footer
+
+    class MarkataWidget(Widget):
+        def __init__(self, markata: Markata, widget: str = "server"):
+            super().__init__(widget)
+            self.m = markata
+            self.widget = widget
+            self.renderable = getattr(self.m, self.widget)
+
+        def render(self):
+            return self.renderable
+
+        async def update(self, renderable: RenderableType) -> None:
+            self.renderable = renderable
+            self.refresh()
+
+    class MarkataApp(App):
+        async def on_load(self, event):
+            self.m = Markata()
+            self.m.console.quiet = True
+            await self.bind("q", "quit", "quit")
+            await self.bind("r", "refresh", "refresh")
+            self.new_cmd = self.m.config.get("tui", {}).get("new_cmd", "")
+            if self.new_cmd != "":
+                await self.bind("n", "new", "new")
+
+        async def on_mount(self) -> None:
+            self.server = MarkataWidget(self.m, "server")
+            self.runner = MarkataWidget(self.m, "runner")
+            self.plugins = MarkataWidget(self.m, "plugins")
+            self.summary = MarkataWidget(self.m, "summary")
+            await self.view.dock(Footer(), edge="bottom")
+            await self.view.dock(self.plugins, edge="left", size=30, name="plugins")
+            await self.view.dock(self.summary, edge="right", size=30, name="summary")
+            await self.view.dock(self.server, self.runner, edge="top")
+            self.set_interval(1, self.action_refresh)
+
+        async def action_refresh(self) -> None:
+            self.refresh()
+            self.runner.refresh()
+            self.server.refresh()
+            self.plugins.refresh()
+            self.summary.refresh()
+
+        async def action_new(self) -> None:
+            subprocess.Popen(
+                self.new_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE
+            )
 
-class MarkataWidget(Widget):
-    def __init__(self, markata: Markata, widget: str = "server"):
-        super().__init__(widget)
-        self.m = markata
-        self.widget = widget
-        self.renderable = getattr(self.m, self.widget)
-
-    def render(self):
-        return self.renderable
-
-    async def update(self, renderable: RenderableType) -> None:
-        self.renderable = renderable
-        self.refresh()
-
-
-class MarkataApp(App):
-    async def on_load(self, event):
-        self.m = Markata()
-        self.m.console.quiet = True
-        await self.bind("q", "quit", "quit")
-        await self.bind("r", "refresh", "refresh")
-        self.new_cmd = self.m.config.get("tui", {}).get("new_cmd", "")
-        if self.new_cmd != "":
-            await self.bind("n", "new", "new")
-
-    async def on_mount(self) -> None:
-        self.server = MarkataWidget(self.m, "server")
-        self.runner = MarkataWidget(self.m, "runner")
-        self.plugins = MarkataWidget(self.m, "plugins")
-        self.summary = MarkataWidget(self.m, "summary")
-        await self.view.dock(Footer(), edge="bottom")
-        await self.view.dock(self.plugins, edge="left", size=30, name="plugins")
-        await self.view.dock(self.summary, edge="right", size=30, name="summary")
-        await self.view.dock(self.server, self.runner, edge="top")
-        self.set_interval(1, self.action_refresh)
-
-    async def action_refresh(self) -> None:
-        self.refresh()
-        self.runner.refresh()
-        self.server.refresh()
-        self.plugins.refresh()
-        self.summary.refresh()
-
-    async def action_new(self) -> None:
-        subprocess.Popen(self.new_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+except ImportError:
+    ...
 
 
 @hook_impl()
 def cli(app, markata):
     @app.command()
     def tui():
         MarkataApp.run(log="textual.log")
```

### Comparing `markata-0.7.0.dev5/markata/scripts/migrate_to_slugify.py` & `markata-0.7.0.dev6/markata/scripts/migrate_to_slugify.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/static/_redirects` & `markata-0.7.0.dev6/static/_redirects`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/static/favicon.ico` & `markata-0.7.0.dev6/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/static/markata.dev_.webp` & `markata-0.7.0.dev6/static/markata.dev_.webp`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/static/markata.dev_markata_plugins_base-cli_.webp` & `markata-0.7.0.dev6/static/markata.dev_markata_plugins_base-cli_.webp`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/static/waylonwalker.com.webp` & `markata-0.7.0.dev6/static/waylonwalker.com.webp`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/static/waylonwalker.com_archive.webp` & `markata-0.7.0.dev6/static/waylonwalker.com_archive.webp`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/static/waylonwalker.com_markata-configure-head.webp` & `markata-0.7.0.dev6/static/waylonwalker.com_markata-configure-head.webp`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/tests/test_doc_page.py` & `markata-0.7.0.dev6/tests/test_doc_page.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/tests/test_feeds.py` & `markata-0.7.0.dev6/tests/test_feeds.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/tests/test_one_default_page.py` & `markata-0.7.0.dev6/tests/test_one_default_page.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/tests/test_one_default_page_with_path_prefix.py` & `markata-0.7.0.dev6/tests/test_one_default_page_with_path_prefix.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/tests/plugins/test_default_post_template.py` & `markata-0.7.0.dev6/tests/plugins/test_default_post_template.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/tests/plugins/test_flat_slug.py` & `markata-0.7.0.dev6/tests/plugins/test_flat_slug.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/tests/plugins/test_redirects.py` & `markata-0.7.0.dev6/tests/plugins/test_redirects.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/.gitignore` & `markata-0.7.0.dev6/.gitignore`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev5/LICENSE` & `markata-0.7.0.dev6/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-Copyright (c) 2012-2022 Waylon Walker
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining
-a copy of this software and associated documentation files (the
-"Software"), to deal in the Software without restriction, including
-without limitation the rights to use, copy, modify, merge, publish,
-distribute, sublicense, and/or sell copies of the Software, and to
-permit persons to whom the Software is furnished to do so, subject to
-the following conditions:
+Copyright (c) 2021-present Waylon S. Walker <waylon@waylonwalker.com>
 
-The above copyright notice and this permission notice shall be
-included in all copies or substantial portions of the Software.
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions:
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
-LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
-WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `markata-0.7.0.dev5/README.md` & `markata-0.7.0.dev6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -5,26 +5,40 @@
 
 <p align=center>
   <em>
     Markdown to site, plugins all the way down
   </em>
 </p>
 
+## Coming soon
+
+pydantic all the things.  All post objects and config will become pydantic objects.  This will allow for validation to happen early, and referencing post attributes or config, it can be assumed that they exist whether they were explicitly created or cohersed to their defaults early in the build.
+
+---
+
 A static site generator that will give you a great site with many standard web
 features like rss, sitemaps, and seo tags, out of the box. Running `markata
 build` will get you a that only requires you to write Markdown. If you have
 additional features that you want, don't worry, since markata is built
 completely on plugins you can develop and install your own plugins to add the
 features you want.
 
 ## QuickStart
 
 Markata is fully configurable through a `markata.toml` file, but the defaults
 allow to build your site right out of the box with nothing more than Markdown.
 
+### Installation
+
+`markata` is hosted on pypi and can be installed using pip.
+
+```bash
+python -m pip install markata
+```
+
 ### Create Some Content
 
 Make some `.md` files in your current working directory. By default, `markata`
 will recursively look in all subdirectories for markdown files `**/*.md`.
 
 ```bash
 mkdir pages
@@ -42,15 +56,15 @@
 python -m pip install markata
 markata build
 
 # or if pipx is your thing
 pipx run markata build
 ```
 
-### Building a Blog with Markata
+### Building a Blog with Markata _using a template_
 
 The markata cli includes a `new` command that will present you with questions
 to fill in the jinja variables in this repo.
 
 ```bash
 markata new blog [directory]
```

#### html2text {}

```diff
@@ -1,37 +1,43 @@
                                     ******
                                [Markata] ******
                   Markdown to site, plugins all the way down
-A static site generator that will give you a great site with many standard web
-features like rss, sitemaps, and seo tags, out of the box. Running `markata
-build` will get you a that only requires you to write Markdown. If you have
-additional features that you want, don't worry, since markata is built
+## Coming soon pydantic all the things. All post objects and config will become
+pydantic objects. This will allow for validation to happen early, and
+referencing post attributes or config, it can be assumed that they exist
+whether they were explicitly created or cohersed to their defaults early in the
+build. --- A static site generator that will give you a great site with many
+standard web features like rss, sitemaps, and seo tags, out of the box. Running
+`markata build` will get you a that only requires you to write Markdown. If you
+have additional features that you want, don't worry, since markata is built
 completely on plugins you can develop and install your own plugins to add the
 features you want. ## QuickStart Markata is fully configurable through a
 `markata.toml` file, but the defaults allow to build your site right out of the
-box with nothing more than Markdown. ### Create Some Content Make some `.md`
-files in your current working directory. By default, `markata` will recursively
-look in all subdirectories for markdown files `**/*.md`. ```bash mkdir pages
-echo '# My First Post' > first-post.md echo '# Hello World' > hello-world.md
-``` ### Build your site Install markata into your virtual environment and run
-`markata build`. It will create your site in `./markout`, leave its cache in
-`./.markata.cache`, and copy all assets from `./static` into `./markout` by
-default. ```bash python -m pip install markata markata build # or if pipx is
-your thing pipx run markata build ``` ### Building a Blog with Markata The
-markata cli includes a `new` command that will present you with questions to
-fill in the jinja variables in this repo. ```bash markata new blog [directory]
-# start the site and watch for changes hatch run tui ``` Now if you open
-localhost:8000, you will be presented with an example site that will walk you
-through some features of markata. You can play with it at your own pace, or
-drop all the pages and start writing your own content. ## Motivation Markata is
-able to build your site purely from Markdown, allowing you to get started
-creating your own content quickly. Out of the box it will cover your seo tags,
-rss feeds, sitemap, and og images. Since it is built completely from plugins
-you can remove, modify, or add to any of its behavior. - configurable - plugins
-- seo - rss - sitemap - og-image ## Using Markata The docs are still a work in
+box with nothing more than Markdown. ### Installation `markata` is hosted on
+pypi and can be installed using pip. ```bash python -m pip install markata ```
+### Create Some Content Make some `.md` files in your current working
+directory. By default, `markata` will recursively look in all subdirectories
+for markdown files `**/*.md`. ```bash mkdir pages echo '# My First Post' >
+first-post.md echo '# Hello World' > hello-world.md ``` ### Build your site
+Install markata into your virtual environment and run `markata build`. It will
+create your site in `./markout`, leave its cache in `./.markata.cache`, and
+copy all assets from `./static` into `./markout` by default. ```bash python -
+m pip install markata markata build # or if pipx is your thing pipx run markata
+build ``` ### Building a Blog with Markata _using a template_ The markata cli
+includes a `new` command that will present you with questions to fill in the
+jinja variables in this repo. ```bash markata new blog [directory] # start the
+site and watch for changes hatch run tui ``` Now if you open localhost:8000,
+you will be presented with an example site that will walk you through some
+features of markata. You can play with it at your own pace, or drop all the
+pages and start writing your own content. ## Motivation Markata is able to
+build your site purely from Markdown, allowing you to get started creating your
+own content quickly. Out of the box it will cover your seo tags, rss feeds,
+sitemap, and og images. Since it is built completely from plugins you can
+remove, modify, or add to any of its behavior. - configurable - plugins - seo -
+rss - sitemap - og-image ## Using Markata The docs are still a work in
 progress, but the [base_cli](https://markata.dev/markata/plugins/base_cli/
 ) walks through how to effectively use the `markata build` command. At this
 point Markata is far from stable and **will change quite a bit**, should you
 choose to use it on real site make sure you pin to the version that you want to
 build from. I will let you know as it becomes more stable and ready to use
 without diligence of pinning to the version you want. **Honestly** A big
 motivation for me was wanting to learn and understand how to create a project
```

### Comparing `markata-0.7.0.dev5/pyproject.toml` & `markata-0.7.0.dev6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [project]
 classifiers = [
  "Development Status :: 4 - Beta",
  "Environment :: Console",
  "Environment :: Web Environment",
  "Intended Audience :: Developers",
+ "License :: OSI Approved :: MIT License",
  "Natural Language :: English",
  "Operating System :: OS Independent",
  "Programming Language :: Python :: 3 :: Only",
  "Programming Language :: Python :: 3",
  "Programming Language :: Python :: 3.7",
  "Programming Language :: Python :: 3.8",
  "Programming Language :: Python :: 3.9",
@@ -21,14 +22,15 @@
  "Topic :: Text Processing",
  "Typing :: Typed",
 ]
 dependencies = [
  "anyconfig",
  "beautifulsoup4",
  "checksumdir",
+ "commonmark",
  "cookiecutter",
  "copier",
  "deepmerge",
  "diskcache",
  "feedgen",
  "jinja2",
  "linkify-it-py",
@@ -39,28 +41,29 @@
  "pillow",
  "pluggy",
  "pymdown-extensions",
  "python-frontmatter",
  "python-slugify",
  "pytz",
  "rich",
- "textual<0.2.0",
  "toml",
  "typer",
 ]
+
 dynamic = [
  "version",
 ]
 description = "Static site generator plugins all the way down."
 keywords = [
  "static-site",
 ]
 name = "markata"
 readme = "README.md"
 requires-python = ">=3.6"
+
 [[project.authors]]
 name = "Waylon Walker"
 email = "waylon@waylonwalker.com"
 
 [[project.authors]]
 email = "waylon@markata.dev"
 
@@ -70,14 +73,18 @@
 ]
 build-backend = "hatchling.build"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
+tui = [
+  "textual",
+  "trogon",
+]
 dev = [
  "black==22.10.0",
  "hatch",
  "interrogate",
  "mypy",
  "pre-commit",
  "pytest",
```

### Comparing `markata-0.7.0.dev5/PKG-INFO` & `markata-0.7.0.dev6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d61 726b  : 2.1.Name: mark
 00000020: 6174 610a 5665 7273 696f 6e3a 2030 2e37  ata.Version: 0.7
-00000030: 2e30 2e64 6576 350a 5375 6d6d 6172 793a  .0.dev5.Summary:
+00000030: 2e30 2e64 6576 360a 5375 6d6d 6172 793a  .0.dev6.Summary:
 00000040: 2053 7461 7469 6320 7369 7465 2067 656e   Static site gen
 00000050: 6572 6174 6f72 2070 6c75 6769 6e73 2061  erator plugins a
 00000060: 6c6c 2074 6865 2077 6179 2064 6f77 6e2e  ll the way down.
 00000070: 0a50 726f 6a65 6374 2d55 524c 3a20 486f  .Project-URL: Ho
 00000080: 6d65 7061 6765 2c20 6874 7470 733a 2f2f  mepage, https://
 00000090: 6d61 726b 6174 612e 6465 760a 5072 6f6a  markata.dev.Proj
 000000a0: 6563 742d 5552 4c3a 2043 6861 6e67 656c  ect-URL: Changel
@@ -23,428 +23,469 @@
 00000160: 2044 6f63 756d 656e 7461 7469 6f6e 2c20   Documentation, 
 00000170: 6874 7470 733a 2f2f 6d61 726b 6174 612e  https://markata.
 00000180: 6465 760a 4175 7468 6f72 2d65 6d61 696c  dev.Author-email
 00000190: 3a20 5761 796c 6f6e 2057 616c 6b65 7220  : Waylon Walker 
 000001a0: 3c77 6179 6c6f 6e40 7761 796c 6f6e 7761  <waylon@waylonwa
 000001b0: 6c6b 6572 2e63 6f6d 3e2c 2077 6179 6c6f  lker.com>, waylo
 000001c0: 6e40 6d61 726b 6174 612e 6465 760a 4c69  n@markata.dev.Li
-000001d0: 6365 6e73 653a 2043 6f70 7972 6967 6874  cense: Copyright
-000001e0: 2028 6329 2032 3031 322d 3230 3232 2057   (c) 2012-2022 W
-000001f0: 6179 6c6f 6e20 5761 6c6b 6572 0a20 2020  aylon Walker.   
-00000200: 2020 2020 200a 2020 2020 2020 2020 5065       .        Pe
-00000210: 726d 6973 7369 6f6e 2069 7320 6865 7265  rmission is here
-00000220: 6279 2067 7261 6e74 6564 2c20 6672 6565  by granted, free
-00000230: 206f 6620 6368 6172 6765 2c20 746f 2061   of charge, to a
-00000240: 6e79 2070 6572 736f 6e20 6f62 7461 696e  ny person obtain
-00000250: 696e 670a 2020 2020 2020 2020 6120 636f  ing.        a co
-00000260: 7079 206f 6620 7468 6973 2073 6f66 7477  py of this softw
-00000270: 6172 6520 616e 6420 6173 736f 6369 6174  are and associat
-00000280: 6564 2064 6f63 756d 656e 7461 7469 6f6e  ed documentation
-00000290: 2066 696c 6573 2028 7468 650a 2020 2020   files (the.    
-000002a0: 2020 2020 2253 6f66 7477 6172 6522 292c      "Software"),
-000002b0: 2074 6f20 6465 616c 2069 6e20 7468 6520   to deal in the 
-000002c0: 536f 6674 7761 7265 2077 6974 686f 7574  Software without
-000002d0: 2072 6573 7472 6963 7469 6f6e 2c20 696e   restriction, in
-000002e0: 636c 7564 696e 670a 2020 2020 2020 2020  cluding.        
-000002f0: 7769 7468 6f75 7420 6c69 6d69 7461 7469  without limitati
-00000300: 6f6e 2074 6865 2072 6967 6874 7320 746f  on the rights to
-00000310: 2075 7365 2c20 636f 7079 2c20 6d6f 6469   use, copy, modi
-00000320: 6679 2c20 6d65 7267 652c 2070 7562 6c69  fy, merge, publi
-00000330: 7368 2c0a 2020 2020 2020 2020 6469 7374  sh,.        dist
-00000340: 7269 6275 7465 2c20 7375 626c 6963 656e  ribute, sublicen
-00000350: 7365 2c20 616e 642f 6f72 2073 656c 6c20  se, and/or sell 
-00000360: 636f 7069 6573 206f 6620 7468 6520 536f  copies of the So
-00000370: 6674 7761 7265 2c20 616e 6420 746f 0a20  ftware, and to. 
-00000380: 2020 2020 2020 2070 6572 6d69 7420 7065         permit pe
-00000390: 7273 6f6e 7320 746f 2077 686f 6d20 7468  rsons to whom th
-000003a0: 6520 536f 6674 7761 7265 2069 7320 6675  e Software is fu
-000003b0: 726e 6973 6865 6420 746f 2064 6f20 736f  rnished to do so
-000003c0: 2c20 7375 626a 6563 7420 746f 0a20 2020  , subject to.   
-000003d0: 2020 2020 2074 6865 2066 6f6c 6c6f 7769       the followi
-000003e0: 6e67 2063 6f6e 6469 7469 6f6e 733a 0a20  ng conditions:. 
-000003f0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000400: 5468 6520 6162 6f76 6520 636f 7079 7269  The above copyri
-00000410: 6768 7420 6e6f 7469 6365 2061 6e64 2074  ght notice and t
-00000420: 6869 7320 7065 726d 6973 7369 6f6e 206e  his permission n
-00000430: 6f74 6963 6520 7368 616c 6c20 6265 0a20  otice shall be. 
-00000440: 2020 2020 2020 2069 6e63 6c75 6465 6420         included 
-00000450: 696e 2061 6c6c 2063 6f70 6965 7320 6f72  in all copies or
-00000460: 2073 7562 7374 616e 7469 616c 2070 6f72   substantial por
-00000470: 7469 6f6e 7320 6f66 2074 6865 2053 6f66  tions of the Sof
-00000480: 7477 6172 652e 0a20 2020 2020 2020 200a  tware..        .
-00000490: 2020 2020 2020 2020 5448 4520 534f 4654          THE SOFT
-000004a0: 5741 5245 2049 5320 5052 4f56 4944 4544  WARE IS PROVIDED
-000004b0: 2022 4153 2049 5322 2c20 5749 5448 4f55   "AS IS", WITHOU
-000004c0: 5420 5741 5252 414e 5459 204f 4620 414e  T WARRANTY OF AN
-000004d0: 5920 4b49 4e44 2c0a 2020 2020 2020 2020  Y KIND,.        
-000004e0: 4558 5052 4553 5320 4f52 2049 4d50 4c49  EXPRESS OR IMPLI
-000004f0: 4544 2c20 494e 434c 5544 494e 4720 4255  ED, INCLUDING BU
-00000500: 5420 4e4f 5420 4c49 4d49 5445 4420 544f  T NOT LIMITED TO
-00000510: 2054 4845 2057 4152 5241 4e54 4945 5320   THE WARRANTIES 
-00000520: 4f46 0a20 2020 2020 2020 204d 4552 4348  OF.        MERCH
-00000530: 414e 5441 4249 4c49 5459 2c20 4649 544e  ANTABILITY, FITN
-00000540: 4553 5320 464f 5220 4120 5041 5254 4943  ESS FOR A PARTIC
-00000550: 554c 4152 2050 5552 504f 5345 2041 4e44  ULAR PURPOSE AND
-00000560: 0a20 2020 2020 2020 204e 4f4e 494e 4652  .        NONINFR
-00000570: 494e 4745 4d45 4e54 2e20 494e 204e 4f20  INGEMENT. IN NO 
-00000580: 4556 454e 5420 5348 414c 4c20 5448 4520  EVENT SHALL THE 
-00000590: 4155 5448 4f52 5320 4f52 2043 4f50 5952  AUTHORS OR COPYR
-000005a0: 4947 4854 2048 4f4c 4445 5253 2042 450a  IGHT HOLDERS BE.
-000005b0: 2020 2020 2020 2020 4c49 4142 4c45 2046          LIABLE F
-000005c0: 4f52 2041 4e59 2043 4c41 494d 2c20 4441  OR ANY CLAIM, DA
-000005d0: 4d41 4745 5320 4f52 204f 5448 4552 204c  MAGES OR OTHER L
-000005e0: 4941 4249 4c49 5459 2c20 5748 4554 4845  IABILITY, WHETHE
-000005f0: 5220 494e 2041 4e20 4143 5449 4f4e 0a20  R IN AN ACTION. 
-00000600: 2020 2020 2020 204f 4620 434f 4e54 5241         OF CONTRA
-00000610: 4354 2c20 544f 5254 204f 5220 4f54 4845  CT, TORT OR OTHE
-00000620: 5257 4953 452c 2041 5249 5349 4e47 2046  RWISE, ARISING F
-00000630: 524f 4d2c 204f 5554 204f 4620 4f52 2049  ROM, OUT OF OR I
-00000640: 4e20 434f 4e4e 4543 5449 4f4e 0a20 2020  N CONNECTION.   
-00000650: 2020 2020 2057 4954 4820 5448 4520 534f       WITH THE SO
-00000660: 4654 5741 5245 204f 5220 5448 4520 5553  FTWARE OR THE US
-00000670: 4520 4f52 204f 5448 4552 2044 4541 4c49  E OR OTHER DEALI
-00000680: 4e47 5320 494e 2054 4845 2053 4f46 5457  NGS IN THE SOFTW
-00000690: 4152 452e 0a4c 6963 656e 7365 2d46 696c  ARE..License-Fil
-000006a0: 653a 204c 4943 454e 5345 0a4b 6579 776f  e: LICENSE.Keywo
-000006b0: 7264 733a 2073 7461 7469 632d 7369 7465  rds: static-site
-000006c0: 0a43 6c61 7373 6966 6965 723a 2044 6576  .Classifier: Dev
-000006d0: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
-000006e0: 3a3a 2034 202d 2042 6574 610a 436c 6173  :: 4 - Beta.Clas
-000006f0: 7369 6669 6572 3a20 456e 7669 726f 6e6d  sifier: Environm
-00000700: 656e 7420 3a3a 2043 6f6e 736f 6c65 0a43  ent :: Console.C
-00000710: 6c61 7373 6966 6965 723a 2045 6e76 6972  lassifier: Envir
-00000720: 6f6e 6d65 6e74 203a 3a20 5765 6220 456e  onment :: Web En
-00000730: 7669 726f 6e6d 656e 740a 436c 6173 7369  vironment.Classi
-00000740: 6669 6572 3a20 496e 7465 6e64 6564 2041  fier: Intended A
-00000750: 7564 6965 6e63 6520 3a3a 2044 6576 656c  udience :: Devel
-00000760: 6f70 6572 730a 436c 6173 7369 6669 6572  opers.Classifier
-00000770: 3a20 4e61 7475 7261 6c20 4c61 6e67 7561  : Natural Langua
-00000780: 6765 203a 3a20 456e 676c 6973 680a 436c  ge :: English.Cl
-00000790: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
-000007a0: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
-000007b0: 2049 6e64 6570 656e 6465 6e74 0a43 6c61   Independent.Cla
-000007c0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-000007d0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000007e0: 2050 7974 686f 6e0a 436c 6173 7369 6669   Python.Classifi
-000007f0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-00000800: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000810: 6f6e 203a 3a20 330a 436c 6173 7369 6669  on :: 3.Classifi
-00000820: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-00000830: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000840: 6f6e 203a 3a20 3320 3a3a 204f 6e6c 790a  on :: 3 :: Only.
+000001d0: 6365 6e73 653a 204d 4954 204c 6963 656e  cense: MIT Licen
+000001e0: 7365 0a20 2020 2020 2020 200a 2020 2020  se.        .    
+000001f0: 2020 2020 436f 7079 7269 6768 7420 2863      Copyright (c
+00000200: 2920 3230 3231 2d70 7265 7365 6e74 2057  ) 2021-present W
+00000210: 6179 6c6f 6e20 532e 2057 616c 6b65 7220  aylon S. Walker 
+00000220: 3c77 6179 6c6f 6e40 7761 796c 6f6e 7761  <waylon@waylonwa
+00000230: 6c6b 6572 2e63 6f6d 3e0a 2020 2020 2020  lker.com>.      
+00000240: 2020 0a20 2020 2020 2020 2050 6572 6d69    .        Permi
+00000250: 7373 696f 6e20 6973 2068 6572 6562 7920  ssion is hereby 
+00000260: 6772 616e 7465 642c 2066 7265 6520 6f66  granted, free of
+00000270: 2063 6861 7267 652c 2074 6f20 616e 7920   charge, to any 
+00000280: 7065 7273 6f6e 206f 6274 6169 6e69 6e67  person obtaining
+00000290: 2061 2063 6f70 7920 6f66 0a20 2020 2020   a copy of.     
+000002a0: 2020 2074 6869 7320 736f 6674 7761 7265     this software
+000002b0: 2061 6e64 2061 7373 6f63 6961 7465 6420   and associated 
+000002c0: 646f 6375 6d65 6e74 6174 696f 6e20 6669  documentation fi
+000002d0: 6c65 7320 2874 6865 2022 536f 6674 7761  les (the "Softwa
+000002e0: 7265 2229 2c20 746f 2064 6561 6c20 696e  re"), to deal in
+000002f0: 0a20 2020 2020 2020 2074 6865 2053 6f66  .        the Sof
+00000300: 7477 6172 6520 7769 7468 6f75 7420 7265  tware without re
+00000310: 7374 7269 6374 696f 6e2c 2069 6e63 6c75  striction, inclu
+00000320: 6469 6e67 2077 6974 686f 7574 206c 696d  ding without lim
+00000330: 6974 6174 696f 6e20 7468 6520 7269 6768  itation the righ
+00000340: 7473 2074 6f0a 2020 2020 2020 2020 7573  ts to.        us
+00000350: 652c 2063 6f70 792c 206d 6f64 6966 792c  e, copy, modify,
+00000360: 206d 6572 6765 2c20 7075 626c 6973 682c   merge, publish,
+00000370: 2064 6973 7472 6962 7574 652c 2073 7562   distribute, sub
+00000380: 6c69 6365 6e73 652c 2061 6e64 2f6f 7220  license, and/or 
+00000390: 7365 6c6c 2063 6f70 6965 730a 2020 2020  sell copies.    
+000003a0: 2020 2020 6f66 2074 6865 2053 6f66 7477      of the Softw
+000003b0: 6172 652c 2061 6e64 2074 6f20 7065 726d  are, and to perm
+000003c0: 6974 2070 6572 736f 6e73 2074 6f20 7768  it persons to wh
+000003d0: 6f6d 2074 6865 2053 6f66 7477 6172 6520  om the Software 
+000003e0: 6973 2066 7572 6e69 7368 6564 2074 6f20  is furnished to 
+000003f0: 646f 0a20 2020 2020 2020 2073 6f2c 2073  do.        so, s
+00000400: 7562 6a65 6374 2074 6f20 7468 6520 666f  ubject to the fo
+00000410: 6c6c 6f77 696e 6720 636f 6e64 6974 696f  llowing conditio
+00000420: 6e73 3a0a 2020 2020 2020 2020 0a20 2020  ns:.        .   
+00000430: 2020 2020 2054 6865 2061 626f 7665 2063       The above c
+00000440: 6f70 7972 6967 6874 206e 6f74 6963 6520  opyright notice 
+00000450: 616e 6420 7468 6973 2070 6572 6d69 7373  and this permiss
+00000460: 696f 6e20 6e6f 7469 6365 2073 6861 6c6c  ion notice shall
+00000470: 2062 6520 696e 636c 7564 6564 2069 6e20   be included in 
+00000480: 616c 6c0a 2020 2020 2020 2020 636f 7069  all.        copi
+00000490: 6573 206f 7220 7375 6273 7461 6e74 6961  es or substantia
+000004a0: 6c20 706f 7274 696f 6e73 206f 6620 7468  l portions of th
+000004b0: 6520 536f 6674 7761 7265 2e0a 2020 2020  e Software..    
+000004c0: 2020 2020 0a20 2020 2020 2020 2054 4845      .        THE
+000004d0: 2053 4f46 5457 4152 4520 4953 2050 524f   SOFTWARE IS PRO
+000004e0: 5649 4445 4420 2241 5320 4953 222c 2057  VIDED "AS IS", W
+000004f0: 4954 484f 5554 2057 4152 5241 4e54 5920  ITHOUT WARRANTY 
+00000500: 4f46 2041 4e59 204b 494e 442c 2045 5850  OF ANY KIND, EXP
+00000510: 5245 5353 204f 520a 2020 2020 2020 2020  RESS OR.        
+00000520: 494d 504c 4945 442c 2049 4e43 4c55 4449  IMPLIED, INCLUDI
+00000530: 4e47 2042 5554 204e 4f54 204c 494d 4954  NG BUT NOT LIMIT
+00000540: 4544 2054 4f20 5448 4520 5741 5252 414e  ED TO THE WARRAN
+00000550: 5449 4553 204f 4620 4d45 5243 4841 4e54  TIES OF MERCHANT
+00000560: 4142 494c 4954 592c 0a20 2020 2020 2020  ABILITY,.       
+00000570: 2046 4954 4e45 5353 2046 4f52 2041 2050   FITNESS FOR A P
+00000580: 4152 5449 4355 4c41 5220 5055 5250 4f53  ARTICULAR PURPOS
+00000590: 4520 414e 4420 4e4f 4e49 4e46 5249 4e47  E AND NONINFRING
+000005a0: 454d 454e 542e 2049 4e20 4e4f 2045 5645  EMENT. IN NO EVE
+000005b0: 4e54 2053 4841 4c4c 2054 4845 0a20 2020  NT SHALL THE.   
+000005c0: 2020 2020 2041 5554 484f 5253 204f 5220       AUTHORS OR 
+000005d0: 434f 5059 5249 4748 5420 484f 4c44 4552  COPYRIGHT HOLDER
+000005e0: 5320 4245 204c 4941 424c 4520 464f 5220  S BE LIABLE FOR 
+000005f0: 414e 5920 434c 4149 4d2c 2044 414d 4147  ANY CLAIM, DAMAG
+00000600: 4553 204f 5220 4f54 4845 520a 2020 2020  ES OR OTHER.    
+00000610: 2020 2020 4c49 4142 494c 4954 592c 2057      LIABILITY, W
+00000620: 4845 5448 4552 2049 4e20 414e 2041 4354  HETHER IN AN ACT
+00000630: 494f 4e20 4f46 2043 4f4e 5452 4143 542c  ION OF CONTRACT,
+00000640: 2054 4f52 5420 4f52 204f 5448 4552 5749   TORT OR OTHERWI
+00000650: 5345 2c20 4152 4953 494e 4720 4652 4f4d  SE, ARISING FROM
+00000660: 2c0a 2020 2020 2020 2020 4f55 5420 4f46  ,.        OUT OF
+00000670: 204f 5220 494e 2043 4f4e 4e45 4354 494f   OR IN CONNECTIO
+00000680: 4e20 5749 5448 2054 4845 2053 4f46 5457  N WITH THE SOFTW
+00000690: 4152 4520 4f52 2054 4845 2055 5345 204f  ARE OR THE USE O
+000006a0: 5220 4f54 4845 5220 4445 414c 494e 4753  R OTHER DEALINGS
+000006b0: 2049 4e20 5448 450a 2020 2020 2020 2020   IN THE.        
+000006c0: 534f 4654 5741 5245 2e0a 4c69 6365 6e73  SOFTWARE..Licens
+000006d0: 652d 4669 6c65 3a20 4c49 4345 4e53 450a  e-File: LICENSE.
+000006e0: 4b65 7977 6f72 6473 3a20 7374 6174 6963  Keywords: static
+000006f0: 2d73 6974 650a 436c 6173 7369 6669 6572  -site.Classifier
+00000700: 3a20 4465 7665 6c6f 706d 656e 7420 5374  : Development St
+00000710: 6174 7573 203a 3a20 3420 2d20 4265 7461  atus :: 4 - Beta
+00000720: 0a43 6c61 7373 6966 6965 723a 2045 6e76  .Classifier: Env
+00000730: 6972 6f6e 6d65 6e74 203a 3a20 436f 6e73  ironment :: Cons
+00000740: 6f6c 650a 436c 6173 7369 6669 6572 3a20  ole.Classifier: 
+00000750: 456e 7669 726f 6e6d 656e 7420 3a3a 2057  Environment :: W
+00000760: 6562 2045 6e76 6972 6f6e 6d65 6e74 0a43  eb Environment.C
+00000770: 6c61 7373 6966 6965 723a 2049 6e74 656e  lassifier: Inten
+00000780: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
+00000790: 4465 7665 6c6f 7065 7273 0a43 6c61 7373  Developers.Class
+000007a0: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
+000007b0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+000007c0: 3a20 4d49 5420 4c69 6365 6e73 650a 436c  : MIT License.Cl
+000007d0: 6173 7369 6669 6572 3a20 4e61 7475 7261  assifier: Natura
+000007e0: 6c20 4c61 6e67 7561 6765 203a 3a20 456e  l Language :: En
+000007f0: 676c 6973 680a 436c 6173 7369 6669 6572  glish.Classifier
+00000800: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
+00000810: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+00000820: 6465 6e74 0a43 6c61 7373 6966 6965 723a  dent.Classifier:
+00000830: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000840: 6775 6167 6520 3a3a 2050 7974 686f 6e0a  guage :: Python.
 00000850: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
 00000860: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000870: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000880: 370a 436c 6173 7369 6669 6572 3a20 5072  7.Classifier: Pr
-00000890: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000008a0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000008b0: 332e 380a 436c 6173 7369 6669 6572 3a20  3.8.Classifier: 
-000008c0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000008d0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000008e0: 3a20 332e 390a 436c 6173 7369 6669 6572  : 3.9.Classifier
-000008f0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000900: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000910: 203a 3a20 332e 3130 0a43 6c61 7373 6966   :: 3.10.Classif
-00000920: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000930: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000940: 686f 6e20 3a3a 2033 2e31 310a 436c 6173  hon :: 3.11.Clas
-00000950: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000960: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000970: 5079 7468 6f6e 203a 3a20 496d 706c 656d  Python :: Implem
-00000980: 656e 7461 7469 6f6e 203a 3a20 4350 7974  entation :: CPyt
-00000990: 686f 6e0a 436c 6173 7369 6669 6572 3a20  hon.Classifier: 
-000009a0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000009b0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000009c0: 3a20 496d 706c 656d 656e 7461 7469 6f6e  : Implementation
-000009d0: 203a 3a20 5079 5079 0a43 6c61 7373 6966   :: PyPy.Classif
-000009e0: 6965 723a 2054 6f70 6963 203a 3a20 446f  ier: Topic :: Do
-000009f0: 6375 6d65 6e74 6174 696f 6e0a 436c 6173  cumentation.Clas
-00000a00: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
-00000a10: 2053 6f66 7477 6172 6520 4465 7665 6c6f   Software Develo
-00000a20: 706d 656e 740a 436c 6173 7369 6669 6572  pment.Classifier
-00000a30: 3a20 546f 7069 6320 3a3a 2054 6578 7420  : Topic :: Text 
-00000a40: 5072 6f63 6573 7369 6e67 0a43 6c61 7373  Processing.Class
-00000a50: 6966 6965 723a 2054 7970 696e 6720 3a3a  ifier: Typing ::
-00000a60: 2054 7970 6564 0a52 6571 7569 7265 732d   Typed.Requires-
-00000a70: 5079 7468 6f6e 3a20 3e3d 332e 360a 5265  Python: >=3.6.Re
-00000a80: 7175 6972 6573 2d44 6973 743a 2061 6e79  quires-Dist: any
-00000a90: 636f 6e66 6967 0a52 6571 7569 7265 732d  config.Requires-
-00000aa0: 4469 7374 3a20 6265 6175 7469 6675 6c73  Dist: beautifuls
-00000ab0: 6f75 7034 0a52 6571 7569 7265 732d 4469  oup4.Requires-Di
-00000ac0: 7374 3a20 6368 6563 6b73 756d 6469 720a  st: checksumdir.
-00000ad0: 5265 7175 6972 6573 2d44 6973 743a 2063  Requires-Dist: c
-00000ae0: 6f6f 6b69 6563 7574 7465 720a 5265 7175  ookiecutter.Requ
-00000af0: 6972 6573 2d44 6973 743a 2063 6f70 6965  ires-Dist: copie
-00000b00: 720a 5265 7175 6972 6573 2d44 6973 743a  r.Requires-Dist:
-00000b10: 2064 6565 706d 6572 6765 0a52 6571 7569   deepmerge.Requi
-00000b20: 7265 732d 4469 7374 3a20 6469 736b 6361  res-Dist: diskca
-00000b30: 6368 650a 5265 7175 6972 6573 2d44 6973  che.Requires-Dis
-00000b40: 743a 2066 6565 6467 656e 0a52 6571 7569  t: feedgen.Requi
-00000b50: 7265 732d 4469 7374 3a20 6a69 6e6a 6132  res-Dist: jinja2
-00000b60: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000b70: 6c69 6e6b 6966 792d 6974 2d70 790a 5265  linkify-it-py.Re
-00000b80: 7175 6972 6573 2d44 6973 743a 206d 6172  quires-Dist: mar
-00000b90: 6b64 6f77 6e2d 6974 2d70 795b 706c 7567  kdown-it-py[plug
-00000ba0: 696e 735d 0a52 6571 7569 7265 732d 4469  ins].Requires-Di
-00000bb0: 7374 3a20 6d61 726b 646f 776e 325b 616c  st: markdown2[al
-00000bc0: 6c5d 0a52 6571 7569 7265 732d 4469 7374  l].Requires-Dist
-00000bd0: 3a20 6d6f 7265 2d69 7465 7274 6f6f 6c73  : more-itertools
-00000be0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000bf0: 7061 7468 7370 6563 0a52 6571 7569 7265  pathspec.Require
-00000c00: 732d 4469 7374 3a20 7069 6c6c 6f77 0a52  s-Dist: pillow.R
-00000c10: 6571 7569 7265 732d 4469 7374 3a20 706c  equires-Dist: pl
-00000c20: 7567 6779 0a52 6571 7569 7265 732d 4469  uggy.Requires-Di
-00000c30: 7374 3a20 7079 6d64 6f77 6e2d 6578 7465  st: pymdown-exte
-00000c40: 6e73 696f 6e73 0a52 6571 7569 7265 732d  nsions.Requires-
-00000c50: 4469 7374 3a20 7079 7468 6f6e 2d66 726f  Dist: python-fro
-00000c60: 6e74 6d61 7474 6572 0a52 6571 7569 7265  ntmatter.Require
-00000c70: 732d 4469 7374 3a20 7079 7468 6f6e 2d73  s-Dist: python-s
-00000c80: 6c75 6769 6679 0a52 6571 7569 7265 732d  lugify.Requires-
-00000c90: 4469 7374 3a20 7079 747a 0a52 6571 7569  Dist: pytz.Requi
-00000ca0: 7265 732d 4469 7374 3a20 7269 6368 0a52  res-Dist: rich.R
-00000cb0: 6571 7569 7265 732d 4469 7374 3a20 7465  equires-Dist: te
-00000cc0: 7874 7561 6c3c 302e 322e 300a 5265 7175  xtual<0.2.0.Requ
-00000cd0: 6972 6573 2d44 6973 743a 2074 6f6d 6c0a  ires-Dist: toml.
-00000ce0: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
-00000cf0: 7970 6572 0a50 726f 7669 6465 732d 4578  yper.Provides-Ex
-00000d00: 7472 613a 2064 6576 0a52 6571 7569 7265  tra: dev.Require
-00000d10: 732d 4469 7374 3a20 626c 6163 6b3d 3d32  s-Dist: black==2
-00000d20: 322e 3130 2e30 3b20 6578 7472 6120 3d3d  2.10.0; extra ==
-00000d30: 2027 6465 7627 0a52 6571 7569 7265 732d   'dev'.Requires-
-00000d40: 4469 7374 3a20 6861 7463 683b 2065 7874  Dist: hatch; ext
-00000d50: 7261 203d 3d20 2764 6576 270a 5265 7175  ra == 'dev'.Requ
-00000d60: 6972 6573 2d44 6973 743a 2069 6e74 6572  ires-Dist: inter
-00000d70: 726f 6761 7465 3b20 6578 7472 6120 3d3d  rogate; extra ==
-00000d80: 2027 6465 7627 0a52 6571 7569 7265 732d   'dev'.Requires-
-00000d90: 4469 7374 3a20 6d79 7079 3b20 6578 7472  Dist: mypy; extr
-00000da0: 6120 3d3d 2027 6465 7627 0a52 6571 7569  a == 'dev'.Requi
-00000db0: 7265 732d 4469 7374 3a20 7072 652d 636f  res-Dist: pre-co
-00000dc0: 6d6d 6974 3b20 6578 7472 6120 3d3d 2027  mmit; extra == '
-00000dd0: 6465 7627 0a52 6571 7569 7265 732d 4469  dev'.Requires-Di
-00000de0: 7374 3a20 7079 7465 7374 3b20 6578 7472  st: pytest; extr
-00000df0: 6120 3d3d 2027 6465 7627 0a52 6571 7569  a == 'dev'.Requi
-00000e00: 7265 732d 4469 7374 3a20 7079 7465 7374  res-Dist: pytest
-00000e10: 2d63 6f76 3b20 6578 7472 6120 3d3d 2027  -cov; extra == '
-00000e20: 6465 7627 0a52 6571 7569 7265 732d 4469  dev'.Requires-Di
-00000e30: 7374 3a20 7079 7465 7374 2d6d 6f63 6b3b  st: pytest-mock;
-00000e40: 2065 7874 7261 203d 3d20 2764 6576 270a   extra == 'dev'.
-00000e50: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
-00000e60: 7974 6573 742d 746d 702d 6669 6c65 733b  ytest-tmp-files;
-00000e70: 2065 7874 7261 203d 3d20 2764 6576 270a   extra == 'dev'.
-00000e80: 5265 7175 6972 6573 2d44 6973 743a 2072  Requires-Dist: r
-00000e90: 7566 663b 2065 7874 7261 203d 3d20 2764  uff; extra == 'd
-00000ea0: 6576 270a 5072 6f76 6964 6573 2d45 7874  ev'.Provides-Ext
-00000eb0: 7261 3a20 7079 696e 7374 7275 6d65 6e74  ra: pyinstrument
-00000ec0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000ed0: 7079 696e 7374 7275 6d65 6e74 3b20 6578  pyinstrument; ex
-00000ee0: 7472 6120 3d3d 2027 7079 696e 7374 7275  tra == 'pyinstru
-00000ef0: 6d65 6e74 270a 4465 7363 7269 7074 696f  ment'.Descriptio
-00000f00: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-00000f10: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a3c  text/markdown..<
-00000f20: 6831 2061 6c69 676e 3d63 656e 7465 723e  h1 align=center>
-00000f30: 0a20 203c 6272 3e0a 2020 3c61 2068 7265  .  <br>.  <a hre
-00000f40: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00000f50: 622e 636f 6d2f 5761 796c 6f6e 5761 6c6b  b.com/WaylonWalk
-00000f60: 6572 2f6d 6172 6b61 7461 223e 3c69 6d67  er/markata"><img
-00000f70: 2073 7263 3d22 6874 7470 733a 2f2f 7573   src="https://us
-00000f80: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
-00000f90: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000fa0: 3232 3634 3833 3735 2f31 3637 3532 3731  22648375/1675271
-00000fb0: 3933 2d34 6536 3664 3533 372d 6537 3866  93-4e66d537-e78f
-00000fc0: 2d34 3464 642d 6265 3635 2d32 6331 6331  -44dd-be65-2c1c1
-00000fd0: 3039 6164 6633 342e 706e 6722 2061 6c74  09adf34.png" alt
-00000fe0: 3d22 4d61 726b 6174 6122 2077 6964 7468  ="Markata" width
-00000ff0: 3d22 3430 3022 3e3c 2f61 3e0a 3c2f 6831  ="400"></a>.</h1
-00001000: 3e0a 0a3c 7020 616c 6967 6e3d 6365 6e74  >..<p align=cent
-00001010: 6572 3e0a 2020 3c65 6d3e 0a20 2020 204d  er>.  <em>.    M
-00001020: 6172 6b64 6f77 6e20 746f 2073 6974 652c  arkdown to site,
-00001030: 2070 6c75 6769 6e73 2061 6c6c 2074 6865   plugins all the
-00001040: 2077 6179 2064 6f77 6e0a 2020 3c2f 656d   way down.  </em
-00001050: 3e0a 3c2f 703e 0a0a 4120 7374 6174 6963  >.</p>..A static
-00001060: 2073 6974 6520 6765 6e65 7261 746f 7220   site generator 
-00001070: 7468 6174 2077 696c 6c20 6769 7665 2079  that will give y
-00001080: 6f75 2061 2067 7265 6174 2073 6974 6520  ou a great site 
-00001090: 7769 7468 206d 616e 7920 7374 616e 6461  with many standa
-000010a0: 7264 2077 6562 0a66 6561 7475 7265 7320  rd web.features 
-000010b0: 6c69 6b65 2072 7373 2c20 7369 7465 6d61  like rss, sitema
-000010c0: 7073 2c20 616e 6420 7365 6f20 7461 6773  ps, and seo tags
-000010d0: 2c20 6f75 7420 6f66 2074 6865 2062 6f78  , out of the box
-000010e0: 2e20 5275 6e6e 696e 6720 606d 6172 6b61  . Running `marka
-000010f0: 7461 0a62 7569 6c64 6020 7769 6c6c 2067  ta.build` will g
-00001100: 6574 2079 6f75 2061 2074 6861 7420 6f6e  et you a that on
-00001110: 6c79 2072 6571 7569 7265 7320 796f 7520  ly requires you 
-00001120: 746f 2077 7269 7465 204d 6172 6b64 6f77  to write Markdow
-00001130: 6e2e 2049 6620 796f 7520 6861 7665 0a61  n. If you have.a
-00001140: 6464 6974 696f 6e61 6c20 6665 6174 7572  dditional featur
-00001150: 6573 2074 6861 7420 796f 7520 7761 6e74  es that you want
-00001160: 2c20 646f 6e27 7420 776f 7272 792c 2073  , don't worry, s
-00001170: 696e 6365 206d 6172 6b61 7461 2069 7320  ince markata is 
-00001180: 6275 696c 740a 636f 6d70 6c65 7465 6c79  built.completely
-00001190: 206f 6e20 706c 7567 696e 7320 796f 7520   on plugins you 
-000011a0: 6361 6e20 6465 7665 6c6f 7020 616e 6420  can develop and 
-000011b0: 696e 7374 616c 6c20 796f 7572 206f 776e  install your own
-000011c0: 2070 6c75 6769 6e73 2074 6f20 6164 6420   plugins to add 
-000011d0: 7468 650a 6665 6174 7572 6573 2079 6f75  the.features you
-000011e0: 2077 616e 742e 0a0a 2323 2051 7569 636b   want...## Quick
-000011f0: 5374 6172 740a 0a4d 6172 6b61 7461 2069  Start..Markata i
-00001200: 7320 6675 6c6c 7920 636f 6e66 6967 7572  s fully configur
-00001210: 6162 6c65 2074 6872 6f75 6768 2061 2060  able through a `
-00001220: 6d61 726b 6174 612e 746f 6d6c 6020 6669  markata.toml` fi
-00001230: 6c65 2c20 6275 7420 7468 6520 6465 6661  le, but the defa
-00001240: 756c 7473 0a61 6c6c 6f77 2074 6f20 6275  ults.allow to bu
-00001250: 696c 6420 796f 7572 2073 6974 6520 7269  ild your site ri
-00001260: 6768 7420 6f75 7420 6f66 2074 6865 2062  ght out of the b
-00001270: 6f78 2077 6974 6820 6e6f 7468 696e 6720  ox with nothing 
-00001280: 6d6f 7265 2074 6861 6e20 4d61 726b 646f  more than Markdo
-00001290: 776e 2e0a 0a23 2323 2043 7265 6174 6520  wn...### Create 
-000012a0: 536f 6d65 2043 6f6e 7465 6e74 0a0a 4d61  Some Content..Ma
-000012b0: 6b65 2073 6f6d 6520 602e 6d64 6020 6669  ke some `.md` fi
-000012c0: 6c65 7320 696e 2079 6f75 7220 6375 7272  les in your curr
-000012d0: 656e 7420 776f 726b 696e 6720 6469 7265  ent working dire
-000012e0: 6374 6f72 792e 2042 7920 6465 6661 756c  ctory. By defaul
-000012f0: 742c 2060 6d61 726b 6174 6160 0a77 696c  t, `markata`.wil
-00001300: 6c20 7265 6375 7273 6976 656c 7920 6c6f  l recursively lo
-00001310: 6f6b 2069 6e20 616c 6c20 7375 6264 6972  ok in all subdir
-00001320: 6563 746f 7269 6573 2066 6f72 206d 6172  ectories for mar
-00001330: 6b64 6f77 6e20 6669 6c65 7320 602a 2a2f  kdown files `**/
-00001340: 2a2e 6d64 602e 0a0a 6060 6062 6173 680a  *.md`...```bash.
-00001350: 6d6b 6469 7220 7061 6765 730a 6563 686f  mkdir pages.echo
-00001360: 2027 2320 4d79 2046 6972 7374 2050 6f73   '# My First Pos
-00001370: 7427 203e 2066 6972 7374 2d70 6f73 742e  t' > first-post.
-00001380: 6d64 0a65 6368 6f20 2723 2048 656c 6c6f  md.echo '# Hello
-00001390: 2057 6f72 6c64 2720 3e20 6865 6c6c 6f2d   World' > hello-
-000013a0: 776f 726c 642e 6d64 0a60 6060 0a0a 2323  world.md.```..##
-000013b0: 2320 4275 696c 6420 796f 7572 2073 6974  # Build your sit
-000013c0: 650a 0a49 6e73 7461 6c6c 206d 6172 6b61  e..Install marka
-000013d0: 7461 2069 6e74 6f20 796f 7572 2076 6972  ta into your vir
-000013e0: 7475 616c 2065 6e76 6972 6f6e 6d65 6e74  tual environment
-000013f0: 2061 6e64 2072 756e 2060 6d61 726b 6174   and run `markat
-00001400: 6120 6275 696c 6460 2e20 4974 2077 696c  a build`. It wil
-00001410: 6c0a 6372 6561 7465 2079 6f75 7220 7369  l.create your si
-00001420: 7465 2069 6e20 602e 2f6d 6172 6b6f 7574  te in `./markout
-00001430: 602c 206c 6561 7665 2069 7473 2063 6163  `, leave its cac
-00001440: 6865 2069 6e20 602e 2f2e 6d61 726b 6174  he in `./.markat
-00001450: 612e 6361 6368 6560 2c20 616e 640a 636f  a.cache`, and.co
-00001460: 7079 2061 6c6c 2061 7373 6574 7320 6672  py all assets fr
-00001470: 6f6d 2060 2e2f 7374 6174 6963 6020 696e  om `./static` in
-00001480: 746f 2060 2e2f 6d61 726b 6f75 7460 2062  to `./markout` b
-00001490: 7920 6465 6661 756c 742e 0a0a 6060 6062  y default...```b
-000014a0: 6173 680a 7079 7468 6f6e 202d 6d20 7069  ash.python -m pi
-000014b0: 7020 696e 7374 616c 6c20 6d61 726b 6174  p install markat
-000014c0: 610a 6d61 726b 6174 6120 6275 696c 640a  a.markata build.
-000014d0: 0a23 206f 7220 6966 2070 6970 7820 6973  .# or if pipx is
-000014e0: 2079 6f75 7220 7468 696e 670a 7069 7078   your thing.pipx
-000014f0: 2072 756e 206d 6172 6b61 7461 2062 7569   run markata bui
-00001500: 6c64 0a60 6060 0a0a 2323 2320 4275 696c  ld.```..### Buil
-00001510: 6469 6e67 2061 2042 6c6f 6720 7769 7468  ding a Blog with
-00001520: 204d 6172 6b61 7461 0a0a 5468 6520 6d61   Markata..The ma
-00001530: 726b 6174 6120 636c 6920 696e 636c 7564  rkata cli includ
-00001540: 6573 2061 2060 6e65 7760 2063 6f6d 6d61  es a `new` comma
-00001550: 6e64 2074 6861 7420 7769 6c6c 2070 7265  nd that will pre
-00001560: 7365 6e74 2079 6f75 2077 6974 6820 7175  sent you with qu
-00001570: 6573 7469 6f6e 730a 746f 2066 696c 6c20  estions.to fill 
-00001580: 696e 2074 6865 206a 696e 6a61 2076 6172  in the jinja var
-00001590: 6961 626c 6573 2069 6e20 7468 6973 2072  iables in this r
-000015a0: 6570 6f2e 0a0a 6060 6062 6173 680a 6d61  epo...```bash.ma
-000015b0: 726b 6174 6120 6e65 7720 626c 6f67 205b  rkata new blog [
-000015c0: 6469 7265 6374 6f72 795d 0a0a 2320 7374  directory]..# st
-000015d0: 6172 7420 7468 6520 7369 7465 2061 6e64  art the site and
-000015e0: 2077 6174 6368 2066 6f72 2063 6861 6e67   watch for chang
-000015f0: 6573 0a68 6174 6368 2072 756e 2074 7569  es.hatch run tui
-00001600: 0a60 6060 0a0a 4e6f 7720 6966 2079 6f75  .```..Now if you
-00001610: 206f 7065 6e20 6c6f 6361 6c68 6f73 743a   open localhost:
-00001620: 3830 3030 2c20 796f 7520 7769 6c6c 2062  8000, you will b
-00001630: 6520 7072 6573 656e 7465 6420 7769 7468  e presented with
-00001640: 2061 6e20 6578 616d 706c 6520 7369 7465   an example site
-00001650: 2074 6861 740a 7769 6c6c 2077 616c 6b20   that.will walk 
-00001660: 796f 7520 7468 726f 7567 6820 736f 6d65  you through some
-00001670: 2066 6561 7475 7265 7320 6f66 206d 6172   features of mar
-00001680: 6b61 7461 2e20 596f 7520 6361 6e20 706c  kata. You can pl
-00001690: 6179 2077 6974 6820 6974 2061 740a 796f  ay with it at.yo
-000016a0: 7572 206f 776e 2070 6163 652c 206f 7220  ur own pace, or 
-000016b0: 6472 6f70 2061 6c6c 2074 6865 2070 6167  drop all the pag
-000016c0: 6573 2061 6e64 2073 7461 7274 2077 7269  es and start wri
-000016d0: 7469 6e67 2079 6f75 7220 6f77 6e20 636f  ting your own co
-000016e0: 6e74 656e 742e 0a0a 2323 204d 6f74 6976  ntent...## Motiv
-000016f0: 6174 696f 6e0a 0a4d 6172 6b61 7461 2069  ation..Markata i
-00001700: 7320 6162 6c65 2074 6f20 6275 696c 6420  s able to build 
-00001710: 796f 7572 2073 6974 6520 7075 7265 6c79  your site purely
-00001720: 2066 726f 6d20 4d61 726b 646f 776e 2c20   from Markdown, 
-00001730: 616c 6c6f 7769 6e67 2079 6f75 2074 6f20  allowing you to 
-00001740: 6765 740a 7374 6172 7465 6420 6372 6561  get.started crea
-00001750: 7469 6e67 2079 6f75 7220 6f77 6e20 636f  ting your own co
-00001760: 6e74 656e 7420 7175 6963 6b6c 792e 204f  ntent quickly. O
-00001770: 7574 206f 6620 7468 6520 626f 7820 6974  ut of the box it
-00001780: 2077 696c 6c20 636f 7665 7220 796f 7572   will cover your
-00001790: 0a73 656f 2074 6167 732c 2072 7373 2066  .seo tags, rss f
-000017a0: 6565 6473 2c20 7369 7465 6d61 702c 2061  eeds, sitemap, a
-000017b0: 6e64 206f 6720 696d 6167 6573 2e20 5369  nd og images. Si
-000017c0: 6e63 6520 6974 2069 7320 6275 696c 7420  nce it is built 
-000017d0: 636f 6d70 6c65 7465 6c79 2066 726f 6d0a  completely from.
-000017e0: 706c 7567 696e 7320 796f 7520 6361 6e20  plugins you can 
-000017f0: 7265 6d6f 7665 2c20 6d6f 6469 6679 2c20  remove, modify, 
-00001800: 6f72 2061 6464 2074 6f20 616e 7920 6f66  or add to any of
-00001810: 2069 7473 2062 6568 6176 696f 722e 0a0a   its behavior...
-00001820: 2d20 636f 6e66 6967 7572 6162 6c65 0a2d  - configurable.-
-00001830: 2070 6c75 6769 6e73 0a2d 2073 656f 0a2d   plugins.- seo.-
-00001840: 2072 7373 0a2d 2073 6974 656d 6170 0a2d   rss.- sitemap.-
-00001850: 206f 672d 696d 6167 650a 0a23 2320 5573   og-image..## Us
-00001860: 696e 6720 4d61 726b 6174 610a 0a54 6865  ing Markata..The
-00001870: 2064 6f63 7320 6172 6520 7374 696c 6c20   docs are still 
-00001880: 6120 776f 726b 2069 6e20 7072 6f67 7265  a work in progre
-00001890: 7373 2c20 6275 7420 7468 650a 5b62 6173  ss, but the.[bas
-000018a0: 655f 636c 695d 2868 7474 7073 3a2f 2f6d  e_cli](https://m
-000018b0: 6172 6b61 7461 2e64 6576 2f6d 6172 6b61  arkata.dev/marka
-000018c0: 7461 2f70 6c75 6769 6e73 2f62 6173 655f  ta/plugins/base_
-000018d0: 636c 692f 2920 7761 6c6b 7320 7468 726f  cli/) walks thro
-000018e0: 7567 6820 686f 7720 746f 0a65 6666 6563  ugh how to.effec
-000018f0: 7469 7665 6c79 2075 7365 2074 6865 2060  tively use the `
-00001900: 6d61 726b 6174 6120 6275 696c 6460 2063  markata build` c
-00001910: 6f6d 6d61 6e64 2e20 4174 2074 6869 7320  ommand. At this 
-00001920: 706f 696e 7420 4d61 726b 6174 6120 6973  point Markata is
-00001930: 2066 6172 2066 726f 6d0a 7374 6162 6c65   far from.stable
-00001940: 2061 6e64 202a 2a77 696c 6c20 6368 616e   and **will chan
-00001950: 6765 2071 7569 7465 2061 2062 6974 2a2a  ge quite a bit**
-00001960: 2c20 7368 6f75 6c64 2079 6f75 2063 686f  , should you cho
-00001970: 6f73 6520 746f 2075 7365 2069 7420 6f6e  ose to use it on
-00001980: 2072 6561 6c0a 7369 7465 206d 616b 6520   real.site make 
-00001990: 7375 7265 2079 6f75 2070 696e 2074 6f20  sure you pin to 
-000019a0: 7468 6520 7665 7273 696f 6e20 7468 6174  the version that
-000019b0: 2079 6f75 2077 616e 7420 746f 2062 7569   you want to bui
-000019c0: 6c64 2066 726f 6d2e 2049 2077 696c 6c20  ld from. I will 
-000019d0: 6c65 740a 796f 7520 6b6e 6f77 2061 7320  let.you know as 
-000019e0: 6974 2062 6563 6f6d 6573 206d 6f72 6520  it becomes more 
-000019f0: 7374 6162 6c65 2061 6e64 2072 6561 6479  stable and ready
-00001a00: 2074 6f20 7573 6520 7769 7468 6f75 7420   to use without 
-00001a10: 6469 6c69 6765 6e63 6520 6f66 0a70 696e  diligence of.pin
-00001a20: 6e69 6e67 2074 6f20 7468 6520 7665 7273  ning to the vers
-00001a30: 696f 6e20 796f 7520 7761 6e74 2e0a 0a2a  ion you want...*
-00001a40: 2a48 6f6e 6573 746c 792a 2a20 4120 6269  *Honestly** A bi
-00001a50: 6720 6d6f 7469 7661 7469 6f6e 2066 6f72  g motivation for
-00001a60: 206d 6520 7761 7320 7761 6e74 696e 6720   me was wanting 
-00001a70: 746f 206c 6561 726e 2061 6e64 2075 6e64  to learn and und
-00001a80: 6572 7374 616e 6420 686f 7720 746f 0a63  erstand how to.c
-00001a90: 7265 6174 6520 6120 7072 6f6a 6563 7420  reate a project 
-00001aa0: 7468 6174 2069 7320 636f 6d70 6c65 7465  that is complete
-00001ab0: 6c79 2070 6c75 6769 6e20 6472 6976 656e  ly plugin driven
-00001ac0: 2e20 5468 6973 2069 7320 6869 6768 6c79  . This is highly
-00001ad0: 2061 206c 6561 726e 696e 670a 7072 6f6a   a learning.proj
-00001ae0: 6563 7420 666f 7220 6d65 2c20 616e 6420  ect for me, and 
-00001af0: 6974 2068 6173 2067 726f 776e 2069 6e74  it has grown int
-00001b00: 6f20 736f 6d65 7468 696e 6720 4920 7573  o something I us
-00001b10: 6520 6576 6572 7920 6461 792e 0a0a 2323  e every day...##
-00001b20: 2045 7861 6d70 6c65 7320 4761 6c6c 6172   Examples Gallar
-00001b30: 790a 0a4d 6172 6b61 7461 2068 6173 2061  y..Markata has a
-00001b40: 2070 726f 6a65 6374 2067 616c 6c65 7279   project gallery
-00001b50: 2074 6f20 7368 6f77 206f 6666 2073 6974   to show off sit
-00001b60: 6573 2062 7569 6c74 2077 6974 6820 6d61  es built with ma
-00001b70: 726b 6174 612e 2050 6c65 6173 650a 5b73  rkata. Please.[s
-00001b80: 7562 6d69 745d 2868 7474 7073 3a2f 2f67  ubmit](https://g
-00001b90: 6974 6875 622e 636f 6d2f 5761 796c 6f6e  ithub.com/Waylon
-00001ba0: 5761 6c6b 6572 2f6d 6172 6b61 7461 2f69  Walker/markata/i
-00001bb0: 7373 7565 732f 3738 2920 796f 7572 732c  ssues/78) yours,
-00001bc0: 2061 6e64 2063 6865 636b 0a6f 7574 2074   and check.out t
-00001bd0: 6865 205b 7072 6f6a 6563 742d 6761 6c6c  he [project-gall
-00001be0: 6572 795d 2868 7474 703a 2f2f 6d61 726b  ery](http://mark
-00001bf0: 6174 612e 6465 762f 7072 6f6a 6563 742d  ata.dev/project-
-00001c00: 6761 6c6c 6572 792f 2920 666f 7220 696e  gallery/) for in
-00001c10: 7370 6972 6174 696f 6e2e 0a              spiration..
+00000870: 203a 3a20 5079 7468 6f6e 203a 3a20 330a   :: Python :: 3.
+00000880: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000890: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000008a0: 203a 3a20 5079 7468 6f6e 203a 3a20 3320   :: Python :: 3 
+000008b0: 3a3a 204f 6e6c 790a 436c 6173 7369 6669  :: Only.Classifi
+000008c0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+000008d0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000008e0: 6f6e 203a 3a20 332e 370a 436c 6173 7369  on :: 3.7.Classi
+000008f0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000900: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000910: 7468 6f6e 203a 3a20 332e 380a 436c 6173  thon :: 3.8.Clas
+00000920: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000930: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000940: 5079 7468 6f6e 203a 3a20 332e 390a 436c  Python :: 3.9.Cl
+00000950: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000960: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000970: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
+00000980: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000990: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000009a0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000009b0: 2e31 310a 436c 6173 7369 6669 6572 3a20  .11.Classifier: 
+000009c0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000009d0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000009e0: 3a20 496d 706c 656d 656e 7461 7469 6f6e  : Implementation
+000009f0: 203a 3a20 4350 7974 686f 6e0a 436c 6173   :: CPython.Clas
+00000a00: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000a10: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000a20: 5079 7468 6f6e 203a 3a20 496d 706c 656d  Python :: Implem
+00000a30: 656e 7461 7469 6f6e 203a 3a20 5079 5079  entation :: PyPy
+00000a40: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+00000a50: 6963 203a 3a20 446f 6375 6d65 6e74 6174  ic :: Documentat
+00000a60: 696f 6e0a 436c 6173 7369 6669 6572 3a20  ion.Classifier: 
+00000a70: 546f 7069 6320 3a3a 2053 6f66 7477 6172  Topic :: Softwar
+00000a80: 6520 4465 7665 6c6f 706d 656e 740a 436c  e Development.Cl
+00000a90: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
+00000aa0: 3a3a 2054 6578 7420 5072 6f63 6573 7369  :: Text Processi
+00000ab0: 6e67 0a43 6c61 7373 6966 6965 723a 2054  ng.Classifier: T
+00000ac0: 7970 696e 6720 3a3a 2054 7970 6564 0a52  yping :: Typed.R
+00000ad0: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
+00000ae0: 3e3d 332e 360a 5265 7175 6972 6573 2d44  >=3.6.Requires-D
+00000af0: 6973 743a 2061 6e79 636f 6e66 6967 0a52  ist: anyconfig.R
+00000b00: 6571 7569 7265 732d 4469 7374 3a20 6265  equires-Dist: be
+00000b10: 6175 7469 6675 6c73 6f75 7034 0a52 6571  autifulsoup4.Req
+00000b20: 7569 7265 732d 4469 7374 3a20 6368 6563  uires-Dist: chec
+00000b30: 6b73 756d 6469 720a 5265 7175 6972 6573  ksumdir.Requires
+00000b40: 2d44 6973 743a 2063 6f6d 6d6f 6e6d 6172  -Dist: commonmar
+00000b50: 6b0a 5265 7175 6972 6573 2d44 6973 743a  k.Requires-Dist:
+00000b60: 2063 6f6f 6b69 6563 7574 7465 720a 5265   cookiecutter.Re
+00000b70: 7175 6972 6573 2d44 6973 743a 2063 6f70  quires-Dist: cop
+00000b80: 6965 720a 5265 7175 6972 6573 2d44 6973  ier.Requires-Dis
+00000b90: 743a 2064 6565 706d 6572 6765 0a52 6571  t: deepmerge.Req
+00000ba0: 7569 7265 732d 4469 7374 3a20 6469 736b  uires-Dist: disk
+00000bb0: 6361 6368 650a 5265 7175 6972 6573 2d44  cache.Requires-D
+00000bc0: 6973 743a 2066 6565 6467 656e 0a52 6571  ist: feedgen.Req
+00000bd0: 7569 7265 732d 4469 7374 3a20 6a69 6e6a  uires-Dist: jinj
+00000be0: 6132 0a52 6571 7569 7265 732d 4469 7374  a2.Requires-Dist
+00000bf0: 3a20 6c69 6e6b 6966 792d 6974 2d70 790a  : linkify-it-py.
+00000c00: 5265 7175 6972 6573 2d44 6973 743a 206d  Requires-Dist: m
+00000c10: 6172 6b64 6f77 6e2d 6974 2d70 795b 706c  arkdown-it-py[pl
+00000c20: 7567 696e 735d 0a52 6571 7569 7265 732d  ugins].Requires-
+00000c30: 4469 7374 3a20 6d61 726b 646f 776e 325b  Dist: markdown2[
+00000c40: 616c 6c5d 0a52 6571 7569 7265 732d 4469  all].Requires-Di
+00000c50: 7374 3a20 6d6f 7265 2d69 7465 7274 6f6f  st: more-itertoo
+00000c60: 6c73 0a52 6571 7569 7265 732d 4469 7374  ls.Requires-Dist
+00000c70: 3a20 7061 7468 7370 6563 0a52 6571 7569  : pathspec.Requi
+00000c80: 7265 732d 4469 7374 3a20 7069 6c6c 6f77  res-Dist: pillow
+00000c90: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000ca0: 706c 7567 6779 0a52 6571 7569 7265 732d  pluggy.Requires-
+00000cb0: 4469 7374 3a20 7079 6d64 6f77 6e2d 6578  Dist: pymdown-ex
+00000cc0: 7465 6e73 696f 6e73 0a52 6571 7569 7265  tensions.Require
+00000cd0: 732d 4469 7374 3a20 7079 7468 6f6e 2d66  s-Dist: python-f
+00000ce0: 726f 6e74 6d61 7474 6572 0a52 6571 7569  rontmatter.Requi
+00000cf0: 7265 732d 4469 7374 3a20 7079 7468 6f6e  res-Dist: python
+00000d00: 2d73 6c75 6769 6679 0a52 6571 7569 7265  -slugify.Require
+00000d10: 732d 4469 7374 3a20 7079 747a 0a52 6571  s-Dist: pytz.Req
+00000d20: 7569 7265 732d 4469 7374 3a20 7269 6368  uires-Dist: rich
+00000d30: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000d40: 746f 6d6c 0a52 6571 7569 7265 732d 4469  toml.Requires-Di
+00000d50: 7374 3a20 7479 7065 720a 5072 6f76 6964  st: typer.Provid
+00000d60: 6573 2d45 7874 7261 3a20 6465 760a 5265  es-Extra: dev.Re
+00000d70: 7175 6972 6573 2d44 6973 743a 2062 6c61  quires-Dist: bla
+00000d80: 636b 3d3d 3232 2e31 302e 303b 2065 7874  ck==22.10.0; ext
+00000d90: 7261 203d 3d20 2764 6576 270a 5265 7175  ra == 'dev'.Requ
+00000da0: 6972 6573 2d44 6973 743a 2068 6174 6368  ires-Dist: hatch
+00000db0: 3b20 6578 7472 6120 3d3d 2027 6465 7627  ; extra == 'dev'
+00000dc0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000dd0: 696e 7465 7272 6f67 6174 653b 2065 7874  interrogate; ext
+00000de0: 7261 203d 3d20 2764 6576 270a 5265 7175  ra == 'dev'.Requ
+00000df0: 6972 6573 2d44 6973 743a 206d 7970 793b  ires-Dist: mypy;
+00000e00: 2065 7874 7261 203d 3d20 2764 6576 270a   extra == 'dev'.
+00000e10: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
+00000e20: 7265 2d63 6f6d 6d69 743b 2065 7874 7261  re-commit; extra
+00000e30: 203d 3d20 2764 6576 270a 5265 7175 6972   == 'dev'.Requir
+00000e40: 6573 2d44 6973 743a 2070 7974 6573 743b  es-Dist: pytest;
+00000e50: 2065 7874 7261 203d 3d20 2764 6576 270a   extra == 'dev'.
+00000e60: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
+00000e70: 7974 6573 742d 636f 763b 2065 7874 7261  ytest-cov; extra
+00000e80: 203d 3d20 2764 6576 270a 5265 7175 6972   == 'dev'.Requir
+00000e90: 6573 2d44 6973 743a 2070 7974 6573 742d  es-Dist: pytest-
+00000ea0: 6d6f 636b 3b20 6578 7472 6120 3d3d 2027  mock; extra == '
+00000eb0: 6465 7627 0a52 6571 7569 7265 732d 4469  dev'.Requires-Di
+00000ec0: 7374 3a20 7079 7465 7374 2d74 6d70 2d66  st: pytest-tmp-f
+00000ed0: 696c 6573 3b20 6578 7472 6120 3d3d 2027  iles; extra == '
+00000ee0: 6465 7627 0a52 6571 7569 7265 732d 4469  dev'.Requires-Di
+00000ef0: 7374 3a20 7275 6666 3b20 6578 7472 6120  st: ruff; extra 
+00000f00: 3d3d 2027 6465 7627 0a50 726f 7669 6465  == 'dev'.Provide
+00000f10: 732d 4578 7472 613a 2070 7969 6e73 7472  s-Extra: pyinstr
+00000f20: 756d 656e 740a 5265 7175 6972 6573 2d44  ument.Requires-D
+00000f30: 6973 743a 2070 7969 6e73 7472 756d 656e  ist: pyinstrumen
+00000f40: 743b 2065 7874 7261 203d 3d20 2770 7969  t; extra == 'pyi
+00000f50: 6e73 7472 756d 656e 7427 0a50 726f 7669  nstrument'.Provi
+00000f60: 6465 732d 4578 7472 613a 2074 7569 0a52  des-Extra: tui.R
+00000f70: 6571 7569 7265 732d 4469 7374 3a20 7465  equires-Dist: te
+00000f80: 7874 7561 6c3b 2065 7874 7261 203d 3d20  xtual; extra == 
+00000f90: 2774 7569 270a 5265 7175 6972 6573 2d44  'tui'.Requires-D
+00000fa0: 6973 743a 2074 726f 676f 6e3b 2065 7874  ist: trogon; ext
+00000fb0: 7261 203d 3d20 2774 7569 270a 4465 7363  ra == 'tui'.Desc
+00000fc0: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
+00000fd0: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
+00000fe0: 6f77 6e0a 0a3c 6831 2061 6c69 676e 3d63  own..<h1 align=c
+00000ff0: 656e 7465 723e 0a20 203c 6272 3e0a 2020  enter>.  <br>.  
+00001000: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001010: 2f67 6974 6875 622e 636f 6d2f 5761 796c  /github.com/Wayl
+00001020: 6f6e 5761 6c6b 6572 2f6d 6172 6b61 7461  onWalker/markata
+00001030: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00001040: 733a 2f2f 7573 6572 2d69 6d61 6765 732e  s://user-images.
+00001050: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00001060: 742e 636f 6d2f 3232 3634 3833 3735 2f31  t.com/22648375/1
+00001070: 3637 3532 3731 3933 2d34 6536 3664 3533  67527193-4e66d53
+00001080: 372d 6537 3866 2d34 3464 642d 6265 3635  7-e78f-44dd-be65
+00001090: 2d32 6331 6331 3039 6164 6633 342e 706e  -2c1c109adf34.pn
+000010a0: 6722 2061 6c74 3d22 4d61 726b 6174 6122  g" alt="Markata"
+000010b0: 2077 6964 7468 3d22 3430 3022 3e3c 2f61   width="400"></a
+000010c0: 3e0a 3c2f 6831 3e0a 0a3c 7020 616c 6967  >.</h1>..<p alig
+000010d0: 6e3d 6365 6e74 6572 3e0a 2020 3c65 6d3e  n=center>.  <em>
+000010e0: 0a20 2020 204d 6172 6b64 6f77 6e20 746f  .    Markdown to
+000010f0: 2073 6974 652c 2070 6c75 6769 6e73 2061   site, plugins a
+00001100: 6c6c 2074 6865 2077 6179 2064 6f77 6e0a  ll the way down.
+00001110: 2020 3c2f 656d 3e0a 3c2f 703e 0a0a 2323    </em>.</p>..##
+00001120: 2043 6f6d 696e 6720 736f 6f6e 0a0a 7079   Coming soon..py
+00001130: 6461 6e74 6963 2061 6c6c 2074 6865 2074  dantic all the t
+00001140: 6869 6e67 732e 2020 416c 6c20 706f 7374  hings.  All post
+00001150: 206f 626a 6563 7473 2061 6e64 2063 6f6e   objects and con
+00001160: 6669 6720 7769 6c6c 2062 6563 6f6d 6520  fig will become 
+00001170: 7079 6461 6e74 6963 206f 626a 6563 7473  pydantic objects
+00001180: 2e20 2054 6869 7320 7769 6c6c 2061 6c6c  .  This will all
+00001190: 6f77 2066 6f72 2076 616c 6964 6174 696f  ow for validatio
+000011a0: 6e20 746f 2068 6170 7065 6e20 6561 726c  n to happen earl
+000011b0: 792c 2061 6e64 2072 6566 6572 656e 6369  y, and referenci
+000011c0: 6e67 2070 6f73 7420 6174 7472 6962 7574  ng post attribut
+000011d0: 6573 206f 7220 636f 6e66 6967 2c20 6974  es or config, it
+000011e0: 2063 616e 2062 6520 6173 7375 6d65 6420   can be assumed 
+000011f0: 7468 6174 2074 6865 7920 6578 6973 7420  that they exist 
+00001200: 7768 6574 6865 7220 7468 6579 2077 6572  whether they wer
+00001210: 6520 6578 706c 6963 6974 6c79 2063 7265  e explicitly cre
+00001220: 6174 6564 206f 7220 636f 6865 7273 6564  ated or cohersed
+00001230: 2074 6f20 7468 6569 7220 6465 6661 756c   to their defaul
+00001240: 7473 2065 6172 6c79 2069 6e20 7468 6520  ts early in the 
+00001250: 6275 696c 642e 0a0a 2d2d 2d0a 0a41 2073  build...---..A s
+00001260: 7461 7469 6320 7369 7465 2067 656e 6572  tatic site gener
+00001270: 6174 6f72 2074 6861 7420 7769 6c6c 2067  ator that will g
+00001280: 6976 6520 796f 7520 6120 6772 6561 7420  ive you a great 
+00001290: 7369 7465 2077 6974 6820 6d61 6e79 2073  site with many s
+000012a0: 7461 6e64 6172 6420 7765 620a 6665 6174  tandard web.feat
+000012b0: 7572 6573 206c 696b 6520 7273 732c 2073  ures like rss, s
+000012c0: 6974 656d 6170 732c 2061 6e64 2073 656f  itemaps, and seo
+000012d0: 2074 6167 732c 206f 7574 206f 6620 7468   tags, out of th
+000012e0: 6520 626f 782e 2052 756e 6e69 6e67 2060  e box. Running `
+000012f0: 6d61 726b 6174 610a 6275 696c 6460 2077  markata.build` w
+00001300: 696c 6c20 6765 7420 796f 7520 6120 7468  ill get you a th
+00001310: 6174 206f 6e6c 7920 7265 7175 6972 6573  at only requires
+00001320: 2079 6f75 2074 6f20 7772 6974 6520 4d61   you to write Ma
+00001330: 726b 646f 776e 2e20 4966 2079 6f75 2068  rkdown. If you h
+00001340: 6176 650a 6164 6469 7469 6f6e 616c 2066  ave.additional f
+00001350: 6561 7475 7265 7320 7468 6174 2079 6f75  eatures that you
+00001360: 2077 616e 742c 2064 6f6e 2774 2077 6f72   want, don't wor
+00001370: 7279 2c20 7369 6e63 6520 6d61 726b 6174  ry, since markat
+00001380: 6120 6973 2062 7569 6c74 0a63 6f6d 706c  a is built.compl
+00001390: 6574 656c 7920 6f6e 2070 6c75 6769 6e73  etely on plugins
+000013a0: 2079 6f75 2063 616e 2064 6576 656c 6f70   you can develop
+000013b0: 2061 6e64 2069 6e73 7461 6c6c 2079 6f75   and install you
+000013c0: 7220 6f77 6e20 706c 7567 696e 7320 746f  r own plugins to
+000013d0: 2061 6464 2074 6865 0a66 6561 7475 7265   add the.feature
+000013e0: 7320 796f 7520 7761 6e74 2e0a 0a23 2320  s you want...## 
+000013f0: 5175 6963 6b53 7461 7274 0a0a 4d61 726b  QuickStart..Mark
+00001400: 6174 6120 6973 2066 756c 6c79 2063 6f6e  ata is fully con
+00001410: 6669 6775 7261 626c 6520 7468 726f 7567  figurable throug
+00001420: 6820 6120 606d 6172 6b61 7461 2e74 6f6d  h a `markata.tom
+00001430: 6c60 2066 696c 652c 2062 7574 2074 6865  l` file, but the
+00001440: 2064 6566 6175 6c74 730a 616c 6c6f 7720   defaults.allow 
+00001450: 746f 2062 7569 6c64 2079 6f75 7220 7369  to build your si
+00001460: 7465 2072 6967 6874 206f 7574 206f 6620  te right out of 
+00001470: 7468 6520 626f 7820 7769 7468 206e 6f74  the box with not
+00001480: 6869 6e67 206d 6f72 6520 7468 616e 204d  hing more than M
+00001490: 6172 6b64 6f77 6e2e 0a0a 2323 2320 496e  arkdown...### In
+000014a0: 7374 616c 6c61 7469 6f6e 0a0a 606d 6172  stallation..`mar
+000014b0: 6b61 7461 6020 6973 2068 6f73 7465 6420  kata` is hosted 
+000014c0: 6f6e 2070 7970 6920 616e 6420 6361 6e20  on pypi and can 
+000014d0: 6265 2069 6e73 7461 6c6c 6564 2075 7369  be installed usi
+000014e0: 6e67 2070 6970 2e0a 0a60 6060 6261 7368  ng pip...```bash
+000014f0: 0a70 7974 686f 6e20 2d6d 2070 6970 2069  .python -m pip i
+00001500: 6e73 7461 6c6c 206d 6172 6b61 7461 0a60  nstall markata.`
+00001510: 6060 0a0a 2323 2320 4372 6561 7465 2053  ``..### Create S
+00001520: 6f6d 6520 436f 6e74 656e 740a 0a4d 616b  ome Content..Mak
+00001530: 6520 736f 6d65 2060 2e6d 6460 2066 696c  e some `.md` fil
+00001540: 6573 2069 6e20 796f 7572 2063 7572 7265  es in your curre
+00001550: 6e74 2077 6f72 6b69 6e67 2064 6972 6563  nt working direc
+00001560: 746f 7279 2e20 4279 2064 6566 6175 6c74  tory. By default
+00001570: 2c20 606d 6172 6b61 7461 600a 7769 6c6c  , `markata`.will
+00001580: 2072 6563 7572 7369 7665 6c79 206c 6f6f   recursively loo
+00001590: 6b20 696e 2061 6c6c 2073 7562 6469 7265  k in all subdire
+000015a0: 6374 6f72 6965 7320 666f 7220 6d61 726b  ctories for mark
+000015b0: 646f 776e 2066 696c 6573 2060 2a2a 2f2a  down files `**/*
+000015c0: 2e6d 6460 2e0a 0a60 6060 6261 7368 0a6d  .md`...```bash.m
+000015d0: 6b64 6972 2070 6167 6573 0a65 6368 6f20  kdir pages.echo 
+000015e0: 2723 204d 7920 4669 7273 7420 506f 7374  '# My First Post
+000015f0: 2720 3e20 6669 7273 742d 706f 7374 2e6d  ' > first-post.m
+00001600: 640a 6563 686f 2027 2320 4865 6c6c 6f20  d.echo '# Hello 
+00001610: 576f 726c 6427 203e 2068 656c 6c6f 2d77  World' > hello-w
+00001620: 6f72 6c64 2e6d 640a 6060 600a 0a23 2323  orld.md.```..###
+00001630: 2042 7569 6c64 2079 6f75 7220 7369 7465   Build your site
+00001640: 0a0a 496e 7374 616c 6c20 6d61 726b 6174  ..Install markat
+00001650: 6120 696e 746f 2079 6f75 7220 7669 7274  a into your virt
+00001660: 7561 6c20 656e 7669 726f 6e6d 656e 7420  ual environment 
+00001670: 616e 6420 7275 6e20 606d 6172 6b61 7461  and run `markata
+00001680: 2062 7569 6c64 602e 2049 7420 7769 6c6c   build`. It will
+00001690: 0a63 7265 6174 6520 796f 7572 2073 6974  .create your sit
+000016a0: 6520 696e 2060 2e2f 6d61 726b 6f75 7460  e in `./markout`
+000016b0: 2c20 6c65 6176 6520 6974 7320 6361 6368  , leave its cach
+000016c0: 6520 696e 2060 2e2f 2e6d 6172 6b61 7461  e in `./.markata
+000016d0: 2e63 6163 6865 602c 2061 6e64 0a63 6f70  .cache`, and.cop
+000016e0: 7920 616c 6c20 6173 7365 7473 2066 726f  y all assets fro
+000016f0: 6d20 602e 2f73 7461 7469 6360 2069 6e74  m `./static` int
+00001700: 6f20 602e 2f6d 6172 6b6f 7574 6020 6279  o `./markout` by
+00001710: 2064 6566 6175 6c74 2e0a 0a60 6060 6261   default...```ba
+00001720: 7368 0a70 7974 686f 6e20 2d6d 2070 6970  sh.python -m pip
+00001730: 2069 6e73 7461 6c6c 206d 6172 6b61 7461   install markata
+00001740: 0a6d 6172 6b61 7461 2062 7569 6c64 0a0a  .markata build..
+00001750: 2320 6f72 2069 6620 7069 7078 2069 7320  # or if pipx is 
+00001760: 796f 7572 2074 6869 6e67 0a70 6970 7820  your thing.pipx 
+00001770: 7275 6e20 6d61 726b 6174 6120 6275 696c  run markata buil
+00001780: 640a 6060 600a 0a23 2323 2042 7569 6c64  d.```..### Build
+00001790: 696e 6720 6120 426c 6f67 2077 6974 6820  ing a Blog with 
+000017a0: 4d61 726b 6174 6120 5f75 7369 6e67 2061  Markata _using a
+000017b0: 2074 656d 706c 6174 655f 0a0a 5468 6520   template_..The 
+000017c0: 6d61 726b 6174 6120 636c 6920 696e 636c  markata cli incl
+000017d0: 7564 6573 2061 2060 6e65 7760 2063 6f6d  udes a `new` com
+000017e0: 6d61 6e64 2074 6861 7420 7769 6c6c 2070  mand that will p
+000017f0: 7265 7365 6e74 2079 6f75 2077 6974 6820  resent you with 
+00001800: 7175 6573 7469 6f6e 730a 746f 2066 696c  questions.to fil
+00001810: 6c20 696e 2074 6865 206a 696e 6a61 2076  l in the jinja v
+00001820: 6172 6961 626c 6573 2069 6e20 7468 6973  ariables in this
+00001830: 2072 6570 6f2e 0a0a 6060 6062 6173 680a   repo...```bash.
+00001840: 6d61 726b 6174 6120 6e65 7720 626c 6f67  markata new blog
+00001850: 205b 6469 7265 6374 6f72 795d 0a0a 2320   [directory]..# 
+00001860: 7374 6172 7420 7468 6520 7369 7465 2061  start the site a
+00001870: 6e64 2077 6174 6368 2066 6f72 2063 6861  nd watch for cha
+00001880: 6e67 6573 0a68 6174 6368 2072 756e 2074  nges.hatch run t
+00001890: 7569 0a60 6060 0a0a 4e6f 7720 6966 2079  ui.```..Now if y
+000018a0: 6f75 206f 7065 6e20 6c6f 6361 6c68 6f73  ou open localhos
+000018b0: 743a 3830 3030 2c20 796f 7520 7769 6c6c  t:8000, you will
+000018c0: 2062 6520 7072 6573 656e 7465 6420 7769   be presented wi
+000018d0: 7468 2061 6e20 6578 616d 706c 6520 7369  th an example si
+000018e0: 7465 2074 6861 740a 7769 6c6c 2077 616c  te that.will wal
+000018f0: 6b20 796f 7520 7468 726f 7567 6820 736f  k you through so
+00001900: 6d65 2066 6561 7475 7265 7320 6f66 206d  me features of m
+00001910: 6172 6b61 7461 2e20 596f 7520 6361 6e20  arkata. You can 
+00001920: 706c 6179 2077 6974 6820 6974 2061 740a  play with it at.
+00001930: 796f 7572 206f 776e 2070 6163 652c 206f  your own pace, o
+00001940: 7220 6472 6f70 2061 6c6c 2074 6865 2070  r drop all the p
+00001950: 6167 6573 2061 6e64 2073 7461 7274 2077  ages and start w
+00001960: 7269 7469 6e67 2079 6f75 7220 6f77 6e20  riting your own 
+00001970: 636f 6e74 656e 742e 0a0a 2323 204d 6f74  content...## Mot
+00001980: 6976 6174 696f 6e0a 0a4d 6172 6b61 7461  ivation..Markata
+00001990: 2069 7320 6162 6c65 2074 6f20 6275 696c   is able to buil
+000019a0: 6420 796f 7572 2073 6974 6520 7075 7265  d your site pure
+000019b0: 6c79 2066 726f 6d20 4d61 726b 646f 776e  ly from Markdown
+000019c0: 2c20 616c 6c6f 7769 6e67 2079 6f75 2074  , allowing you t
+000019d0: 6f20 6765 740a 7374 6172 7465 6420 6372  o get.started cr
+000019e0: 6561 7469 6e67 2079 6f75 7220 6f77 6e20  eating your own 
+000019f0: 636f 6e74 656e 7420 7175 6963 6b6c 792e  content quickly.
+00001a00: 204f 7574 206f 6620 7468 6520 626f 7820   Out of the box 
+00001a10: 6974 2077 696c 6c20 636f 7665 7220 796f  it will cover yo
+00001a20: 7572 0a73 656f 2074 6167 732c 2072 7373  ur.seo tags, rss
+00001a30: 2066 6565 6473 2c20 7369 7465 6d61 702c   feeds, sitemap,
+00001a40: 2061 6e64 206f 6720 696d 6167 6573 2e20   and og images. 
+00001a50: 5369 6e63 6520 6974 2069 7320 6275 696c  Since it is buil
+00001a60: 7420 636f 6d70 6c65 7465 6c79 2066 726f  t completely fro
+00001a70: 6d0a 706c 7567 696e 7320 796f 7520 6361  m.plugins you ca
+00001a80: 6e20 7265 6d6f 7665 2c20 6d6f 6469 6679  n remove, modify
+00001a90: 2c20 6f72 2061 6464 2074 6f20 616e 7920  , or add to any 
+00001aa0: 6f66 2069 7473 2062 6568 6176 696f 722e  of its behavior.
+00001ab0: 0a0a 2d20 636f 6e66 6967 7572 6162 6c65  ..- configurable
+00001ac0: 0a2d 2070 6c75 6769 6e73 0a2d 2073 656f  .- plugins.- seo
+00001ad0: 0a2d 2072 7373 0a2d 2073 6974 656d 6170  .- rss.- sitemap
+00001ae0: 0a2d 206f 672d 696d 6167 650a 0a23 2320  .- og-image..## 
+00001af0: 5573 696e 6720 4d61 726b 6174 610a 0a54  Using Markata..T
+00001b00: 6865 2064 6f63 7320 6172 6520 7374 696c  he docs are stil
+00001b10: 6c20 6120 776f 726b 2069 6e20 7072 6f67  l a work in prog
+00001b20: 7265 7373 2c20 6275 7420 7468 650a 5b62  ress, but the.[b
+00001b30: 6173 655f 636c 695d 2868 7474 7073 3a2f  ase_cli](https:/
+00001b40: 2f6d 6172 6b61 7461 2e64 6576 2f6d 6172  /markata.dev/mar
+00001b50: 6b61 7461 2f70 6c75 6769 6e73 2f62 6173  kata/plugins/bas
+00001b60: 655f 636c 692f 2920 7761 6c6b 7320 7468  e_cli/) walks th
+00001b70: 726f 7567 6820 686f 7720 746f 0a65 6666  rough how to.eff
+00001b80: 6563 7469 7665 6c79 2075 7365 2074 6865  ectively use the
+00001b90: 2060 6d61 726b 6174 6120 6275 696c 6460   `markata build`
+00001ba0: 2063 6f6d 6d61 6e64 2e20 4174 2074 6869   command. At thi
+00001bb0: 7320 706f 696e 7420 4d61 726b 6174 6120  s point Markata 
+00001bc0: 6973 2066 6172 2066 726f 6d0a 7374 6162  is far from.stab
+00001bd0: 6c65 2061 6e64 202a 2a77 696c 6c20 6368  le and **will ch
+00001be0: 616e 6765 2071 7569 7465 2061 2062 6974  ange quite a bit
+00001bf0: 2a2a 2c20 7368 6f75 6c64 2079 6f75 2063  **, should you c
+00001c00: 686f 6f73 6520 746f 2075 7365 2069 7420  hoose to use it 
+00001c10: 6f6e 2072 6561 6c0a 7369 7465 206d 616b  on real.site mak
+00001c20: 6520 7375 7265 2079 6f75 2070 696e 2074  e sure you pin t
+00001c30: 6f20 7468 6520 7665 7273 696f 6e20 7468  o the version th
+00001c40: 6174 2079 6f75 2077 616e 7420 746f 2062  at you want to b
+00001c50: 7569 6c64 2066 726f 6d2e 2049 2077 696c  uild from. I wil
+00001c60: 6c20 6c65 740a 796f 7520 6b6e 6f77 2061  l let.you know a
+00001c70: 7320 6974 2062 6563 6f6d 6573 206d 6f72  s it becomes mor
+00001c80: 6520 7374 6162 6c65 2061 6e64 2072 6561  e stable and rea
+00001c90: 6479 2074 6f20 7573 6520 7769 7468 6f75  dy to use withou
+00001ca0: 7420 6469 6c69 6765 6e63 6520 6f66 0a70  t diligence of.p
+00001cb0: 696e 6e69 6e67 2074 6f20 7468 6520 7665  inning to the ve
+00001cc0: 7273 696f 6e20 796f 7520 7761 6e74 2e0a  rsion you want..
+00001cd0: 0a2a 2a48 6f6e 6573 746c 792a 2a20 4120  .**Honestly** A 
+00001ce0: 6269 6720 6d6f 7469 7661 7469 6f6e 2066  big motivation f
+00001cf0: 6f72 206d 6520 7761 7320 7761 6e74 696e  or me was wantin
+00001d00: 6720 746f 206c 6561 726e 2061 6e64 2075  g to learn and u
+00001d10: 6e64 6572 7374 616e 6420 686f 7720 746f  nderstand how to
+00001d20: 0a63 7265 6174 6520 6120 7072 6f6a 6563  .create a projec
+00001d30: 7420 7468 6174 2069 7320 636f 6d70 6c65  t that is comple
+00001d40: 7465 6c79 2070 6c75 6769 6e20 6472 6976  tely plugin driv
+00001d50: 656e 2e20 5468 6973 2069 7320 6869 6768  en. This is high
+00001d60: 6c79 2061 206c 6561 726e 696e 670a 7072  ly a learning.pr
+00001d70: 6f6a 6563 7420 666f 7220 6d65 2c20 616e  oject for me, an
+00001d80: 6420 6974 2068 6173 2067 726f 776e 2069  d it has grown i
+00001d90: 6e74 6f20 736f 6d65 7468 696e 6720 4920  nto something I 
+00001da0: 7573 6520 6576 6572 7920 6461 792e 0a0a  use every day...
+00001db0: 2323 2045 7861 6d70 6c65 7320 4761 6c6c  ## Examples Gall
+00001dc0: 6172 790a 0a4d 6172 6b61 7461 2068 6173  ary..Markata has
+00001dd0: 2061 2070 726f 6a65 6374 2067 616c 6c65   a project galle
+00001de0: 7279 2074 6f20 7368 6f77 206f 6666 2073  ry to show off s
+00001df0: 6974 6573 2062 7569 6c74 2077 6974 6820  ites built with 
+00001e00: 6d61 726b 6174 612e 2050 6c65 6173 650a  markata. Please.
+00001e10: 5b73 7562 6d69 745d 2868 7474 7073 3a2f  [submit](https:/
+00001e20: 2f67 6974 6875 622e 636f 6d2f 5761 796c  /github.com/Wayl
+00001e30: 6f6e 5761 6c6b 6572 2f6d 6172 6b61 7461  onWalker/markata
+00001e40: 2f69 7373 7565 732f 3738 2920 796f 7572  /issues/78) your
+00001e50: 732c 2061 6e64 2063 6865 636b 0a6f 7574  s, and check.out
+00001e60: 2074 6865 205b 7072 6f6a 6563 742d 6761   the [project-ga
+00001e70: 6c6c 6572 795d 2868 7474 703a 2f2f 6d61  llery](http://ma
+00001e80: 726b 6174 612e 6465 762f 7072 6f6a 6563  rkata.dev/projec
+00001e90: 742d 6761 6c6c 6572 792f 2920 666f 7220  t-gallery/) for 
+00001ea0: 696e 7370 6972 6174 696f 6e2e 0a         inspiration..
```

