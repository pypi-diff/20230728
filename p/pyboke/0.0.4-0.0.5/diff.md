# Comparing `tmp/pyboke-0.0.4.tar.gz` & `tmp/pyboke-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyboke-0.0.4.tar", last modified: Thu Oct 27 15:05:04 2022, max compression
+gzip compressed data, was "pyboke-0.0.5.tar", last modified: Fri Jul 28 11:34:50 2023, max compression
```

## Comparing `pyboke-0.0.4.tar` & `pyboke-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       40 2022-10-15 12:26:28.082356 pyboke-0.0.4/.gitignore
--rw-r--r--   0        0        0     1086 2022-09-06 11:21:58.290993 pyboke-0.0.4/LICENSE
--rw-r--r--   0        0        0    11133 2022-10-26 06:10:45.375980 pyboke-0.0.4/README.md
--rw-r--r--   0        0        0    10006 2022-10-25 11:44:36.747414 pyboke-0.0.4/docs/details.md
--rw-r--r--   0        0        0     2960 2022-10-26 05:45:41.165987 pyboke-0.0.4/docs/jianjie.md
--rw-r--r--   0        0        0      552 2022-09-11 10:40:02.916763 pyboke-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      568 2022-09-06 13:04:56.850613 pyboke-0.0.4/setup.cfg
--rw-r--r--   0        0        0      182 2022-10-27 14:56:18.691296 pyboke-0.0.4/src/pyboke/__init__.py
--rw-r--r--   0        0        0     7582 2022-10-18 12:57:23.220696 pyboke-0.0.4/src/pyboke/main.py
--rw-r--r--   0        0        0     8232 2022-10-15 12:38:22.441893 pyboke-0.0.4/src/pyboke/model.py
--rw-r--r--   0        0        0       29 2022-10-08 02:51:13.451023 pyboke-0.0.4/src/pyboke/templates/.rgignore
--rw-r--r--   0        0        0     7169 2022-04-10 00:57:47.267264 pyboke-0.0.4/src/pyboke/templates/LICENSE.txt
--rw-r--r--   0        0        0     1087 2022-10-14 03:23:40.070259 pyboke-0.0.4/src/pyboke/templates/article.html
--rw-r--r--   0        0        0     1091 2022-10-14 02:09:30.419542 pyboke-0.0.4/src/pyboke/templates/article.toml
--rw-r--r--   0        0        0      858 2022-10-10 03:27:36.697173 pyboke-0.0.4/src/pyboke/templates/atom.xml
--rw-r--r--   0        0        0      746 2022-09-29 15:57:06.879481 pyboke-0.0.4/src/pyboke/templates/base.html
--rw-r--r--   0        0        0     1193 2022-10-14 00:34:30.981330 pyboke-0.0.4/src/pyboke/templates/blog.toml
--rw-r--r--   0        0        0       29 2022-09-28 15:43:55.876806 pyboke-0.0.4/src/pyboke/templates/draft.md
--rw-r--r--   0        0        0      674 2022-10-19 00:40:40.914524 pyboke-0.0.4/src/pyboke/templates/index.html
--rw-r--r--   0        0        0      705 2022-10-14 02:58:31.495381 pyboke-0.0.4/src/pyboke/templates/random.html
--rw-r--r--   0        0        0     1453 2022-10-21 00:38:22.586035 pyboke-0.0.4/src/pyboke/templates/style.css
--rw-r--r--   0        0        0     6648 2022-04-11 02:30:02.576648 pyboke-0.0.4/src/pyboke/templates/themes/mvp.css
--rw-r--r--   0        0        0     4524 2022-04-10 13:26:10.230508 pyboke-0.0.4/src/pyboke/templates/themes/new.css
--rw-r--r--   0        0        0     6113 2022-04-02 13:19:46.562534 pyboke-0.0.4/src/pyboke/templates/themes/simple.css
--rw-r--r--   0        0        0    22747 2022-04-10 08:23:19.933466 pyboke-0.0.4/src/pyboke/templates/themes/water.css
--rw-r--r--   0        0        0      677 2022-09-30 02:11:43.995685 pyboke-0.0.4/src/pyboke/templates/title-index.html
--rw-r--r--   0        0        0      429 2022-09-30 02:11:19.275141 pyboke-0.0.4/src/pyboke/templates/years.html
--rw-r--r--   0        0        0    11724 2022-10-18 12:56:58.368130 pyboke-0.0.4/src/pyboke/tmpl_render.py
--rw-r--r--   0        0        0     6214 2022-10-27 14:57:37.251731 pyboke-0.0.4/src/pyboke/util.py
--rw-r--r--   0        0        0    11323 1970-01-01 00:00:00.000000 pyboke-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       44 2023-07-10 02:01:58.401276 pyboke-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1086 2023-07-10 02:01:58.401276 pyboke-0.0.5/LICENSE
+-rw-r--r--   0        0        0    11851 2023-07-10 02:01:58.401276 pyboke-0.0.5/README.md
+-rw-r--r--   0        0        0    10218 2023-07-10 02:01:58.401276 pyboke-0.0.5/docs/details.md
+-rw-r--r--   0        0        0     2960 2023-07-10 02:01:58.401276 pyboke-0.0.5/docs/jianjie.md
+-rw-r--r--   0        0        0      580 2023-07-10 02:01:58.401276 pyboke-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      593 2023-07-10 02:01:58.401276 pyboke-0.0.5/setup.cfg
+-rw-r--r--   0        0        0      188 2023-07-28 11:23:42.100851 pyboke-0.0.5/src/pyboke/__init__.py
+-rw-r--r--   0        0        0     7876 2023-07-10 02:01:58.401276 pyboke-0.0.5/src/pyboke/main.py
+-rw-r--r--   0        0        0     8490 2023-07-28 11:20:03.097406 pyboke-0.0.5/src/pyboke/model.py
+-rw-r--r--   0        0        0       31 2023-07-10 02:01:58.401276 pyboke-0.0.5/src/pyboke/templates/.rgignore
+-rw-r--r--   0        0        0     7169 2023-07-10 02:01:58.401276 pyboke-0.0.5/src/pyboke/templates/LICENSE.txt
+-rw-r--r--   0        0        0     1192 2023-07-28 11:21:27.434352 pyboke-0.0.5/src/pyboke/templates/article.html
+-rw-r--r--   0        0        0     1133 2023-07-10 02:01:58.401276 pyboke-0.0.5/src/pyboke/templates/article.toml
+-rw-r--r--   0        0        0      889 2023-07-10 02:01:58.401276 pyboke-0.0.5/src/pyboke/templates/atom.xml
+-rw-r--r--   0        0        0      779 2023-07-10 02:01:58.401276 pyboke-0.0.5/src/pyboke/templates/base.html
+-rw-r--r--   0        0        0     1234 2023-07-10 02:01:58.401276 pyboke-0.0.5/src/pyboke/templates/blog.toml
+-rw-r--r--   0        0        0       32 2023-07-10 02:01:58.401276 pyboke-0.0.5/src/pyboke/templates/draft.md
+-rw-r--r--   0        0        0      709 2023-07-10 02:01:58.401276 pyboke-0.0.5/src/pyboke/templates/index.html
+-rw-r--r--   0        0        0      741 2023-07-10 02:01:58.401276 pyboke-0.0.5/src/pyboke/templates/random.html
+-rw-r--r--   0        0        0     1453 2023-07-10 02:01:58.401276 pyboke-0.0.5/src/pyboke/templates/style.css
+-rw-r--r--   0        0        0     6654 2023-07-10 02:01:58.401276 pyboke-0.0.5/src/pyboke/templates/themes/mvp.css
+-rw-r--r--   0        0        0     4524 2023-07-10 02:01:58.401276 pyboke-0.0.5/src/pyboke/templates/themes/new.css
+-rw-r--r--   0        0        0     6113 2023-07-10 02:01:58.401276 pyboke-0.0.5/src/pyboke/templates/themes/simple.css
+-rw-r--r--   0        0        0    22747 2023-07-10 02:01:58.416860 pyboke-0.0.5/src/pyboke/templates/themes/water.css
+-rw-r--r--   0        0        0      711 2023-07-10 02:01:58.416948 pyboke-0.0.5/src/pyboke/templates/title-index.html
+-rw-r--r--   0        0        0      448 2023-07-10 02:01:58.417489 pyboke-0.0.5/src/pyboke/templates/years.html
+-rw-r--r--   0        0        0    12098 2023-07-10 02:01:58.417489 pyboke-0.0.5/src/pyboke/tmpl_render.py
+-rw-r--r--   0        0        0     6402 2023-07-10 02:01:58.417489 pyboke-0.0.5/src/pyboke/util.py
+-rw-r--r--   0        0        0    12025 1970-01-01 00:00:00.000000 pyboke-0.0.5/PKG-INFO
```

### Comparing `pyboke-0.0.4/LICENSE` & `pyboke-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyboke-0.0.4/README.md` & `pyboke-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,44 +26,47 @@
 推荐使用 [pyenv](https://github.com/pyenv/pyenv) 或
 [miniconda](https://docs.conda.io/en/latest/miniconda.html)
 来安装最新版本的 Python。
 
 例如，安装 miniconda 后，可以这样创建 3.10 环境：
 
 ```sh
-$ conda create --name py310 python=3.10
+$ conda create --name py310 python=3.10.6
 $ conda activate py310
 ```
 
 安装非常简单，只要 `pip install pyboke` 即可。  
-另外推荐采用 [pipx](https://pypa.github.io/pipx/) 进行安装。
+
+(另外推荐了解一下 [pipx](https://pypa.github.io/pipx/)
+这是用来安装 Python 命令行软件的优秀工具）
 
 ## 创建一个新博客
 
 1. `mkdir my-blog` _(新建一个空文件夹)_
 2. `cd my-blog` _(进入空文件夹内)_
-3. `boke init` _(初始化博客，创建一些必要的文件和文件夹)_
+3. `boke init` _(初始化博客)_
 
-然后可以在当前文件内看到以下文件与文件夹：
+成功后，可以在当前文件夹内看到以下文件与文件夹：
 
 - **articles** (全部文章都在这里，采用 markdown 格式, `.md` 后缀名)
 - **articles/metadata** (与 markdown 文件一一对应的 toml 文件)
 - **drafts** (待发布的草稿放在这里)
 - **output** (程序生成的 HTML, RSS 等文件将会输出到该文件夹)
 - **templates** (Jinja2模板 与 CSS文件)
-- **boke.toml** (博客名称、作者名称等)
+- **blog.toml** (博客名称、作者名称等)
 
-请用文本编辑器打开 boke.toml 填写博客名称、作者名称等。
+请用文本编辑器打开 blog.toml 填写博客名称、作者名称等。
 
 执行命令 `boke -info` 查看博客信息。
 
 ## 添加文章
 
 - 文件后缀必须是 ".md", 文件内容必须采用 Markdown 格式, 使用 utf-8 编码。
 - 文件名只能使用 0-9, a-z, A-Z, _(下划线), -(短横线), .(点)。
+- 文件名会成为网址的一部分, 因此建议尽量短一点.
 - 把 md 文件放入 articles 文件夹，执行 `boke render articles/filename`,
   会在 **articles/metadata** 文件夹里生成 TOML 文件，
   在 **output** 文件夹生成 HTML 文件。
 - 其中, TOML 里有文章的标题、作者、创建日期、修改日期等信息。
 - 大多数情况下你都可以忘记 articles/metadata 里的 toml 文件，不需要修改它。
 - 推荐使用 `boke new` 和 `boke post` 命令，详见后文 **草稿** 部分。
 
@@ -246,14 +249,27 @@
 
 例如可以使用 [ripgrep](https://github.com/BurntSushi/ripgrep), 在博客的根目录执行
 `rg -i 'keyword' articles` 即可查找包含 `keyword` 的文章，其中 `-i` 表示不分大小写。
 
 如果不搜索文章正文内容，只搜索文章标题，可打开网页 title-index.html(标题索引),
 按 `Ctrl+F` 在页面内搜索。
 
+## 建议使用终端文本编辑器
+
+本软件的大部分操作都需要在终端输入命令, 有时需要稍稍修改一下 toml,
+这种情况下如果切换到文本编辑器去操作, 会感觉有点麻烦, 因此建议使用类似
+Vim/Emacs 的终端文本编辑器, 就很方便.
+
+我找到了 [micro](https://github.com/zyedidia/micro), 它类似 Vim/Emacs
+并且更轻, 也更易学易用, 优点:
+
+- 启动速度飞快, 感觉非常轻巧.
+- 非常易学易用, 支持鼠标选择, 以及用 Ctrl-C / Ctrl-V 来复制黏贴.  
+  支持 Ctrl-S 保存 / Ctrl-A 全选等符合现代习惯的快捷键.
+
 
 [^css-themes]: 例如这里就有一些极简 CSS 主题: [github.com/dohliam/dropin-minimal-css](https://github.com/dohliam/dropin-minimal-css)
 
 ## 我的博客
 
 作为参考，可以看看我的博客，就是用 PyBoke 生成的。
 <https://ahui2016.github.io/>
```

### Comparing `pyboke-0.0.4/docs/details.md` & `pyboke-0.0.5/docs/details.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,212 +1,212 @@
-# PyBoke
-
-Static Blog Generator (极简博客生成器)
-
-- 使用过程极简
-- 功能极简，代码极简
-
-因为功能少、代码简单，任何懂编程的人（只要懂 Python 基础）
-就能在短时间内完全看明白本软件的全部代码并且随心所欲地修改。
-
-- 文章文件名、图片文件名由用户设定，只允许使用 0-9, a-z, A-Z, _(下划线), -(短横线), .(点)。
-- 文章文件名、图片文件名相当于 ID
-
-## 三个维度管理文章
-
-- 管理博客文章的最常见的思维是通过 "类别", "标签", "日期" 三个维度来实现
-- 本软件的第一版也是这样做的，花了很多时间精力几乎全部功能都实现时
-  (甚至还用 PyQt 做了一些 GUI), 又全部推倒重做，因为发现了新的文章管理方法。
-
-### "类别", "标签", "日期" 的缺点
-
-- 这套方法有很多优点，因此才会流行，但也有缺点。
-- 我认为缺点是用户发布文章时，每次都要选择分类、填标签，产生额外的心智负担。
-- 而且处理这些功能，要写很多代码。
-
-### 新的灵感
-
-- 最近我在做一个小工具的过程中，突然想到了一种管理文章的简单方法：首字符索引。
-- 这是一种很古老的方法了，纸质书年代曾被广泛采用，英文书经常会在书末列出索引。
-- 特别是当预估文章数量不会很多的时候（一般个人博客文章不多），这种方法是够用的。
-  虽然最终的效果不如类别+标签，但也勉强够用。
-- 而且有两大优点：
-  1. 用户发布文章时，直接发布！不需要选择类别、不需要填写标签，非常畅快。
-  2. 代码量大幅减少！程序简单了很多很多，这我可太高兴了，同时对于懂编程的用户来说，
-     阅读或修改这个项目的代码也非常轻松。
-
-### 三个维度发现文章
-
-- 经过上述思考，我的思维从 "三个维度**管理**文章" 变成 "三个维度**发现**文章"。
-- 管理的目的是使文章井井有条，但我发现我真正担心的并不是文章是否排列整齐，而是
-  如何让读者（或我自己）从旧文章中挑选一些文章来看，避免旧文章被埋没。
-- 因此，我只要提供一些**发现**文章的维度即可，不需要强迫用户（作者）花时间精力去**管理**。
-- 结果，我的博客不提供传统的 "类别", "标签", "日期", 而是提供 "标题索引", "日期", "随机"。
-- 我相信，对于文章数量不会很多的个人博客来说, "标题索引", "日期", "随机" 已经够用了，
-  同时使代码大幅减少，使用过程也很畅快，这个 trade-off 是值得的。
-
-## 一大特点：添加/修改/删除文章都非常方便
-
-1. 添加文章：直接在 articles 文件夹里新建 '.md' 后缀名的文件，采用 markdown 格式编写内容。
-2. 修改文章：直接修改 articles 文件夹里的文件。
-3. 删除文章：直接删除 articles 文件夹里的文件。
-4. 执行命令 `boke render -all`
-
-进一步说明究竟有多简单：
-
-- 添加文章时，不需要在任何地方填写文章标题、标签、日期、作者姓名…… 这些全部都不用管，只管写文章。
-- 可以在添加/修改了一篇或多篇文章后，包括删除一些文章后，再统一执行 `boke render -all` 即可。
-
-## 创建一个新博客
-
-1. `mkdir my-blog` (新建一个空文件夹)
-2. `cd my-blog` (进入空文件夹内)
-3. `boke init` (如果检测到文件夹不是空的，会拒绝初始化)
-
-然后可以在当前文件内看到以下文件与文件夹：
-
-- articles (文章文件 (markdown 格式, .md 后缀名) 请放在这里)
-- articles/pics (供 markdown 文件使用的本地图片)
-- articles/metadata (与 markdown 文件一一对应的 toml 文件)
-- drafts (待发布的草稿放在这里)
-- output (程序生成的 HTML, RSS 等文件将会输出到该文件夹)
-- templates (Jinja2模板 与 CSS文件)
-- boke.toml (博客名称、作者名称等等)
-
-请用文本编辑器打开 boke.toml 填写博客名称、作者名称等。
-
-建议尽量少用图片，本程序未为大量图片做优化。
-
-## 添加文章
-
-- 文件后缀必须是 ".md", 文件内容必须采用 Markdown 格式, 必须采用 utf-8 编码。
-- 文件名只能使用 0-9, a-z, A-Z, _(下划线), -(短横线), .(点)。
-- 把 md 文件放入 articles 文件夹，执行 `boke render articles/filename`,
-  会在 **articles/metadata** 文件夹里生成 TOML 文件，
-  在 **output** 文件夹生成 HTML 文件。
-- 其中, TOML 里有文章的标题、作者、创建日期、修改日期等信息。
-- 大多数情况下你都可以忘记 articles/metadata 里的 toml 文件，不需要修改它。
-
-## 修改文章内容
-
-- 直接修改 articles 里的 md 文件。
-- 然后执行 `boke render articles/filename`, 即可自动更新指定文件的 toml 和 html
-- 该命令与前面所述 "添加文章" 的命令是一样的，作用都是渲染 toml 和 html
-
-## 批量处理
-
-- 执行 `boke render -all` 可自动检查全部文件是否被修改过，如有则更新其 toml 和 html
-  (如有新文章，也会自动生成 toml 和 html)。
-
-## 强制渲染
-
-使用前述的 `boke render` 命令时，如果文章内容无变化，会自动忽略。  
-也就是说，如果只修改 toml 的内容，不修改 markdown 文件的内容，就不会触发渲染处理。
-
-因此，如果想在不修改文章内容的情况下，修改文章的作者或日期，就需要强制渲染。
-
-- `boke render -force articles/filename` 强制渲染指定的一篇文章。
-- `boke render --title-index` 强制渲染全部标题索引（在发现未触发更新时使用）
-- `boke render -force -all` 强制渲全部文章。
-
-大多数情况下不需要强制渲染，但有一种情况：修改了 blog.toml 里的博客名称、作者名称
-等信息后，需要执行 `boke render -force -all` 强制渲全部文章。
-
-### 手动更新文章创建日期
-
-如果想修改一篇文章的创建日期，可手动修改该文章的 toml 文件中的 ctime,
-然后执行命令 `boke render -years`
-
-### 手动更新文章修改日期
-
-如果修改了文章的内容，在执行上述 `boke render` 相关命令时会自动更新文章的修改日期。
-
-如果想手动设定一篇文章的修改日期，可手动修改该文章的 toml 文件中的 mtime,
-然后执行命令 `boke render articles/XXX.md -force`
-
-## 删除文章
-
-有两种方法：
-
-1. 使用命令 `boke delete articles/filename`
-2. 直接删除 articles 文件夹里的文件，然后执行 `boke render -all`
-
-## RSS
-
-注意，在正式对外发布你的博客时，请在 blog.toml 中填写你的博客网址 (website),
-第一次生成 atom.xml 需要执行 `boke render -rss`,
-后续在执行其它命令时会自动重新渲染 atom.xml
-
-只有执行 `boke render -rss` 才会强制更新 atom.xml, 其他任何情况下都是自动更新。
-
-本软件只提供有限的 RSS 功能：
-
-1. 只包含最新发布的 10 篇文章（并且该数字写死在代码里，用户不能自由设定）
-2. 只包含内容摘要，不包含全文
-
-## 草稿
-
-如上文所示，添加文章只需要把 markdown 文件放进 articles 文件夹即可，
-操作非常简单明瞭。
-
-但考虑到有时文章写到一半不想发布，需要一个存放草稿的地方，因此提供了一个
-drafts 文件夹，草稿可以放在这里。（但其实草稿放在硬盘里的其它文件夹也行，
-这个 drafts 文件夹只是提供方便，并非强制要求）
-
-### `boke new drafts/abc.md`
-
-该命令用来新建一个 markdown 文件，并确保其采用 UTF-8 编码。  
-这个命令也只是提供方便，你完全可以不使用该命令，而是自己用其它方法创建文件。
-
-### `boke post drafts/abc.md`
-
-该命令的作用是把 drafts 文件夹里的指定文件移动到 articles 文件夹里，并对其执行渲染
-(生成 toml 和 html 文件)。
-
-这个命令也只是提供方便，你完全可以不使用该命令，而是自己移动文件，然后自己执行
-`boke render` 命令。
-
-### 提醒：小心覆盖文件
-
-在终端用 `cp` 命令复制文件到 articles 文件夹，或使用 `mv` 命令更改文件名时，
-如有同名文件，会直接覆盖。
-
-因此建议用 `boke post` 命令和 `boke rename` 命令，可以防止覆盖。  
-(注意: 由于涉及文件移动, `boke post` 只能用来发布 drafts 文件夹里的文章。)
-
-例: `boke post drafts/abc.md`
-
-### 更改文件名
-
-更改 articles 文件夹内的文件名时，必须同时更改对应的 toml 及 html 的文件名。
-
-建议使用 `boke rename` 命令，可自动更改对应的 toml 及 html 的文件名。
-
-- 例: `boke rename articles/old-name.md articles/new-name.md`
-- 或: `boke rename articles/old-name.md new-name.md`
-
-## Preview (预览)
-
-- 预览是指将一个 Markdown 文件转换为 HTML, 输出文件名固定为 output/temp.html
-- 预览并非发布文章或修改文章，不会对博客产生任何修改。
-
-- 例: `boke render darfts/abc.md -preview`
-- 或: `boke render articles/abc.md -preview`
-
-## Themes (主题)
-
-- 主题名称只能由英文字母组成，不分大小写，不可包含空格。
-
-## 替换图片地址
-
-- 在 markdown 中可使用 `![photo-1](../output/pics/XXX.jpg)` 的形式插入图片。
-- 本地图片建议放在 output/pics 文件夹内。
-- 图片文件名建议使用半角英文数字，尽量不使用中文和特殊字符
-- 在每篇文章对应的 toml 文件的 pairs 项目里，可指定图片的替换地址，比如：
-  ```toml
-  pairs =  [
-    [ '''../output/pics/abc.jpg''', '''https://example.com/abc.jpg''' ],
-  ]
-  ```
-- markdown 文件的内容保持不变, HTML 文件中如有第一个字符串，会被替代为第二个字符串。
-- 不只是图片地址，该功能可以替换任何字符，但主要用途是替换图片地址。
-- HTML 显示图片的宽度上限可以统一设定，详见 blog.toml 及文章对应的 toml。
+# PyBoke
+
+Static Blog Generator (极简博客生成器)
+
+- 使用过程极简
+- 功能极简，代码极简
+
+因为功能少、代码简单，任何懂编程的人（只要懂 Python 基础）
+就能在短时间内完全看明白本软件的全部代码并且随心所欲地修改。
+
+- 文章文件名、图片文件名由用户设定，只允许使用 0-9, a-z, A-Z, _(下划线), -(短横线), .(点)。
+- 文章文件名、图片文件名相当于 ID
+
+## 三个维度管理文章
+
+- 管理博客文章的最常见的思维是通过 "类别", "标签", "日期" 三个维度来实现
+- 本软件的第一版也是这样做的，花了很多时间精力几乎全部功能都实现时
+  (甚至还用 PyQt 做了一些 GUI), 又全部推倒重做，因为发现了新的文章管理方法。
+
+### "类别", "标签", "日期" 的缺点
+
+- 这套方法有很多优点，因此才会流行，但也有缺点。
+- 我认为缺点是用户发布文章时，每次都要选择分类、填标签，产生额外的心智负担。
+- 而且处理这些功能，要写很多代码。
+
+### 新的灵感
+
+- 最近我在做一个小工具的过程中，突然想到了一种管理文章的简单方法：首字符索引。
+- 这是一种很古老的方法了，纸质书年代曾被广泛采用，英文书经常会在书末列出索引。
+- 特别是当预估文章数量不会很多的时候（一般个人博客文章不多），这种方法是够用的。
+  虽然最终的效果不如类别+标签，但也勉强够用。
+- 而且有两大优点：
+  1. 用户发布文章时，直接发布！不需要选择类别、不需要填写标签，非常畅快。
+  2. 代码量大幅减少！程序简单了很多很多，这我可太高兴了，同时对于懂编程的用户来说，
+     阅读或修改这个项目的代码也非常轻松。
+
+### 三个维度发现文章
+
+- 经过上述思考，我的思维从 "三个维度**管理**文章" 变成 "三个维度**发现**文章"。
+- 管理的目的是使文章井井有条，但我发现我真正担心的并不是文章是否排列整齐，而是
+  如何让读者（或我自己）从旧文章中挑选一些文章来看，避免旧文章被埋没。
+- 因此，我只要提供一些**发现**文章的维度即可，不需要强迫用户（作者）花时间精力去**管理**。
+- 结果，我的博客不提供传统的 "类别", "标签", "日期", 而是提供 "标题索引", "日期", "随机"。
+- 我相信，对于文章数量不会很多的个人博客来说, "标题索引", "日期", "随机" 已经够用了，
+  同时使代码大幅减少，使用过程也很畅快，这个 trade-off 是值得的。
+
+## 一大特点：添加/修改/删除文章都非常方便
+
+1. 添加文章：直接在 articles 文件夹里新建 '.md' 后缀名的文件，采用 markdown 格式编写内容。
+2. 修改文章：直接修改 articles 文件夹里的文件。
+3. 删除文章：直接删除 articles 文件夹里的文件。
+4. 执行命令 `boke render -all`
+
+进一步说明究竟有多简单：
+
+- 添加文章时，不需要在任何地方填写文章标题、标签、日期、作者姓名…… 这些全部都不用管，只管写文章。
+- 可以在添加/修改了一篇或多篇文章后，包括删除一些文章后，再统一执行 `boke render -all` 即可。
+
+## 创建一个新博客
+
+1. `mkdir my-blog` (新建一个空文件夹)
+2. `cd my-blog` (进入空文件夹内)
+3. `boke init` (如果检测到文件夹不是空的，会拒绝初始化)
+
+然后可以在当前文件内看到以下文件与文件夹：
+
+- articles (文章文件 (markdown 格式, .md 后缀名) 请放在这里)
+- articles/pics (供 markdown 文件使用的本地图片)
+- articles/metadata (与 markdown 文件一一对应的 toml 文件)
+- drafts (待发布的草稿放在这里)
+- output (程序生成的 HTML, RSS 等文件将会输出到该文件夹)
+- templates (Jinja2模板 与 CSS文件)
+- blog.toml (博客名称、作者名称等等)
+
+请用文本编辑器打开 blog.toml 填写博客名称、作者名称等。
+
+建议尽量少用图片，本程序未为大量图片做优化。
+
+## 添加文章
+
+- 文件后缀必须是 ".md", 文件内容必须采用 Markdown 格式, 必须采用 utf-8 编码。
+- 文件名只能使用 0-9, a-z, A-Z, _(下划线), -(短横线), .(点)。
+- 把 md 文件放入 articles 文件夹，执行 `boke render articles/filename`,
+  会在 **articles/metadata** 文件夹里生成 TOML 文件，
+  在 **output** 文件夹生成 HTML 文件。
+- 其中, TOML 里有文章的标题、作者、创建日期、修改日期等信息。
+- 大多数情况下你都可以忘记 articles/metadata 里的 toml 文件，不需要修改它。
+
+## 修改文章内容
+
+- 直接修改 articles 里的 md 文件。
+- 然后执行 `boke render articles/filename`, 即可自动更新指定文件的 toml 和 html
+- 该命令与前面所述 "添加文章" 的命令是一样的，作用都是渲染 toml 和 html
+
+## 批量处理
+
+- 执行 `boke render -all` 可自动检查全部文件是否被修改过，如有则更新其 toml 和 html
+  (如有新文章，也会自动生成 toml 和 html)。
+
+## 强制渲染
+
+使用前述的 `boke render` 命令时，如果文章内容无变化，会自动忽略。  
+也就是说，如果只修改 toml 的内容，不修改 markdown 文件的内容，就不会触发渲染处理。
+
+因此，如果想在不修改文章内容的情况下，修改文章的作者或日期，就需要强制渲染。
+
+- `boke render -force articles/filename` 强制渲染指定的一篇文章。
+- `boke render --title-index` 强制渲染全部标题索引（在发现未触发更新时使用）
+- `boke render -force -all` 强制渲全部文章。
+
+大多数情况下不需要强制渲染，但有一种情况：修改了 blog.toml 里的博客名称、作者名称
+等信息后，需要执行 `boke render -force -all` 强制渲全部文章。
+
+### 手动更新文章创建日期
+
+如果想修改一篇文章的创建日期，可手动修改该文章的 toml 文件中的 ctime,
+然后执行命令 `boke render -years`
+
+### 手动更新文章修改日期
+
+如果修改了文章的内容，在执行上述 `boke render` 相关命令时会自动更新文章的修改日期。
+
+如果想手动设定一篇文章的修改日期，可手动修改该文章的 toml 文件中的 mtime,
+然后执行命令 `boke render articles/XXX.md -force`
+
+## 删除文章
+
+有两种方法：
+
+1. 使用命令 `boke delete articles/filename`
+2. 直接删除 articles 文件夹里的文件，然后执行 `boke render -all`
+
+## RSS
+
+注意，在正式对外发布你的博客时，请在 blog.toml 中填写你的博客网址 (website),
+第一次生成 atom.xml 需要执行 `boke render -rss`,
+后续在执行其它命令时会自动重新渲染 atom.xml
+
+只有执行 `boke render -rss` 才会强制更新 atom.xml, 其他任何情况下都是自动更新。
+
+本软件只提供有限的 RSS 功能：
+
+1. 只包含最新发布的 10 篇文章（并且该数字写死在代码里，用户不能自由设定）
+2. 只包含内容摘要，不包含全文
+
+## 草稿
+
+如上文所示，添加文章只需要把 markdown 文件放进 articles 文件夹即可，
+操作非常简单明瞭。
+
+但考虑到有时文章写到一半不想发布，需要一个存放草稿的地方，因此提供了一个
+drafts 文件夹，草稿可以放在这里。（但其实草稿放在硬盘里的其它文件夹也行，
+这个 drafts 文件夹只是提供方便，并非强制要求）
+
+### `boke new drafts/abc.md`
+
+该命令用来新建一个 markdown 文件，并确保其采用 UTF-8 编码。  
+这个命令也只是提供方便，你完全可以不使用该命令，而是自己用其它方法创建文件。
+
+### `boke post drafts/abc.md`
+
+该命令的作用是把 drafts 文件夹里的指定文件移动到 articles 文件夹里，并对其执行渲染
+(生成 toml 和 html 文件)。
+
+这个命令也只是提供方便，你完全可以不使用该命令，而是自己移动文件，然后自己执行
+`boke render` 命令。
+
+### 提醒：小心覆盖文件
+
+在终端用 `cp` 命令复制文件到 articles 文件夹，或使用 `mv` 命令更改文件名时，
+如有同名文件，会直接覆盖。
+
+因此建议用 `boke post` 命令和 `boke rename` 命令，可以防止覆盖。  
+(注意: 由于涉及文件移动, `boke post` 只能用来发布 drafts 文件夹里的文章。)
+
+例: `boke post drafts/abc.md`
+
+### 更改文件名
+
+更改 articles 文件夹内的文件名时，必须同时更改对应的 toml 及 html 的文件名。
+
+建议使用 `boke rename` 命令，可自动更改对应的 toml 及 html 的文件名。
+
+- 例: `boke rename articles/old-name.md articles/new-name.md`
+- 或: `boke rename articles/old-name.md new-name.md`
+
+## Preview (预览)
+
+- 预览是指将一个 Markdown 文件转换为 HTML, 输出文件名固定为 output/temp.html
+- 预览并非发布文章或修改文章，不会对博客产生任何修改。
+
+- 例: `boke render darfts/abc.md -preview`
+- 或: `boke render articles/abc.md -preview`
+
+## Themes (主题)
+
+- 主题名称只能由英文字母组成，不分大小写，不可包含空格。
+
+## 替换图片地址
+
+- 在 markdown 中可使用 `![photo-1](../output/pics/XXX.jpg)` 的形式插入图片。
+- 本地图片建议放在 output/pics 文件夹内。
+- 图片文件名建议使用半角英文数字，尽量不使用中文和特殊字符
+- 在每篇文章对应的 toml 文件的 pairs 项目里，可指定图片的替换地址，比如：
+  ```toml
+  pairs =  [
+    [ '''../output/pics/abc.jpg''', '''https://example.com/abc.jpg''' ],
+  ]
+  ```
+- markdown 文件的内容保持不变, HTML 文件中如有第一个字符串，会被替代为第二个字符串。
+- 不只是图片地址，该功能可以替换任何字符，但主要用途是替换图片地址。
+- HTML 显示图片的宽度上限可以统一设定，详见 blog.toml 及文章对应的 toml。
```

### Comparing `pyboke-0.0.4/docs/jianjie.md` & `pyboke-0.0.5/docs/jianjie.md`

 * *Files identical despite different names*

### Comparing `pyboke-0.0.4/setup.cfg` & `pyboke-0.0.5/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 7079 626f 6b65 0a76 6572 7369 6f6e  = pyboke.version
-00000020: 203d 2061 7474 723a 2070 7962 6f6b 652e   = attr: pyboke.
-00000030: 5f5f 7665 7273 696f 6e5f 5f0a 6175 7468  __version__.auth
-00000040: 6f72 203d 2061 6875 690a 6175 7468 6f72  or = ahui.author
-00000050: 5f65 6d61 696c 203d 2031 3032 3431 3940  _email = 102419@
-00000060: 676d 6169 6c2e 636f 6d0a 6465 7363 7269  gmail.com.descri
-00000070: 7074 696f 6e20 3d20 5079 426f 6b65 3a20  ption = PyBoke: 
-00000080: 4120 7369 6d70 6c65 2073 7461 7469 6320  A simple static 
-00000090: 626c 6f67 2067 656e 6572 6174 6f72 2e0a  blog generator..
-000000a0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000b0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
-000000c0: 6d64 0a6c 6f6e 675f 6465 7363 7269 7074  md.long_descript
-000000d0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-000000e0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-000000f0: 0a75 726c 203d 2068 7474 7073 3a2f 2f67  .url = https://g
-00000100: 6974 6875 622e 636f 6d2f 6168 7569 3230  ithub.com/ahui20
-00000110: 3136 2f70 7962 6f6b 650a 636c 6173 7369  16/pyboke.classi
-00000120: 6669 6572 7320 3d0a 2020 2020 5072 6f67  fiers =.    Prog
-00000130: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000140: 203a 3a20 5079 7468 6f6e 203a 3a20 330a   :: Python :: 3.
-00000150: 2020 2020 4c69 6365 6e73 6520 3a3a 204f      License :: O
-00000160: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
-00000170: 4954 204c 6963 656e 7365 0a20 2020 204f  IT License.    O
-00000180: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000190: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-000001a0: 740a 0a5b 6f70 7469 6f6e 735d 0a70 6163  t..[options].pac
-000001b0: 6b61 6765 5f64 6972 203d 0a20 2020 203d  kage_dir =.    =
-000001c0: 2073 7263 0a70 7974 686f 6e5f 7265 7175   src.python_requ
-000001d0: 6972 6573 203d 203e 3d33 2e31 300a 7061  ires = >=3.10.pa
-000001e0: 636b 6167 6573 203d 2066 696e 643a 0a0a  ckages = find:..
-000001f0: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000200: 732e 6669 6e64 5d0a 7768 6572 6520 3d20  s.find].where = 
-00000210: 7372 630a 0a5b 666c 616b 6538 5d0a 6967  src..[flake8].ig
-00000220: 6e6f 7265 203d 2045 3230 332c 2045 3530  nore = E203, E50
-00000230: 312c 2057 3530 330a                      1, W503.
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 2070 7962 6f6b 650d 0a76 6572 7369   = pyboke..versi
+00000020: 6f6e 203d 2061 7474 723a 2070 7962 6f6b  on = attr: pybok
+00000030: 652e 5f5f 7665 7273 696f 6e5f 5f0d 0a61  e.__version__..a
+00000040: 7574 686f 7220 3d20 6168 7569 0d0a 6175  uthor = ahui..au
+00000050: 7468 6f72 5f65 6d61 696c 203d 2031 3032  thor_email = 102
+00000060: 3431 3940 676d 6169 6c2e 636f 6d0d 0a64  419@gmail.com..d
+00000070: 6573 6372 6970 7469 6f6e 203d 2050 7942  escription = PyB
+00000080: 6f6b 653a 2041 2073 696d 706c 6520 7374  oke: A simple st
+00000090: 6174 6963 2062 6c6f 6720 6765 6e65 7261  atic blog genera
+000000a0: 746f 722e 0d0a 6c6f 6e67 5f64 6573 6372  tor...long_descr
+000000b0: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
+000000c0: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
+000000d0: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
+000000e0: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
+000000f0: 6172 6b64 6f77 6e0d 0a75 726c 203d 2068  arkdown..url = h
+00000100: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000110: 6d2f 6168 7569 3230 3136 2f70 7962 6f6b  m/ahui2016/pybok
+00000120: 650d 0a63 6c61 7373 6966 6965 7273 203d  e..classifiers =
+00000130: 0d0a 2020 2020 5072 6f67 7261 6d6d 696e  ..    Programmin
+00000140: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000150: 7468 6f6e 203a 3a20 330d 0a20 2020 204c  thon :: 3..    L
+00000160: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+00000170: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+00000180: 6365 6e73 650d 0a20 2020 204f 7065 7261  cense..    Opera
+00000190: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
+000001a0: 5320 496e 6465 7065 6e64 656e 740d 0a0d  S Independent...
+000001b0: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
+000001c0: 6167 655f 6469 7220 3d0d 0a20 2020 203d  age_dir =..    =
+000001d0: 2073 7263 0d0a 7079 7468 6f6e 5f72 6571   src..python_req
+000001e0: 7569 7265 7320 3d20 3e3d 332e 3130 0d0a  uires = >=3.10..
+000001f0: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+00000200: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
+00000210: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
+00000220: 7265 203d 2073 7263 0d0a 0d0a 5b66 6c61  re = src....[fla
+00000230: 6b65 385d 0d0a 6967 6e6f 7265 203d 2045  ke8]..ignore = E
+00000240: 3230 332c 2045 3530 312c 2057 3530 330d  203, E501, W503.
+00000250: 0a                                       .
```

### Comparing `pyboke-0.0.4/src/pyboke/model.py` & `pyboke-0.0.5/src/pyboke/model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,234 +1,234 @@
-import hashlib
-import re
-from dataclasses import dataclass, asdict
-from pathlib import Path
-
-import arrow
-import tomli
-
-# 注意: model.py 在最底层，不能 import util.py, tmpl_render.py, 更不能 import main.py
-
-RFC3339               = "YYYY-MM-DD HH:mm:ssZZ"
-Blog_Config_Filename  = "blog.toml"
-Drafts_Folder_Name    = "drafts"
-Draft_TMPL_Name       = "draft.md"
-Articles_Folder_Name  = "articles"
-Pics_Folder_Name      = "pics"
-Metadata_Folder_Name  = "metadata"
-Output_Folder_Name    = "output"
-Templates_Folder_Name = "templates"
-Themes_Folder_Name    = "themes"
-HTML_Suffix           = ".html"
-TOML_Suffix           = ".toml"
-MD_Suffix             = ".md"
-RSS_Atom_XML          = "atom.xml"
-Theme_CSS_Name        = "theme.css"
-Default_Theme_Name    = "simple"
-Temp_HTML             = "temp.html"
-
-CWD = Path.cwd().resolve()
-Drafts_Folder_Path    = CWD.joinpath(Drafts_Folder_Name)
-Articles_Folder_Path  = CWD.joinpath(Articles_Folder_Name)
-Metadata_Folder_Path  = Articles_Folder_Path.joinpath(Metadata_Folder_Name)
-Output_Folder_Path    = CWD.joinpath(Output_Folder_Name)
-Pics_Folder_Path      = Output_Folder_Path.joinpath(Pics_Folder_Name)
-RSS_Path              = Output_Folder_Path.joinpath(RSS_Atom_XML)
-Theme_CSS_Path        = Output_Folder_Path.joinpath(Theme_CSS_Name)
-Temp_HTML_Path        = Output_Folder_Path.joinpath(Temp_HTML)
-Templates_Folder_Path = CWD.joinpath(Templates_Folder_Name)
-Themes_Folder_Path    = Templates_Folder_Path.joinpath(Themes_Folder_Name)
-Draft_TMPL_Path       = Templates_Folder_Path.joinpath(Draft_TMPL_Name)
-Blog_Config_Path      = CWD.joinpath(Blog_Config_Filename)
-
-Filename_Forbid_Pattern = re.compile(r"[^._0-9a-zA-Z\-]")
-"""文件名只能使用 0-9, a-z, A-Z, _(下划线), -(短横线)。"""
-
-Markdown_Title_Pattern = re.compile(r"^(#{1,6}|>|1.|-|\*) (.+)")
-
-Title_Index_Length = 1
-"""标题索引字数（以后有可能改成允许用户自定义）"""
-
-RSS_Entries_Max = 10
-"""RSS 里最多可包含多少篇文章"""
-
-RSS_Content_Size = 256
-"""RSS 里每篇文章的摘要长度上限，单位: UTF8字符"""
-
-
-def now():
-    return arrow.now().format(RFC3339)
-
-
-@dataclass
-class BlogConfig:
-    name             : str   # 博客名称
-    author           : str   # 默认作者（每篇文章也可独立设定作者）
-    uuid             : str   # 用于 RSS feed 的 uuid
-    website          : str   # 博客网址，用于 RSS feed
-    rss_link         : str   # RSS feed 的网址，根据 website 生成
-    home_recent_max  : int   # 首页 "最近更新" 列表中的项目上限
-    title_length_max : int   # 文章标题长度上限，单位: byte
-    rss_updated      : str   # 上次生成 RSS feed 的时间
-    blog_updated     : str   # 博客更新日期，如果大于 rss_updated 就要重新生成 RSS
-    auto_replace     : bool  # 是否执行自动替换
-    img_max_width    : str   # HTML中的图片的最大宽度
-    current_theme    : str   # 当前主题 (CSS)
-
-    @classmethod
-    def default(cls):
-        return BlogConfig(
-            name             = "在此填写博客名称",
-            author           = "在此填写作者名称",
-            uuid             = "",  # 在第一次填写博客名称时生成
-            website          = "在此填写博客网址",
-            rss_link         = "",  # 在博客名称变更时生成
-            home_recent_max  = 10,
-            title_length_max = 192,
-            rss_updated      = "",
-            blog_updated     = now(),
-            auto_replace     = True,
-            img_max_width    = "100%",
-            current_theme    = "simple",
-        )
-
-    @classmethod
-    def loads(cls):
-        """Loads BlogConfig from Blog_Config_Path"""
-        data = tomli_loads(Blog_Config_Path)
-        return BlogConfig(**data)
-
-
-@dataclass
-class ArticleConfig:
-    title     : str   # 文章标题 [不需要手动填写，会自动获取]
-    author    : str   # 文章作者 [通常留空，自动等同于博客作者]
-    ctime     : str   # 文章创建时间
-    mtime     : str   # 文章修改时间
-    checksum  : str   # sha1, 用来判断文章内容有无变更
-    ignored   : bool  # 忽略文章 (不出现在索引列表里，但仍会出现在 RSS 里)
-    img_width : str   # HTML中的图片的最大宽度 (留空表示跟随总设定)
-    replace   : int   # 是否执行自动替换 (0:跟随总设定, -1:不执行, 1:执行)
-    pairs     : list  # 自动替换（主要用于替换图片地址）
-
-    """其中, pairs 用 TOML 描述如下：
-    pairs =  [
-        [ '''../output/pics/abc.jpg''', '''https://example.com/abc.jpg''' ],
-        [ '''../output/pics/def.jpg''', '''https://example.com/def.jpg''' ],
-    ]
-    
-    意思是，渲染时用每一对的第二个字符串来代替第一个字符串。
-    （只是渲染后的 HTML 的内容被替换, markdown 文件的内容保持不变）
-    """
-
-    @classmethod
-    def from_md_file(cls, file_path: Path, file_data: bytes, title_length: int):
-        md_str      = file_data.decode()
-        first_line  = get_first_line(md_str)
-        checksum    = hashlib.sha1(file_data).hexdigest()
-        ctime       = now()
-
-        title = get_md_title(first_line, title_length)
-        if not title:
-            return None, f"无法获取文章标题，请修改文章的标题(文件的第一行内容): {file_path}"
-
-        art_cfg = ArticleConfig(
-            title     = title,
-            author    = "",
-            ctime     = ctime,
-            mtime     = ctime,
-            checksum  = checksum,
-            ignored   = False,
-            img_width = "",
-            replace   = 0,
-            pairs     = [],
-        )
-        return art_cfg, None
-
-    @classmethod
-    def loads(cls, file):
-        """Loads ArticleConfig from an article.toml file."""
-        data = tomli_loads(file)
-        return ArticleConfig(**data)
-
-    def copy(self):
-        """Make a copy."""
-        return ArticleConfig(**asdict(self))
-
-
-@dataclass
-class TitleIndex:
-    name: str
-    id: str
-    articles: []  # List[ArticleConfig]
-
-
-def tomli_loads(file) -> dict:
-    """正确处理 utf-16"""
-    with open(file, "rb") as f:
-        text = f.read()
-        try:
-            text = text.decode()  # Default encoding is 'utf-8'.
-        except UnicodeDecodeError:
-            text = text.decode("utf-16").encode().decode()
-        return tomli.loads(text)
-
-
-def get_first_line(file):
-    """
-    :param file: str
-    :return: str, 注意有可能返回空字符串。
-    """
-    for line in file.splitlines():
-        line = line.strip()
-        if line:
-            return line
-    return ""
-
-
-def byte_len(s: str) -> int:
-    return len(s.encode("utf8"))
-
-
-def utf8_lead_byte(b):
-    """A UTF-8 intermediate byte starts with the bits 10xxxxxx."""
-    return (b & 0xC0) != 0x80
-
-
-# https://stackoverflow.com/questions/13727977/truncating-string-to-byte-length-in-python
-def utf8_byte_truncate(text: str, max_bytes: int) -> str:
-    """If text[max_bytes] is not a lead byte, back up until a lead byte is
-    found and truncate before that character."""
-    utf8 = text.encode("utf8")
-    if len(utf8) <= max_bytes:
-        return text
-    i = max_bytes
-    while i > 0 and not utf8_lead_byte(utf8[i]):
-        i -= 1
-    return utf8[:i].decode("utf8")
-
-
-def check_filename(name: str):
-    """
-    :return: 发生错误时返回 err_msg: str, 没有错误则返回 False 或空字符串。
-    """
-    if Filename_Forbid_Pattern.search(name) is None:
-        return False
-    else:
-        return "文件名只能使用 0-9, a-z, A-Z, _(下划线), -(短横线), .(点)" \
-               "\n注意：不能使用空格，请用下划线或短横线代替空格。"
-
-
-def get_md_title(md_first_line: str, max_bytes: int) -> str:
-    """
-    :param md_first_line: 应已去除首尾空白字符。
-    :param max_bytes: 标题长度上限，单位: bytes
-    :return: 注意有可能返回空字符串。
-    """
-    md_title = Markdown_Title_Pattern.findall(md_first_line)
-    if not md_title:
-        title = md_first_line
-    else:
-        # 此时 md_title 大概像这样: [('#', ' abcd')]
-        title = md_title[0][1].strip()
-
-    return utf8_byte_truncate(title, max_bytes).strip()
+import hashlib
+import re
+from dataclasses import dataclass, asdict
+from pathlib import Path
+
+import arrow
+import tomli
+
+# 注意: model.py 在最底层，不能 import util.py, tmpl_render.py, 更不能 import main.py
+
+RFC3339               = "YYYY-MM-DD HH:mm:ssZZ"
+Blog_Config_Filename  = "blog.toml"
+Drafts_Folder_Name    = "drafts"
+Draft_TMPL_Name       = "draft.md"
+Articles_Folder_Name  = "articles"
+Pics_Folder_Name      = "pics"
+Metadata_Folder_Name  = "metadata"
+Output_Folder_Name    = "output"
+Templates_Folder_Name = "templates"
+Themes_Folder_Name    = "themes"
+HTML_Suffix           = ".html"
+TOML_Suffix           = ".toml"
+MD_Suffix             = ".md"
+RSS_Atom_XML          = "atom.xml"
+Theme_CSS_Name        = "theme.css"
+Default_Theme_Name    = "simple"
+Temp_HTML             = "temp.html"
+
+CWD = Path.cwd().resolve()
+Drafts_Folder_Path    = CWD.joinpath(Drafts_Folder_Name)
+Articles_Folder_Path  = CWD.joinpath(Articles_Folder_Name)
+Metadata_Folder_Path  = Articles_Folder_Path.joinpath(Metadata_Folder_Name)
+Output_Folder_Path    = CWD.joinpath(Output_Folder_Name)
+Pics_Folder_Path      = Output_Folder_Path.joinpath(Pics_Folder_Name)
+RSS_Path              = Output_Folder_Path.joinpath(RSS_Atom_XML)
+Theme_CSS_Path        = Output_Folder_Path.joinpath(Theme_CSS_Name)
+Temp_HTML_Path        = Output_Folder_Path.joinpath(Temp_HTML)
+Templates_Folder_Path = CWD.joinpath(Templates_Folder_Name)
+Themes_Folder_Path    = Templates_Folder_Path.joinpath(Themes_Folder_Name)
+Draft_TMPL_Path       = Templates_Folder_Path.joinpath(Draft_TMPL_Name)
+Blog_Config_Path      = CWD.joinpath(Blog_Config_Filename)
+
+Filename_Forbid_Pattern = re.compile(r"[^._0-9a-zA-Z\-]")
+"""文件名只能使用 0-9, a-z, A-Z, _(下划线), -(短横线), .(点)。"""
+
+Markdown_Title_Pattern = re.compile(r"^(#{1,6}|>|1.|-|\*) (.+)")
+
+Title_Index_Length = 1
+"""标题索引字数（以后有可能改成允许用户自定义）"""
+
+RSS_Entries_Max = 10
+"""RSS 里最多可包含多少篇文章"""
+
+RSS_Content_Size = 256
+"""RSS 里每篇文章的摘要长度上限，单位: UTF8字符"""
+
+
+def now():
+    return arrow.now().format(RFC3339)
+
+
+@dataclass
+class BlogConfig:
+    name             : str   # 博客名称
+    author           : str   # 默认作者（每篇文章也可独立设定作者）
+    uuid             : str   # 用于 RSS feed 的 uuid
+    website          : str   # 博客网址，用于 RSS feed
+    rss_link         : str   # RSS feed 的网址，根据 website 生成
+    home_recent_max  : int   # 首页 "最近更新" 列表中的项目上限
+    title_length_max : int   # 文章标题长度上限，单位: byte
+    rss_updated      : str   # 上次生成 RSS feed 的时间
+    blog_updated     : str   # 博客更新日期，如果大于 rss_updated 就要重新生成 RSS
+    auto_replace     : bool  # 是否执行自动替换
+    img_max_width    : str   # HTML中的图片的最大宽度
+    current_theme    : str   # 当前主题 (CSS)
+
+    @classmethod
+    def default(cls):
+        return BlogConfig(
+            name             = "在此填写博客名称",
+            author           = "在此填写作者名称",
+            uuid             = "",  # 在第一次填写博客名称时生成
+            website          = "在此填写博客网址",
+            rss_link         = "",  # 在博客名称变更时生成
+            home_recent_max  = 10,
+            title_length_max = 192,
+            rss_updated      = "",
+            blog_updated     = now(),
+            auto_replace     = True,
+            img_max_width    = "100%",
+            current_theme    = "simple",
+        )
+
+    @classmethod
+    def loads(cls):
+        """Loads BlogConfig from Blog_Config_Path"""
+        data = tomli_loads(Blog_Config_Path)
+        return BlogConfig(**data)
+
+
+@dataclass
+class ArticleConfig:
+    title     : str   # 文章标题 [不需要手动填写，会自动获取]
+    author    : str   # 文章作者 [通常留空，自动等同于博客作者]
+    ctime     : str   # 文章创建时间
+    mtime     : str   # 文章修改时间
+    checksum  : str   # sha1, 用来判断文章内容有无变更
+    ignored   : bool  # 忽略文章 (不出现在索引列表里，但仍会出现在 RSS 里)
+    img_width : str   # HTML中的图片的最大宽度 (留空表示跟随总设定)
+    replace   : int   # 是否执行自动替换 (0:跟随总设定, -1:不执行, 1:执行)
+    pairs     : list  # 自动替换（主要用于替换图片地址）
+
+    """其中, pairs 用 TOML 描述如下：
+    pairs =  [
+        [ '''../output/pics/abc.jpg''', '''https://example.com/abc.jpg''' ],
+        [ '''../output/pics/def.jpg''', '''https://example.com/def.jpg''' ],
+    ]
+    
+    意思是，渲染时用每一对的第二个字符串来代替第一个字符串。
+    （只是渲染后的 HTML 的内容被替换, markdown 文件的内容保持不变）
+    """
+
+    @classmethod
+    def from_md_file(cls, file_path: Path, file_data: bytes, title_length: int):
+        md_str      = file_data.decode()
+        first_line  = get_first_line(md_str)
+        checksum    = hashlib.sha1(file_data).hexdigest()
+        ctime       = now()
+
+        title = get_md_title(first_line, title_length)
+        if not title:
+            return None, f"无法获取文章标题，请修改文章的标题(文件的第一行内容): {file_path}"
+
+        art_cfg = ArticleConfig(
+            title     = title,
+            author    = "",
+            ctime     = ctime,
+            mtime     = ctime,
+            checksum  = checksum,
+            ignored   = False,
+            img_width = "",
+            replace   = 0,
+            pairs     = [],
+        )
+        return art_cfg, None
+
+    @classmethod
+    def loads(cls, file):
+        """Loads ArticleConfig from an article.toml file."""
+        data = tomli_loads(file)
+        return ArticleConfig(**data)
+
+    def copy(self):
+        """Make a copy."""
+        return ArticleConfig(**asdict(self))
+
+
+@dataclass
+class TitleIndex:
+    name: str
+    id: str
+    articles: list  # List[ArticleConfig]
+
+
+def tomli_loads(file) -> dict:
+    """正确处理 utf-16"""
+    with open(file, "rb") as f:
+        text = f.read()
+        try:
+            text = text.decode()  # Default encoding is 'utf-8'.
+        except UnicodeDecodeError:
+            text = text.decode("utf-16").encode("utf-8").decode("utf-8")
+        return tomli.loads(text)
+
+
+def get_first_line(file):
+    """
+    :param file: str
+    :return: str, 注意有可能返回空字符串。
+    """
+    for line in file.splitlines():
+        line = line.strip()
+        if line:
+            return line
+    return ""
+
+
+def byte_len(s: str) -> int:
+    return len(s.encode("utf8"))
+
+
+def utf8_lead_byte(b):
+    """A UTF-8 intermediate byte starts with the bits 10xxxxxx."""
+    return (b & 0xC0) != 0x80
+
+
+# https://stackoverflow.com/questions/13727977/truncating-string-to-byte-length-in-python
+def utf8_byte_truncate(text: str, max_bytes: int) -> str:
+    """If text[max_bytes] is not a lead byte, back up until a lead byte is
+    found and truncate before that character."""
+    utf8 = text.encode("utf8")
+    if len(utf8) <= max_bytes:
+        return text
+    i = max_bytes
+    while i > 0 and not utf8_lead_byte(utf8[i]):
+        i -= 1
+    return utf8[:i].decode("utf8")
+
+
+def check_filename(name: str):
+    """
+    :return: 发生错误时返回 err_msg: str, 没有错误则返回 False 或空字符串。
+    """
+    if Filename_Forbid_Pattern.search(name) is None:
+        return False
+    else:
+        return "文件名只能使用 0-9, a-z, A-Z, _(下划线), -(短横线), .(点)" \
+               "\n注意：不能使用空格，请用下划线或短横线代替空格。"
+
+
+def get_md_title(md_first_line: str, max_bytes: int) -> str:
+    """
+    :param md_first_line: 应已去除首尾空白字符。
+    :param max_bytes: 标题长度上限，单位: bytes
+    :return: 注意有可能返回空字符串。
+    """
+    md_title = Markdown_Title_Pattern.findall(md_first_line)
+    if not md_title:
+        title = md_first_line
+    else:
+        # 此时 md_title 大概像这样: [('#', ' abcd')]
+        title = md_title[0][1].strip()
+
+    return utf8_byte_truncate(title, max_bytes).strip()
```

### Comparing `pyboke-0.0.4/src/pyboke/templates/LICENSE.txt` & `pyboke-0.0.5/src/pyboke/templates/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyboke-0.0.4/src/pyboke/templates/article.html` & `pyboke-0.0.5/src/pyboke/templates/article.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,53 @@
-{% extends "base.html" %}
-
-{% block title%}
-  <title>{{ art.title }} - {{ blog.name }}</title>
-{% endblock %}
-
-{% block style %}
-  <style>
-  img {
-    {% if art.img_width|length %}
-    max-width: {{ art.img_width }} !important;
-    {% else %}
-    max-width: {{ blog.img_max_width }} !important;
-    {% endif %}
-    height: auto !important;
-  }
-  </style>
-{% endblock %}
-
-{% block header %}
-{% endblock %}
-
-{% block main %}
-
-{{ art.content|safe }}
-
-<div id="updated-at">
-  <span>Updated at {{ art.mtime[0:19] }}</span>
-</div>
-{% endblock %}
-
-{% block footer %}
-<div id="footer">
-  <div id="footer-home-link">
-    <a href="index.html">&lt;&lt; Home</a>
-    {% if not art.ignored %}
-    <a href="title-index.html#{{art.index_id}}">&lt;&lt; Index</a>
-    |
-    <a href="random.html">Random &gt;&gt;</a>
-    {% endif %}
-  </div>
-  <p id="footer-body">
-    {% if art.author|length %}
-    Author: {{ art.author }}
-    {% else %}
-    Author: {{ blog.author }}
-    {% endif %}
-    | LICENSE <a href="LICENSE.txt">CC0-1.0</a>
-    | RSS <a href="atom.xml">atom.xml</a>
-  </p>
-</div>
-{% endblock %}
+{% extends "base.html" %}
+
+{% block title%}
+  <title>{{ art.title }} - {{ blog.name }}</title>
+{% endblock %}
+
+{% block style %}
+  <style>
+  img {
+    {% if art.img_width|length %}
+    max-width: {{ art.img_width }} !important;
+    {% else %}
+    max-width: {{ blog.img_max_width }} !important;
+    {% endif %}
+    height: auto !important;
+  }
+  </style>
+{% endblock %}
+
+{% block header %}
+{% endblock %}
+
+{% block main %}
+
+{{ art.content|safe }}
+
+<div id="updated-at">
+  <span>Updated at {{ art.mtime[0:19] }}</span><br>
+  <span>Created at {{ art.ctime[0:19] }}</span>
+</div>
+{% endblock %}
+
+{% block footer %}
+<div id="footer">
+  <div id="footer-home-link">
+    <a href="index.html">&lt;&lt; Home</a>
+    {% if not art.ignored %}
+    <a href="title-index.html#{{art.index_id}}">&lt;&lt; Index</a>
+    |
+    <a href="random.html">Random &gt;&gt;</a>
+    {% endif %}
+  </div>
+  <p id="footer-body">
+    {% if art.author|length %}
+    Author: {{ art.author }}
+    {% else %}
+    Author: {{ blog.author }}
+    {% endif %}
+    | LICENSE <a href="LICENSE.txt">CC0-1.0</a>
+    | RSS <a href="atom.xml">atom.xml</a>
+  </p>
+</div>
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 {% extends "base.html" %} {% block title%}
 {% endblock %} {% block style %}
  {% endblock %} {% block header %} {% endblock %} {% block main %} {
 { art.content|safe }}
 Updated at {{ art.mtime[0:19] }}
+Created at {{ art.ctime[0:19] }}
 {% endblock %} {% block footer %}
 <<_Home {% if not art.ignored %} <<_Index | Random_>> {% endif %}
 {% if art.author|length %} Author: {{ art.author }} {% else %} Author: {
 { blog.author }} {% endif %} | LICENSE CC0-1.0 | RSS atom.xml
 {% endblock %}
```

### Comparing `pyboke-0.0.4/src/pyboke/templates/article.toml` & `pyboke-0.0.5/src/pyboke/templates/article.toml`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# 本文件采用 TOML 格式 https://toml.io/
-
-# 文章标题 [请勿手动修改，会自动获取]
-title = '''{{art.title}}'''
-
-# 文章作者 [通常留空，自动等同于博客作者]
-author = '''{{art.author}}'''
-
-# 文章创建时间
-ctime = '{{art.ctime}}'
-
-# 文章修改时间
-mtime = '{{art.mtime}}'
-
-# sha1, 用来判断文章内容有无变更 [请勿手动修改]
-checksum = '{{art.checksum}}'
-
-# 是否忽略文章 (true/false)
-# 被忽略的文章不会出现在最近列表、索引列表里，但仍会出现在 RSS 里
-ignored = {{art.ignored|string|lower}}
-
-# HTML中的图片的最大宽度 (留空表示跟随总设定)
-img_width = '{{art.img_width}}'
-
-# 是否执行自动替换 (0:跟随总设定, -1:不执行, 1:执行)
-replace = {{art.replace}}
-
-# 自动替换。例:
-# pairs =  [
-#   [ '''../output/pics/abc.jpg''', '''https://example.com/abc.jpg''' ],
-#   [ '''../output/pics/def.jpg''', '''https://example.com/def.jpg''' ],
-# ]
-pairs = [
-{% for pair in art.pairs %}
-  [
-    {%- for item in pair -%}
-    '''{{item}}''',
-    {%- endfor -%}
-  ],
-{% endfor %}
-]
-
+# 本文件采用 TOML 格式 https://toml.io/
+
+# 文章标题 [请勿手动修改，会自动获取]
+title = '''{{art.title}}'''
+
+# 文章作者 [通常留空，自动等同于博客作者]
+author = '''{{art.author}}'''
+
+# 文章创建时间
+ctime = '{{art.ctime}}'
+
+# 文章修改时间
+mtime = '{{art.mtime}}'
+
+# sha1, 用来判断文章内容有无变更 [请勿手动修改]
+checksum = '{{art.checksum}}'
+
+# 是否忽略文章 (true/false)
+# 被忽略的文章不会出现在最近列表、索引列表里，但仍会出现在 RSS 里
+ignored = {{art.ignored|string|lower}}
+
+# HTML中的图片的最大宽度 (留空表示跟随总设定)
+img_width = '{{art.img_width}}'
+
+# 是否执行自动替换 (0:跟随总设定, -1:不执行, 1:执行)
+replace = {{art.replace}}
+
+# 自动替换。例:
+# pairs =  [
+#   [ '''../output/pics/abc.jpg''', '''https://example.com/abc.jpg''' ],
+#   [ '''../output/pics/def.jpg''', '''https://example.com/def.jpg''' ],
+# ]
+pairs = [
+{% for pair in art.pairs %}
+  [
+    {%- for item in pair -%}
+    '''{{item}}''',
+    {%- endfor -%}
+  ],
+{% endfor %}
+]
+
```

### Comparing `pyboke-0.0.4/src/pyboke/templates/atom.xml` & `pyboke-0.0.5/src/pyboke/templates/atom.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text*

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 7574  .0" encoding="ut
-00000020: 662d 3822 3f3e 0a3c 6665 6564 2078 6d6c  f-8"?>.<feed xml
-00000030: 6e73 3d22 6874 7470 3a2f 2f77 7777 2e77  ns="http://www.w
-00000040: 332e 6f72 672f 3230 3035 2f41 746f 6d22  3.org/2005/Atom"
-00000050: 3e0a 0a20 203c 7469 746c 653e 7b7b 2062  >..  <title>{{ b
-00000060: 6c6f 672e 6e61 6d65 207d 7d3c 2f74 6974  log.name }}</tit
-00000070: 6c65 3e0a 2020 3c6c 696e 6b20 7265 663d  le>.  <link ref=
-00000080: 2273 656c 6622 2068 7265 663d 227b 7b20  "self" href="{{ 
-00000090: 626c 6f67 2e66 6565 645f 6c69 6e6b 207d  blog.feed_link }
-000000a0: 7d22 2f3e 0a20 203c 6c69 6e6b 2072 6566  }"/>.  <link ref
-000000b0: 3d22 616c 7465 726e 6174 6522 2068 7265  ="alternate" hre
-000000c0: 663d 227b 7b20 626c 6f67 2e77 6562 7369  f="{{ blog.websi
-000000d0: 7465 207d 7d22 2f3e 0a20 203c 7570 6461  te }}"/>.  <upda
-000000e0: 7465 643e 7b7b 2062 6c6f 672e 7570 6461  ted>{{ blog.upda
-000000f0: 7465 6420 7d7d 3c2f 7570 6461 7465 643e  ted }}</updated>
-00000100: 0a20 203c 6175 7468 6f72 3e0a 2020 2020  .  <author>.    
-00000110: 3c6e 616d 653e 7b7b 2062 6c6f 672e 6175  <name>{{ blog.au
-00000120: 7468 6f72 207d 7d3c 2f6e 616d 653e 0a20  thor }}</name>. 
-00000130: 203c 2f61 7574 686f 723e 0a20 203c 6964   </author>.  <id
-00000140: 3e7b 7b20 626c 6f67 2e75 7569 6420 7d7d  >{{ blog.uuid }}
-00000150: 3c2f 6964 3e0a 0a20 207b 2520 666f 7220  </id>..  {% for 
-00000160: 6974 656d 2069 6e20 656e 7472 6965 7320  item in entries 
-00000170: 257d 0a20 203c 656e 7472 793e 0a20 2020  %}.  <entry>.   
-00000180: 203c 7469 746c 653e 7b7b 2069 7465 6d2e   <title>{{ item.
-00000190: 7469 746c 6520 7d7d 3c2f 7469 746c 653e  title }}</title>
-000001a0: 0a20 2020 203c 6c69 6e6b 2072 6566 3d22  .    <link ref="
-000001b0: 616c 7465 726e 6174 6522 2068 7265 663d  alternate" href=
-000001c0: 227b 7b20 626c 6f67 2e77 6562 7369 7465  "{{ blog.website
-000001d0: 202b 2069 7465 6d2e 6964 202b 2027 2e68   + item.id + '.h
-000001e0: 746d 6c27 7d7d 2220 2f3e 0a20 2020 203c  tml'}}" />.    <
-000001f0: 6964 3e7b 7b20 6974 656d 2e69 6420 7d7d  id>{{ item.id }}
-00000200: 3c2f 6964 3e0a 2020 2020 3c70 7562 6c69  </id>.    <publi
-00000210: 7368 6564 3e7b 7b20 6974 656d 2e63 7469  shed>{{ item.cti
-00000220: 6d65 207d 7d3c 2f70 7562 6c69 7368 6564  me }}</published
-00000230: 3e0a 2020 2020 3c75 7064 6174 6564 3e7b  >.    <updated>{
-00000240: 7b20 6974 656d 2e6d 7469 6d65 207d 7d3c  { item.mtime }}<
-00000250: 2f75 7064 6174 6564 3e0a 2020 2020 3c61  /updated>.    <a
-00000260: 7574 686f 723e 3c6e 616d 653e 0a20 2020  uthor><name>.   
-00000270: 2020 207b 252d 2069 6620 6974 656d 2e61     {%- if item.a
-00000280: 7574 686f 727c 6c65 6e67 7468 202d 257d  uthor|length -%}
-00000290: 0a20 2020 2020 2020 207b 7b20 6974 656d  .        {{ item
-000002a0: 2e61 7574 686f 7220 7d7d 0a20 2020 2020  .author }}.     
-000002b0: 207b 252d 2065 6c73 6520 2d25 7d0a 2020   {%- else -%}.  
-000002c0: 2020 2020 2020 7b7b 2062 6c6f 672e 6175        {{ blog.au
-000002d0: 7468 6f72 207d 7d0a 2020 2020 2020 7b25  thor }}.      {%
-000002e0: 2d20 656e 6469 6620 2d25 7d0a 2020 2020  - endif -%}.    
-000002f0: 3c2f 6e61 6d65 3e3c 2f61 7574 686f 723e  </name></author>
-00000300: 0a20 2020 203c 636f 6e74 656e 7420 7479  .    <content ty
-00000310: 7065 3d22 7465 7874 223e 7b7b 2069 7465  pe="text">{{ ite
-00000320: 6d2e 636f 6e74 656e 7420 7d7d 3c2f 636f  m.content }}</co
-00000330: 6e74 656e 743e 0a20 203c 2f65 6e74 7279  ntent>.  </entry
-00000340: 3e0a 2020 7b25 2065 6e64 666f 7220 257d  >.  {% endfor %}
-00000350: 0a0a 3c2f 6665 6564 3e0a                 ..</feed>.
+00000020: 662d 3822 3f3e 0d0a 3c66 6565 6420 786d  f-8"?>..<feed xm
+00000030: 6c6e 733d 2268 7474 703a 2f2f 7777 772e  lns="http://www.
+00000040: 7733 2e6f 7267 2f32 3030 352f 4174 6f6d  w3.org/2005/Atom
+00000050: 223e 0d0a 0d0a 2020 3c74 6974 6c65 3e7b  ">....  <title>{
+00000060: 7b20 626c 6f67 2e6e 616d 6520 7d7d 3c2f  { blog.name }}</
+00000070: 7469 746c 653e 0d0a 2020 3c6c 696e 6b20  title>..  <link 
+00000080: 7265 663d 2273 656c 6622 2068 7265 663d  ref="self" href=
+00000090: 227b 7b20 626c 6f67 2e66 6565 645f 6c69  "{{ blog.feed_li
+000000a0: 6e6b 207d 7d22 2f3e 0d0a 2020 3c6c 696e  nk }}"/>..  <lin
+000000b0: 6b20 7265 663d 2261 6c74 6572 6e61 7465  k ref="alternate
+000000c0: 2220 6872 6566 3d22 7b7b 2062 6c6f 672e  " href="{{ blog.
+000000d0: 7765 6273 6974 6520 7d7d 222f 3e0d 0a20  website }}"/>.. 
+000000e0: 203c 7570 6461 7465 643e 7b7b 2062 6c6f   <updated>{{ blo
+000000f0: 672e 7570 6461 7465 6420 7d7d 3c2f 7570  g.updated }}</up
+00000100: 6461 7465 643e 0d0a 2020 3c61 7574 686f  dated>..  <autho
+00000110: 723e 0d0a 2020 2020 3c6e 616d 653e 7b7b  r>..    <name>{{
+00000120: 2062 6c6f 672e 6175 7468 6f72 207d 7d3c   blog.author }}<
+00000130: 2f6e 616d 653e 0d0a 2020 3c2f 6175 7468  /name>..  </auth
+00000140: 6f72 3e0d 0a20 203c 6964 3e7b 7b20 626c  or>..  <id>{{ bl
+00000150: 6f67 2e75 7569 6420 7d7d 3c2f 6964 3e0d  og.uuid }}</id>.
+00000160: 0a0d 0a20 207b 2520 666f 7220 6974 656d  ...  {% for item
+00000170: 2069 6e20 656e 7472 6965 7320 257d 0d0a   in entries %}..
+00000180: 2020 3c65 6e74 7279 3e0d 0a20 2020 203c    <entry>..    <
+00000190: 7469 746c 653e 7b7b 2069 7465 6d2e 7469  title>{{ item.ti
+000001a0: 746c 6520 7d7d 3c2f 7469 746c 653e 0d0a  tle }}</title>..
+000001b0: 2020 2020 3c6c 696e 6b20 7265 663d 2261      <link ref="a
+000001c0: 6c74 6572 6e61 7465 2220 6872 6566 3d22  lternate" href="
+000001d0: 7b7b 2062 6c6f 672e 7765 6273 6974 6520  {{ blog.website 
+000001e0: 2b20 6974 656d 2e69 6420 2b20 272e 6874  + item.id + '.ht
+000001f0: 6d6c 277d 7d22 202f 3e0d 0a20 2020 203c  ml'}}" />..    <
+00000200: 6964 3e7b 7b20 6974 656d 2e69 6420 7d7d  id>{{ item.id }}
+00000210: 3c2f 6964 3e0d 0a20 2020 203c 7075 626c  </id>..    <publ
+00000220: 6973 6865 643e 7b7b 2069 7465 6d2e 6374  ished>{{ item.ct
+00000230: 696d 6520 7d7d 3c2f 7075 626c 6973 6865  ime }}</publishe
+00000240: 643e 0d0a 2020 2020 3c75 7064 6174 6564  d>..    <updated
+00000250: 3e7b 7b20 6974 656d 2e6d 7469 6d65 207d  >{{ item.mtime }
+00000260: 7d3c 2f75 7064 6174 6564 3e0d 0a20 2020  }</updated>..   
+00000270: 203c 6175 7468 6f72 3e3c 6e61 6d65 3e0d   <author><name>.
+00000280: 0a20 2020 2020 207b 252d 2069 6620 6974  .      {%- if it
+00000290: 656d 2e61 7574 686f 727c 6c65 6e67 7468  em.author|length
+000002a0: 202d 257d 0d0a 2020 2020 2020 2020 7b7b   -%}..        {{
+000002b0: 2069 7465 6d2e 6175 7468 6f72 207d 7d0d   item.author }}.
+000002c0: 0a20 2020 2020 207b 252d 2065 6c73 6520  .      {%- else 
+000002d0: 2d25 7d0d 0a20 2020 2020 2020 207b 7b20  -%}..        {{ 
+000002e0: 626c 6f67 2e61 7574 686f 7220 7d7d 0d0a  blog.author }}..
+000002f0: 2020 2020 2020 7b25 2d20 656e 6469 6620        {%- endif 
+00000300: 2d25 7d0d 0a20 2020 203c 2f6e 616d 653e  -%}..    </name>
+00000310: 3c2f 6175 7468 6f72 3e0d 0a20 2020 203c  </author>..    <
+00000320: 636f 6e74 656e 7420 7479 7065 3d22 7465  content type="te
+00000330: 7874 223e 7b7b 2069 7465 6d2e 636f 6e74  xt">{{ item.cont
+00000340: 656e 7420 7d7d 3c2f 636f 6e74 656e 743e  ent }}</content>
+00000350: 0d0a 2020 3c2f 656e 7472 793e 0d0a 2020  ..  </entry>..  
+00000360: 7b25 2065 6e64 666f 7220 257d 0d0a 0d0a  {% endfor %}....
+00000370: 3c2f 6665 6564 3e0d 0a                   </feed>..
```

### Comparing `pyboke-0.0.4/src/pyboke/templates/blog.toml` & `pyboke-0.0.5/src/pyboke/templates/blog.toml`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-# 本文件采用 TOML 格式 https://toml.io/
-
-# [必填] 博客名称
-name = '''{{cfg.name}}'''
-
-# [必填] 博客作者
-author = '''{{cfg.author}}'''
-
-# 首页 "最近文章" 列表中的项目上限
-home_recent_max = {{cfg.home_recent_max}}
-
-# 文章标题长度上限，单位: byte
-title_length_max = {{cfg.title_length_max}}
-
-# 是否执行自动替换 (true/false)
-auto_replace = {{cfg.auto_replace|string|lower}}
-
-# HTML中的图片的最大宽度
-img_max_width = '{{cfg.img_max_width}}'
-
-# [可暂时不填，但正式发布博客到网上时必填] 博客网址，用于 RSS feed
-website = '''{{cfg.website}}'''
-
-# 请填写以上项目
-# 以下项目一般由程序自动填写，不需要手动操作
-
-# RSS feed 的网址 [一般根据 website 自动生成]
-rss_link = '''{{cfg.rss_link}}'''
-
-# [手动修改无效] 当前主题 (CSS)
-current_theme = '{{cfg.current_theme}}'
-
-# [一般不手动修改] 用于 RSS feed 的 uuid
-uuid = '{{cfg.uuid}}'
-
-# [一般不手动修改] 上次生成 RSS feed 的时间
-rss_updated = '{{cfg.rss_updated}}'
-
-# [一般不手动修改] 博客更新日期，如果大于 rss_updated 就要重新生成 RSS
-blog_updated = '{{cfg.blog_updated}}'
-
+# 本文件采用 TOML 格式 https://toml.io/
+
+# [必填] 博客名称
+name = '''{{cfg.name}}'''
+
+# [必填] 博客作者
+author = '''{{cfg.author}}'''
+
+# 首页 "最近文章" 列表中的项目上限
+home_recent_max = {{cfg.home_recent_max}}
+
+# 文章标题长度上限，单位: byte
+title_length_max = {{cfg.title_length_max}}
+
+# 是否执行自动替换 (true/false)
+auto_replace = {{cfg.auto_replace|string|lower}}
+
+# HTML中的图片的最大宽度
+img_max_width = '{{cfg.img_max_width}}'
+
+# [可暂时不填，但正式发布博客到网上时必填] 博客网址，用于 RSS feed
+website = '''{{cfg.website}}'''
+
+# 请填写以上项目
+# 以下项目一般由程序自动填写，不需要手动操作
+
+# RSS feed 的网址 [一般根据 website 自动生成]
+rss_link = '''{{cfg.rss_link}}'''
+
+# [手动修改无效] 当前主题 (CSS)
+current_theme = '{{cfg.current_theme}}'
+
+# [一般不手动修改] 用于 RSS feed 的 uuid
+uuid = '{{cfg.uuid}}'
+
+# [一般不手动修改] 上次生成 RSS feed 的时间
+rss_updated = '{{cfg.rss_updated}}'
+
+# [一般不手动修改] 博客更新日期，如果大于 rss_updated 就要重新生成 RSS
+blog_updated = '{{cfg.blog_updated}}'
+
```

### Comparing `pyboke-0.0.4/src/pyboke/templates/style.css` & `pyboke-0.0.5/src/pyboke/templates/style.css`

 * *Files identical despite different names*

### Comparing `pyboke-0.0.4/src/pyboke/templates/themes/mvp.css` & `pyboke-0.0.5/src/pyboke/templates/themes/mvp.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-/* MVP.css v1.8 - https://github.com/andybrewer/mvp */
-:root{--active-brightness:0.85;--border-radius:5px;--box-shadow:2px 2px 10px;--color:#118bee;--color-accent:#118bee15;--color-bg:#fff;--color-bg-secondary:#e9e9e9;--color-link:#118bee;--color-secondary:#920de9;--color-secondary-accent:#920de90b;--color-shadow:#f4f4f4;--color-table:#118bee;--color-text:#000;--color-text-secondary:#999;--font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,Oxygen-Sans,Ubuntu,Cantarell,"Helvetica Neue",sans-serif;--hover-brightness:1.2;--justify-important:center;--justify-normal:left;--line-height:1.5;--width-card:285px;--width-card-medium:460px;--width-card-wide:800px;--width-content:1080px}@media (prefers-color-scheme:dark){:root{--color:#0097fc;--color-accent:#0097fc4f;--color-bg:#333;--color-bg-secondary:#555;--color-link:#0097fc;--color-secondary:#e20de9;--color-secondary-accent:#e20de94f;--color-shadow:#bbbbbb20;--color-table:#0097fc;--color-text:#f7f7f7;--color-text-secondary:#aaa}}article aside{background:var(--color-secondary-accent);border-left:4px solid var(--color-secondary);padding:.01rem .8rem}body{background:var(--color-bg);color:var(--color-text);font-family:var(--font-family);line-height:var(--line-height);margin:0;overflow-x:hidden;padding:0}footer,header,main{margin:0 auto;max-width:var(--width-content);padding:3rem 1rem}hr{background-color:var(--color-bg-secondary);border:none;height:1px;margin:4rem 0;width:100%}section{display:flex;flex-wrap:wrap;justify-content:var(--justify-important)}article img,section img{max-width:100%}section pre{overflow:auto}section aside{border:1px solid var(--color-bg-secondary);border-radius:var(--border-radius);box-shadow:var(--box-shadow) var(--color-shadow);margin:1rem;padding:1.25rem;width:var(--width-card)}section aside:hover{box-shadow:var(--box-shadow) var(--color-bg-secondary)}[hidden]{display:none}article header,div header,main header{padding-top:0}header{text-align:var(--justify-important)}header a b,header a em,header a i,header a strong{margin-left:.5rem;margin-right:.5rem}header nav img{margin:1rem 0}section header{padding-top:0;width:100%}nav{align-items:center;display:flex;font-weight:700;justify-content:space-between;margin-bottom:7rem}nav ul{list-style:none;padding:0}nav ul li{display:inline-block;margin:0 .5rem;position:relative;text-align:left}nav ul li:hover ul{display:block}nav ul li ul{background:var(--color-bg);border:1px solid var(--color-bg-secondary);border-radius:var(--border-radius);box-shadow:var(--box-shadow) var(--color-shadow);display:none;height:auto;left:-2px;padding:.5rem 1rem;position:absolute;top:1.7rem;white-space:nowrap;width:auto;z-index:1}nav ul li ul::before{content:"";position:absolute;left:0;right:0;top:-.5rem;height:.5rem}nav ul li ul li,nav ul li ul li a{display:block}code,samp{background-color:var(--color-accent);border-radius:var(--border-radius);color:var(--color-text);display:inline-block;margin:0 .1rem;padding:0 .5rem}details{margin:1.3rem 0}details summary{font-weight:700;cursor:pointer}h1,h2,h3,h4,h5,h6{line-height:var(--line-height)}mark{padding:.1rem}ol li,ul li{padding:.2rem 0}p{margin:.75rem 0;padding:0;width:100%}pre{margin:1rem 0;max-width:var(--width-card-wide);padding:1rem 0}pre code,pre samp{display:block;max-width:var(--width-card-wide);padding:.5rem 2rem;white-space:pre-wrap}small{color:var(--color-text-secondary)}sup{background-color:var(--color-secondary);border-radius:var(--border-radius);color:var(--color-bg);font-size:xx-small;font-weight:700;margin:.2rem;padding:.2rem .3rem;position:relative;top:-2px}a{color:var(--color-link);display:inline-block;font-weight:700;text-decoration:none}a:active{filter:brightness(var(--active-brightness));text-decoration:underline}a:hover{filter:brightness(var(--hover-brightness));text-decoration:underline}a b,a em,a i,a strong,button{border-radius:var(--border-radius);display:inline-block;font-size:medium;font-weight:700;line-height:var(--line-height);margin:.5rem 0;padding:1rem 2rem}button{font-family:var(--font-family)}button:active{filter:brightness(var(--active-brightness))}button:hover{cursor:pointer;filter:brightness(var(--hover-brightness))}a b,a strong,button{background-color:var(--color-link);border:2px solid var(--color-link);color:var(--color-bg)}a em,a i{border:2px solid var(--color-link);border-radius:var(--border-radius);color:var(--color-link);display:inline-block;padding:1rem 2rem}article aside a{color:var(--color-secondary)}figure{margin:0;padding:0}figure img{max-width:100%}figure figcaption{color:var(--color-text-secondary)}button:disabled,input:disabled{background:var(--color-bg-secondary);border-color:var(--color-bg-secondary);color:var(--color-text-secondary);cursor:not-allowed}button[disabled]:hover{filter:none}form{border:1px solid var(--color-bg-secondary);border-radius:var(--border-radius);box-shadow:var(--box-shadow) var(--color-shadow);display:block;max-width:var(--width-card-wide);min-width:var(--width-card);padding:1.5rem;text-align:var(--justify-normal)}form header{margin:1.5rem 0;padding:1.5rem 0}input,label,select,textarea{display:block;font-size:inherit;max-width:var(--width-card-wide)}input[type=checkbox],input[type=radio]{display:inline-block}input[type=checkbox]+label,input[type=radio]+label{display:inline-block;font-weight:400;position:relative;top:1px}input,select,textarea{border:1px solid var(--color-bg-secondary);border-radius:var(--border-radius);margin-bottom:1rem;padding:.4rem .8rem}input[readonly],textarea[readonly]{background-color:var(--color-bg-secondary)}label{font-weight:700;margin-bottom:.2rem}table{border:1px solid var(--color-bg-secondary);border-radius:var(--border-radius);border-spacing:0;display:inline-block;max-width:100%;overflow-x:auto;padding:0;white-space:nowrap}table td,table th,table tr{padding:.4rem .8rem;text-align:var(--justify-important)}table thead{background-color:var(--color-table);border-collapse:collapse;border-radius:var(--border-radius);color:var(--color-bg);margin:0;padding:0}table thead th:first-child{border-top-left-radius:var(--border-radius)}table thead th:last-child{border-top-right-radius:var(--border-radius)}table thead th:first-child,table tr td:first-child{text-align:var(--justify-normal)}table tr:nth-child(even){background-color:var(--color-accent)}blockquote{display:block;font-size:x-large;line-height:var(--line-height);margin:1rem auto;max-width:var(--width-card-medium);padding:1.5rem 1rem;text-align:var(--justify-important)}blockquote footer{color:var(--color-text-secondary);display:block;font-size:small;line-height:var(--line-height);padding:1.5rem 0}
-
-blockquote {
-  border: 5px solid #ccc;
-}
+/* MVP.css v1.8 - https://github.com/andybrewer/mvp */
+:root{--active-brightness:0.85;--border-radius:5px;--box-shadow:2px 2px 10px;--color:#118bee;--color-accent:#118bee15;--color-bg:#fff;--color-bg-secondary:#e9e9e9;--color-link:#118bee;--color-secondary:#920de9;--color-secondary-accent:#920de90b;--color-shadow:#f4f4f4;--color-table:#118bee;--color-text:#000;--color-text-secondary:#999;--font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,Oxygen-Sans,Ubuntu,Cantarell,"Helvetica Neue",sans-serif;--hover-brightness:1.2;--justify-important:center;--justify-normal:left;--line-height:1.5;--width-card:285px;--width-card-medium:460px;--width-card-wide:800px;--width-content:1080px}@media (prefers-color-scheme:dark){:root{--color:#0097fc;--color-accent:#0097fc4f;--color-bg:#333;--color-bg-secondary:#555;--color-link:#0097fc;--color-secondary:#e20de9;--color-secondary-accent:#e20de94f;--color-shadow:#bbbbbb20;--color-table:#0097fc;--color-text:#f7f7f7;--color-text-secondary:#aaa}}article aside{background:var(--color-secondary-accent);border-left:4px solid var(--color-secondary);padding:.01rem .8rem}body{background:var(--color-bg);color:var(--color-text);font-family:var(--font-family);line-height:var(--line-height);margin:0;overflow-x:hidden;padding:0}footer,header,main{margin:0 auto;max-width:var(--width-content);padding:3rem 1rem}hr{background-color:var(--color-bg-secondary);border:none;height:1px;margin:4rem 0;width:100%}section{display:flex;flex-wrap:wrap;justify-content:var(--justify-important)}article img,section img{max-width:100%}section pre{overflow:auto}section aside{border:1px solid var(--color-bg-secondary);border-radius:var(--border-radius);box-shadow:var(--box-shadow) var(--color-shadow);margin:1rem;padding:1.25rem;width:var(--width-card)}section aside:hover{box-shadow:var(--box-shadow) var(--color-bg-secondary)}[hidden]{display:none}article header,div header,main header{padding-top:0}header{text-align:var(--justify-important)}header a b,header a em,header a i,header a strong{margin-left:.5rem;margin-right:.5rem}header nav img{margin:1rem 0}section header{padding-top:0;width:100%}nav{align-items:center;display:flex;font-weight:700;justify-content:space-between;margin-bottom:7rem}nav ul{list-style:none;padding:0}nav ul li{display:inline-block;margin:0 .5rem;position:relative;text-align:left}nav ul li:hover ul{display:block}nav ul li ul{background:var(--color-bg);border:1px solid var(--color-bg-secondary);border-radius:var(--border-radius);box-shadow:var(--box-shadow) var(--color-shadow);display:none;height:auto;left:-2px;padding:.5rem 1rem;position:absolute;top:1.7rem;white-space:nowrap;width:auto;z-index:1}nav ul li ul::before{content:"";position:absolute;left:0;right:0;top:-.5rem;height:.5rem}nav ul li ul li,nav ul li ul li a{display:block}code,samp{background-color:var(--color-accent);border-radius:var(--border-radius);color:var(--color-text);display:inline-block;margin:0 .1rem;padding:0 .5rem}details{margin:1.3rem 0}details summary{font-weight:700;cursor:pointer}h1,h2,h3,h4,h5,h6{line-height:var(--line-height)}mark{padding:.1rem}ol li,ul li{padding:.2rem 0}p{margin:.75rem 0;padding:0;width:100%}pre{margin:1rem 0;max-width:var(--width-card-wide);padding:1rem 0}pre code,pre samp{display:block;max-width:var(--width-card-wide);padding:.5rem 2rem;white-space:pre-wrap}small{color:var(--color-text-secondary)}sup{background-color:var(--color-secondary);border-radius:var(--border-radius);color:var(--color-bg);font-size:xx-small;font-weight:700;margin:.2rem;padding:.2rem .3rem;position:relative;top:-2px}a{color:var(--color-link);display:inline-block;font-weight:700;text-decoration:none}a:active{filter:brightness(var(--active-brightness));text-decoration:underline}a:hover{filter:brightness(var(--hover-brightness));text-decoration:underline}a b,a em,a i,a strong,button{border-radius:var(--border-radius);display:inline-block;font-size:medium;font-weight:700;line-height:var(--line-height);margin:.5rem 0;padding:1rem 2rem}button{font-family:var(--font-family)}button:active{filter:brightness(var(--active-brightness))}button:hover{cursor:pointer;filter:brightness(var(--hover-brightness))}a b,a strong,button{background-color:var(--color-link);border:2px solid var(--color-link);color:var(--color-bg)}a em,a i{border:2px solid var(--color-link);border-radius:var(--border-radius);color:var(--color-link);display:inline-block;padding:1rem 2rem}article aside a{color:var(--color-secondary)}figure{margin:0;padding:0}figure img{max-width:100%}figure figcaption{color:var(--color-text-secondary)}button:disabled,input:disabled{background:var(--color-bg-secondary);border-color:var(--color-bg-secondary);color:var(--color-text-secondary);cursor:not-allowed}button[disabled]:hover{filter:none}form{border:1px solid var(--color-bg-secondary);border-radius:var(--border-radius);box-shadow:var(--box-shadow) var(--color-shadow);display:block;max-width:var(--width-card-wide);min-width:var(--width-card);padding:1.5rem;text-align:var(--justify-normal)}form header{margin:1.5rem 0;padding:1.5rem 0}input,label,select,textarea{display:block;font-size:inherit;max-width:var(--width-card-wide)}input[type=checkbox],input[type=radio]{display:inline-block}input[type=checkbox]+label,input[type=radio]+label{display:inline-block;font-weight:400;position:relative;top:1px}input,select,textarea{border:1px solid var(--color-bg-secondary);border-radius:var(--border-radius);margin-bottom:1rem;padding:.4rem .8rem}input[readonly],textarea[readonly]{background-color:var(--color-bg-secondary)}label{font-weight:700;margin-bottom:.2rem}table{border:1px solid var(--color-bg-secondary);border-radius:var(--border-radius);border-spacing:0;display:inline-block;max-width:100%;overflow-x:auto;padding:0;white-space:nowrap}table td,table th,table tr{padding:.4rem .8rem;text-align:var(--justify-important)}table thead{background-color:var(--color-table);border-collapse:collapse;border-radius:var(--border-radius);color:var(--color-bg);margin:0;padding:0}table thead th:first-child{border-top-left-radius:var(--border-radius)}table thead th:last-child{border-top-right-radius:var(--border-radius)}table thead th:first-child,table tr td:first-child{text-align:var(--justify-normal)}table tr:nth-child(even){background-color:var(--color-accent)}blockquote{display:block;font-size:x-large;line-height:var(--line-height);margin:1rem auto;max-width:var(--width-card-medium);padding:1.5rem 1rem;text-align:var(--justify-important)}blockquote footer{color:var(--color-text-secondary);display:block;font-size:small;line-height:var(--line-height);padding:1.5rem 0}
+
+blockquote {
+  border: 5px solid #ccc;
+}
```

### Comparing `pyboke-0.0.4/src/pyboke/templates/themes/new.css` & `pyboke-0.0.5/src/pyboke/templates/themes/new.css`

 * *Files identical despite different names*

### Comparing `pyboke-0.0.4/src/pyboke/templates/themes/simple.css` & `pyboke-0.0.5/src/pyboke/templates/themes/simple.css`

 * *Files identical despite different names*

### Comparing `pyboke-0.0.4/src/pyboke/templates/themes/water.css` & `pyboke-0.0.5/src/pyboke/templates/themes/water.css`

 * *Files identical despite different names*

### Comparing `pyboke-0.0.4/src/pyboke/templates/title-index.html` & `pyboke-0.0.5/src/pyboke/templates/title-index.html`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-{% extends "base.html" %}
-
-{% block title%}
-  <title>标题索引 - {{ blog.name }}</title>
-{% endblock %}
-
-{% block main %}
-
-<header>
-  <h3>标题索引 - {{ blog.name }}</h3>
-</header>
-
-<div id="back-home"><a href="index.html">&lt;&lt; Home</a></div>
-
-<div id="title-index-list">
-  {% for item in indexes %}
-  <div class="TitleIndexItem">
-    <a href="#{{item.id}}">{{item.name}}</a>
-  </div>
-  {% endfor %}
-</div>
-
-<div id="title-indexes">
-  {% for item in indexes %}
-  <h3 id="{{item.id}}">{{ item.name }}</h3>
-  <ul>
-    {% for art in item.articles %}
-    <li><a href="{{art.id}}.html">{{art.title}}</a></li>
-    {% endfor %}
-  </ul>
-  {% endfor %}
-</div>
-
-{% endblock %}
+{% extends "base.html" %}
+
+{% block title%}
+  <title>标题索引 - {{ blog.name }}</title>
+{% endblock %}
+
+{% block main %}
+
+<header>
+  <h3>标题索引 - {{ blog.name }}</h3>
+</header>
+
+<div id="back-home"><a href="index.html">&lt;&lt; Home</a></div>
+
+<div id="title-index-list">
+  {% for item in indexes %}
+  <div class="TitleIndexItem">
+    <a href="#{{item.id}}">{{item.name}}</a>
+  </div>
+  {% endfor %}
+</div>
+
+<div id="title-indexes">
+  {% for item in indexes %}
+  <h3 id="{{item.id}}">{{ item.name }}</h3>
+  <ul>
+    {% for art in item.articles %}
+    <li><a href="{{art.id}}.html">{{art.title}}</a></li>
+    {% endfor %}
+  </ul>
+  {% endfor %}
+</div>
+
+{% endblock %}
```

### Comparing `pyboke-0.0.4/src/pyboke/tmpl_render.py` & `pyboke-0.0.5/src/pyboke/tmpl_render.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,374 +1,374 @@
-from dataclasses import asdict
-from operator import itemgetter
-from pathlib import Path
-
-import jinja2
-import mistune
-
-from . import model
-from .model import RSS_Atom_XML, Blog_Config_Filename, Blog_Config_Path, \
-    Templates_Folder_Path, TOML_Suffix, ArticleConfig, Metadata_Folder_Path, \
-    Draft_TMPL_Name, Output_Folder_Path, BlogConfig, HTML_Suffix, TitleIndex, \
-    Title_Index_Length, RSS_Entries_Max, MD_Suffix, RSS_Content_Size, RSS_Path, \
-    Articles_Folder_Path, Temp_HTML_Path
-
-# 注意: tmpl_render.py 不能 import util.py
-
-loader = jinja2.FileSystemLoader(Templates_Folder_Path)
-jinja_env = jinja2.Environment(
-    loader=loader, autoescape=jinja2.select_autoescape()
-)
-
-# 渲染时，除了 tmplfile 之外, templates 文件夹里的全部文件都会被复制到 output 文件夹。
-tmplfile = dict(
-    blog_cfg    = Blog_Config_Filename,
-    art_cfg     = "article.toml",
-    draft       = Draft_TMPL_Name,
-    base        = "base.html",
-    index       = "index.html",
-    years       = "years.html",
-    article     = "article.html",
-    random      = "random.html",
-    title_index = "title-index.html",
-    rss         = RSS_Atom_XML,
-)
-
-
-def render_blog_config(cfg):
-    tmpl = jinja_env.get_template(tmplfile["blog_cfg"])
-    blog_toml = tmpl.render(dict(cfg=cfg))
-    print(f"render and write {Blog_Config_Path}")
-    Blog_Config_Path.write_text(blog_toml, encoding="utf-8")
-
-
-def blog_updated_at_now(cfg):
-    """更新博客的更新时间"""
-    cfg.blog_updated = model.now()
-    render_blog_config(cfg)
-
-
-def render_rss(all_articles, cfg, force):
-    if cfg.blog_updated > cfg.rss_updated or force:
-        rss_arts = get_rss_articles(all_articles)
-        really_render_rss(rss_arts, cfg, force)
-
-
-def really_render_rss(articles, blog_cfg, force):
-    """如果不强制渲染，则只在已经存在 RSS (atom.xml) 时才渲染。"""
-    if not force and not RSS_Path.exists():
-        return
-    tmpl = jinja_env.get_template(tmplfile["rss"])
-    xml = tmpl.render(dict(blog=blog_cfg, entries=articles))
-    print(f"render and write {RSS_Path}")
-    RSS_Path.write_text(xml, encoding="utf-8")
-    blog_cfg.rss_updated = model.now()
-    render_blog_config(blog_cfg)
-
-
-def get_rss_articles(all_articles):
-    """
-    按文章的修改时间排列。
-    all_articles 是一个 dict, 已经有 id, 详见 get_all_articles()
-    """
-    sorted_articles = sort_articles(all_articles, key="mtime")
-    recent_arts = get_recent_articles(sorted_articles, RSS_Entries_Max)
-    for art in recent_arts:
-        md_file = Articles_Folder_Path.joinpath(f"{art['id']}{MD_Suffix}")
-        content = md_file.read_text(encoding="utf-8")
-        if len(content) > RSS_Content_Size:
-            content = content[:RSS_Content_Size] + "..."
-        art["content"] = content
-    return recent_arts
-
-
-def get_all_articles():
-    """注意返回的不是 ArticleConfig, 而是 dict"""
-    articles = Metadata_Folder_Path.glob(f"*{TOML_Suffix}")
-    arts = []
-    for art_path in articles:
-        art = ArticleConfig.loads(art_path)
-        art = asdict(art)
-        art["id"] = art_path.stem
-        arts.append(art)
-    return arts
-
-
-def ignore_articles(articles):
-    return [art for art in articles if not art["ignored"]]
-
-
-def sort_articles(articles, key):
-    return sorted(articles, key=itemgetter(key), reverse=True)
-
-def get_all_html_filenames(all_articles):
-    return [art["id"]+HTML_Suffix for art in all_articles]
-
-
-def get_recent_articles(sorted_articles, n):
-    return sorted_articles[:n]
-
-
-def get_articles_in_years(sorted_articles):
-    """获取全部年份的全部文章"""
-    arts = {}
-    for art in sorted_articles:
-        yyyy = art["ctime"][:4]
-        if yyyy in arts:
-            arts[yyyy].append(art)
-        else:
-            arts[yyyy] = [art]
-    return arts
-
-
-def get_title_indexes(sorted_articles):
-    """
-    :return: dict(index, articles)
-    """
-    indexes = {}
-    for art in sorted_articles:
-        index = art["title"][:Title_Index_Length]
-        if index in indexes:
-            indexes[index].articles.append(art)
-        else:
-            index_id = index.encode().hex()
-            indexes[index] = TitleIndex(
-                name=index,
-                id=f"i{index_id}",
-                articles=[art]
-            )
-    return indexes
-
-
-def sort_by_title_index(indexes: dict) -> list:
-    keys = sorted(indexes.keys())
-    result = []
-    for key in keys:
-        item = indexes[key]
-        item.articles = sorted(item.articles, key=itemgetter("title"))
-        result.append(item)
-    return result
-
-
-def render_write_html(page_name: str, data: dict, output_path: Path = None):
-    if output_path is None:
-        output_path = Output_Folder_Path.joinpath(tmplfile[page_name])
-    tmpl = jinja_env.get_template(tmplfile[page_name])
-    html = tmpl.render(data)
-    print(f"render and write {output_path}")
-    output_path.write_text(html, encoding="utf-8")
-
-
-def render_title_index(all_articles, blog_cfg):
-    indexes = get_title_indexes(all_articles)
-    render_write_html("title_index", dict(
-        indexes=sort_by_title_index(indexes),
-        blog=blog_cfg,
-        parent_dir=""
-    ))
-
-
-def render_index_html(recent_articles, html_filenames, blog_cfg):
-    render_write_html("index", dict(
-        blog=blog_cfg,
-        articles=recent_articles,
-        files=html_filenames,
-        parent_dir=""
-    ))
-    render_write_html("random", dict(blog=blog_cfg, files=html_filenames))
-
-
-def render_years_html(year_articles, blog_cfg):
-    render_write_html("years", dict(
-        year_articles=year_articles,
-        blog=blog_cfg,
-        parent_dir=""
-    ))
-
-
-def replace_or_not(art_cfg : ArticleConfig, blog_cfg: BlogConfig):
-    match art_cfg.replace:
-        case 0:
-            return blog_cfg.auto_replace
-        case -1:
-            return False
-        case 1:
-            return True
-
-
-def render_article_html(
-        html_path : Path,
-        md_text : str,
-        blog_cfg: BlogConfig,
-        art_cfg : ArticleConfig,
-):
-    if replace_or_not(art_cfg, blog_cfg):
-        for pair in art_cfg.pairs:
-            md_text = md_text.replace(pair[0], pair[1], 1)
-
-    art = asdict(art_cfg)
-    index_id = art["title"][:Title_Index_Length].encode().hex()
-    art["index_id"] = f"i{index_id}"
-    art["content"] = mistune.html(md_text)
-    render_write_html(
-        "article", dict(blog=blog_cfg, art=art, parent_dir=""), html_path)
-
-
-def delete_articles(all_md_files):
-    """
-    :return: 删除的文件的数量 len(to_be_delete)
-    """
-    all_id = [file.stem for file in all_md_files]
-    all_metadata = Metadata_Folder_Path.glob(f"*{TOML_Suffix}")
-    to_be_delete = [file for file in all_metadata if file.stem not in all_id]
-    result = len(to_be_delete)
-    if result == 0:
-        return 0
-
-    for file in to_be_delete:
-        print(f"DELETE {file}")
-        file.unlink()
-        html_path = html_path_from_md_path(file)
-        print(f"DELETE {html_path}")
-        html_path.unlink()
-
-    return result
-
-
-def update_index_rss(blog_cfg, force=False):
-    all_arts = get_all_articles()
-    render_rss(all_arts, blog_cfg, force=force)
-
-    all_arts = ignore_articles(all_arts)
-    all_arts = sort_articles(all_arts, key="ctime")
-
-    recent_arts = get_recent_articles(all_arts, blog_cfg.home_recent_max)
-    html_filenames = get_all_html_filenames(all_arts)
-    render_index_html(recent_arts, html_filenames, blog_cfg)
-    arts_in_years = get_articles_in_years(all_arts)
-    render_years_html(arts_in_years, blog_cfg)
-    render_title_index(all_arts, blog_cfg)
-
-
-def render_all_articles(blog_cfg: BlogConfig, force: bool):
-    """
-    :return: 发生错误时返回 err_msg: str, 没有错误则返回 False 或空字符串。
-    """
-    all_md_files = Articles_Folder_Path.glob(f"*{MD_Suffix}")
-    all_md_files = list(all_md_files)
-    deleted_count = delete_articles(all_md_files)
-
-    updated_articles = 0
-    for md_file in all_md_files:
-        err, need_to_render = add_or_update_article(md_file, blog_cfg, force)
-        if err:
-            return err
-        if need_to_render:
-            updated_articles += 1
-
-    if force or deleted_count + updated_articles > 0:
-        blog_updated_at_now(blog_cfg)
-        update_index_rss(blog_cfg)
-
-    return False
-
-
-def delete_article(md_path, toml_path, blog_cfg):
-    print(f"DELETE {md_path}")
-    md_path.unlink()
-    print(f"DELETE {toml_path}")
-    toml_path.unlink()
-    html_path = html_path_from_md_path(md_path)
-    print(f"DELETE {html_path}")
-    html_path.unlink()
-    blog_updated_at_now(blog_cfg)
-    update_index_rss(blog_cfg)
-
-
-def render_article(md_file: Path, blog_cfg: BlogConfig, force: bool):
-    """
-    :return: 发生错误时返回 err_msg: str, 没有错误则返回 False 或空字符串。
-    """
-    err, need_to_render = add_or_update_article(md_file, blog_cfg, force)
-
-    if err:
-        return err
-
-    if need_to_render:
-        blog_updated_at_now(blog_cfg)
-        update_index_rss(blog_cfg)
-
-    return False
-
-
-def preview_article(md_file: Path, blog_cfg: BlogConfig):
-    """只渲染一个文件，不执行 update_index_rss() """
-    md_data = md_file.read_bytes()
-    art_toml_path = art_cfg_path_from_md_path(md_file)
-    if art_toml_path.exists():
-        art_cfg = ArticleConfig.loads(art_toml_path)
-    else:
-        art_cfg, err = ArticleConfig.from_md_file(md_file, md_data, blog_cfg.title_length_max)
-        if err:
-            return err
-
-    art_cfg.mtime = model.now()
-    render_article_html(Temp_HTML_Path, md_data.decode(), blog_cfg, art_cfg)
-
-
-def add_or_update_article(md_file: Path, blog_cfg: BlogConfig, force: bool):
-    """
-    在渲染全部文章时，本函数处理其中一个文件。
-
-    :return: 发生错误时返回 (str, None), 否则反回 (None, need_to_render)
-    """
-    md_file_data = md_file.read_bytes()
-    art_cfg_new, err = ArticleConfig.from_md_file(
-        md_file, md_file_data, blog_cfg.title_length_max)
-    if err:
-        return err, False
-
-    art_toml_path = art_cfg_path_from_md_path(md_file)
-    need_to_render = False
-
-    # article toml 不存在，以 art_cfg_new 为准
-    if not art_toml_path.exists():
-        print(f"发现新文章: {art_cfg_new.title}")
-        art_cfg = art_cfg_new
-        need_to_render = True
-    else:
-        # article toml 存在，以 art_toml_path 的文件内容为准
-        art_cfg = ArticleConfig.loads(art_toml_path)
-
-        # 文章内容发生了变化，自动更新 title, checksum, mtime
-        if art_cfg.checksum != art_cfg_new.checksum:
-            print(f"更新: {art_cfg_new.title}")
-            art_cfg.title = art_cfg_new.title
-            art_cfg.checksum = art_cfg_new.checksum
-            art_cfg.mtime = model.now()
-            need_to_render = True
-
-    # 文章内容有变化，需要渲染 toml
-    if need_to_render:
-        tmpl = jinja_env.get_template(tmplfile["art_cfg"])
-        art_toml_data = tmpl.render(dict(art=art_cfg))
-        print(f"render and write {art_toml_path}")
-        art_toml_path.write_text(art_toml_data, encoding="utf-8")
-
-    # 需要渲染 html
-    if need_to_render or force:
-        html_path = html_path_from_md_path(md_file)
-        render_article_html(html_path, md_file_data.decode(), blog_cfg, art_cfg)
-
-    return None, need_to_render
-
-
-def art_cfg_path_from_md_path(md_path):
-    """根据 markdown 文件的路径得出 toml 文件的路径"""
-    name = md_path.with_suffix(TOML_Suffix).name
-    return Metadata_Folder_Path.joinpath(name)
-
-
-def html_path_from_md_path(article_path):
-    """根据文章 (markdown 或 toml) 的路径得出 html 文件的路径"""
-    name = article_path.with_suffix(HTML_Suffix).name
-    return Output_Folder_Path.joinpath(name)
+from dataclasses import asdict
+from operator import itemgetter
+from pathlib import Path
+
+import jinja2
+import mistune
+
+from . import model
+from .model import RSS_Atom_XML, Blog_Config_Filename, Blog_Config_Path, \
+    Templates_Folder_Path, TOML_Suffix, ArticleConfig, Metadata_Folder_Path, \
+    Draft_TMPL_Name, Output_Folder_Path, BlogConfig, HTML_Suffix, TitleIndex, \
+    Title_Index_Length, RSS_Entries_Max, MD_Suffix, RSS_Content_Size, RSS_Path, \
+    Articles_Folder_Path, Temp_HTML_Path
+
+# 注意: tmpl_render.py 不能 import util.py
+
+loader = jinja2.FileSystemLoader(Templates_Folder_Path)
+jinja_env = jinja2.Environment(
+    loader=loader, autoescape=jinja2.select_autoescape()
+)
+
+# 渲染时，除了 tmplfile 之外, templates 文件夹里的全部文件都会被复制到 output 文件夹。
+tmplfile = dict(
+    blog_cfg    = Blog_Config_Filename,
+    art_cfg     = "article.toml",
+    draft       = Draft_TMPL_Name,
+    base        = "base.html",
+    index       = "index.html",
+    years       = "years.html",
+    article     = "article.html",
+    random      = "random.html",
+    title_index = "title-index.html",
+    rss         = RSS_Atom_XML,
+)
+
+
+def render_blog_config(cfg):
+    tmpl = jinja_env.get_template(tmplfile["blog_cfg"])
+    blog_toml = tmpl.render(dict(cfg=cfg))
+    print(f"render and write {Blog_Config_Path}")
+    Blog_Config_Path.write_text(blog_toml, encoding="utf-8")
+
+
+def blog_updated_at_now(cfg):
+    """更新博客的更新时间"""
+    cfg.blog_updated = model.now()
+    render_blog_config(cfg)
+
+
+def render_rss(all_articles, cfg, force):
+    if cfg.blog_updated > cfg.rss_updated or force:
+        rss_arts = get_rss_articles(all_articles)
+        really_render_rss(rss_arts, cfg, force)
+
+
+def really_render_rss(articles, blog_cfg, force):
+    """如果不强制渲染，则只在已经存在 RSS (atom.xml) 时才渲染。"""
+    if not force and not RSS_Path.exists():
+        return
+    tmpl = jinja_env.get_template(tmplfile["rss"])
+    xml = tmpl.render(dict(blog=blog_cfg, entries=articles))
+    print(f"render and write {RSS_Path}")
+    RSS_Path.write_text(xml, encoding="utf-8")
+    blog_cfg.rss_updated = model.now()
+    render_blog_config(blog_cfg)
+
+
+def get_rss_articles(all_articles):
+    """
+    按文章的修改时间排列。
+    all_articles 是一个 dict, 已经有 id, 详见 get_all_articles()
+    """
+    sorted_articles = sort_articles(all_articles, key="mtime")
+    recent_arts = get_recent_articles(sorted_articles, RSS_Entries_Max)
+    for art in recent_arts:
+        md_file = Articles_Folder_Path.joinpath(f"{art['id']}{MD_Suffix}")
+        content = md_file.read_text(encoding="utf-8")
+        if len(content) > RSS_Content_Size:
+            content = content[:RSS_Content_Size] + "..."
+        art["content"] = content
+    return recent_arts
+
+
+def get_all_articles():
+    """注意返回的不是 ArticleConfig, 而是 dict"""
+    articles = Metadata_Folder_Path.glob(f"*{TOML_Suffix}")
+    arts = []
+    for art_path in articles:
+        art = ArticleConfig.loads(art_path)
+        art = asdict(art)
+        art["id"] = art_path.stem
+        arts.append(art)
+    return arts
+
+
+def ignore_articles(articles):
+    return [art for art in articles if not art["ignored"]]
+
+
+def sort_articles(articles, key):
+    return sorted(articles, key=itemgetter(key), reverse=True)
+
+def get_all_html_filenames(all_articles):
+    return [art["id"]+HTML_Suffix for art in all_articles]
+
+
+def get_recent_articles(sorted_articles, n):
+    return sorted_articles[:n]
+
+
+def get_articles_in_years(sorted_articles):
+    """获取全部年份的全部文章"""
+    arts = {}
+    for art in sorted_articles:
+        yyyy = art["ctime"][:4]
+        if yyyy in arts:
+            arts[yyyy].append(art)
+        else:
+            arts[yyyy] = [art]
+    return arts
+
+
+def get_title_indexes(sorted_articles):
+    """
+    :return: dict(index, articles)
+    """
+    indexes = {}
+    for art in sorted_articles:
+        index = art["title"][:Title_Index_Length]
+        if index in indexes:
+            indexes[index].articles.append(art)
+        else:
+            index_id = index.encode().hex()
+            indexes[index] = TitleIndex(
+                name=index,
+                id=f"i{index_id}",
+                articles=[art]
+            )
+    return indexes
+
+
+def sort_by_title_index(indexes: dict) -> list:
+    keys = sorted(indexes.keys())
+    result = []
+    for key in keys:
+        item = indexes[key]
+        item.articles = sorted(item.articles, key=itemgetter("title"))
+        result.append(item)
+    return result
+
+
+def render_write_html(page_name: str, data: dict, output_path: Path = None):
+    if output_path is None:
+        output_path = Output_Folder_Path.joinpath(tmplfile[page_name])
+    tmpl = jinja_env.get_template(tmplfile[page_name])
+    html = tmpl.render(data)
+    print(f"render and write {output_path}")
+    output_path.write_text(html, encoding="utf-8")
+
+
+def render_title_index(all_articles, blog_cfg):
+    indexes = get_title_indexes(all_articles)
+    render_write_html("title_index", dict(
+        indexes=sort_by_title_index(indexes),
+        blog=blog_cfg,
+        parent_dir=""
+    ))
+
+
+def render_index_html(recent_articles, html_filenames, blog_cfg):
+    render_write_html("index", dict(
+        blog=blog_cfg,
+        articles=recent_articles,
+        files=html_filenames,
+        parent_dir=""
+    ))
+    render_write_html("random", dict(blog=blog_cfg, files=html_filenames))
+
+
+def render_years_html(year_articles, blog_cfg):
+    render_write_html("years", dict(
+        year_articles=year_articles,
+        blog=blog_cfg,
+        parent_dir=""
+    ))
+
+
+def replace_or_not(art_cfg : ArticleConfig, blog_cfg: BlogConfig):
+    match art_cfg.replace:
+        case 0:
+            return blog_cfg.auto_replace
+        case -1:
+            return False
+        case 1:
+            return True
+
+
+def render_article_html(
+        html_path : Path,
+        md_text : str,
+        blog_cfg: BlogConfig,
+        art_cfg : ArticleConfig,
+):
+    if replace_or_not(art_cfg, blog_cfg):
+        for pair in art_cfg.pairs:
+            md_text = md_text.replace(pair[0], pair[1], 1)
+
+    art = asdict(art_cfg)
+    index_id = art["title"][:Title_Index_Length].encode().hex()
+    art["index_id"] = f"i{index_id}"
+    art["content"] = mistune.html(md_text)
+    render_write_html(
+        "article", dict(blog=blog_cfg, art=art, parent_dir=""), html_path)
+
+
+def delete_articles(all_md_files):
+    """
+    :return: 删除的文件的数量 len(to_be_delete)
+    """
+    all_id = [file.stem for file in all_md_files]
+    all_metadata = Metadata_Folder_Path.glob(f"*{TOML_Suffix}")
+    to_be_delete = [file for file in all_metadata if file.stem not in all_id]
+    result = len(to_be_delete)
+    if result == 0:
+        return 0
+
+    for file in to_be_delete:
+        print(f"DELETE {file}")
+        file.unlink()
+        html_path = html_path_from_md_path(file)
+        print(f"DELETE {html_path}")
+        html_path.unlink()
+
+    return result
+
+
+def update_index_rss(blog_cfg, force=False):
+    all_arts = get_all_articles()
+    render_rss(all_arts, blog_cfg, force=force)
+
+    all_arts = ignore_articles(all_arts)
+    all_arts = sort_articles(all_arts, key="ctime")
+
+    recent_arts = get_recent_articles(all_arts, blog_cfg.home_recent_max)
+    html_filenames = get_all_html_filenames(all_arts)
+    render_index_html(recent_arts, html_filenames, blog_cfg)
+    arts_in_years = get_articles_in_years(all_arts)
+    render_years_html(arts_in_years, blog_cfg)
+    render_title_index(all_arts, blog_cfg)
+
+
+def render_all_articles(blog_cfg: BlogConfig, force: bool):
+    """
+    :return: 发生错误时返回 err_msg: str, 没有错误则返回 False 或空字符串。
+    """
+    all_md_files = Articles_Folder_Path.glob(f"*{MD_Suffix}")
+    all_md_files = list(all_md_files)
+    deleted_count = delete_articles(all_md_files)
+
+    updated_articles = 0
+    for md_file in all_md_files:
+        err, need_to_render = add_or_update_article(md_file, blog_cfg, force)
+        if err:
+            return err
+        if need_to_render:
+            updated_articles += 1
+
+    if force or deleted_count + updated_articles > 0:
+        blog_updated_at_now(blog_cfg)
+        update_index_rss(blog_cfg)
+
+    return False
+
+
+def delete_article(md_path, toml_path, blog_cfg):
+    print(f"DELETE {md_path}")
+    md_path.unlink()
+    print(f"DELETE {toml_path}")
+    toml_path.unlink()
+    html_path = html_path_from_md_path(md_path)
+    print(f"DELETE {html_path}")
+    html_path.unlink()
+    blog_updated_at_now(blog_cfg)
+    update_index_rss(blog_cfg)
+
+
+def render_article(md_file: Path, blog_cfg: BlogConfig, force: bool):
+    """
+    :return: 发生错误时返回 err_msg: str, 没有错误则返回 False 或空字符串。
+    """
+    err, need_to_render = add_or_update_article(md_file, blog_cfg, force)
+
+    if err:
+        return err
+
+    if need_to_render:
+        blog_updated_at_now(blog_cfg)
+        update_index_rss(blog_cfg)
+
+    return False
+
+
+def preview_article(md_file: Path, blog_cfg: BlogConfig):
+    """只渲染一个文件，不执行 update_index_rss() """
+    md_data = md_file.read_bytes()
+    art_toml_path = art_cfg_path_from_md_path(md_file)
+    if art_toml_path.exists():
+        art_cfg = ArticleConfig.loads(art_toml_path)
+    else:
+        art_cfg, err = ArticleConfig.from_md_file(md_file, md_data, blog_cfg.title_length_max)
+        if err:
+            return err
+
+    art_cfg.mtime = model.now()
+    render_article_html(Temp_HTML_Path, md_data.decode(), blog_cfg, art_cfg)
+
+
+def add_or_update_article(md_file: Path, blog_cfg: BlogConfig, force: bool):
+    """
+    在渲染全部文章时，本函数处理其中一个文件。
+
+    :return: 发生错误时返回 (str, None), 否则反回 (None, need_to_render)
+    """
+    md_file_data = md_file.read_bytes()
+    art_cfg_new, err = ArticleConfig.from_md_file(
+        md_file, md_file_data, blog_cfg.title_length_max)
+    if err:
+        return err, False
+
+    art_toml_path = art_cfg_path_from_md_path(md_file)
+    need_to_render = False
+
+    # article toml 不存在，以 art_cfg_new 为准
+    if not art_toml_path.exists():
+        print(f"发现新文章: {art_cfg_new.title}")
+        art_cfg = art_cfg_new
+        need_to_render = True
+    else:
+        # article toml 存在，以 art_toml_path 的文件内容为准
+        art_cfg = ArticleConfig.loads(art_toml_path)
+
+        # 文章内容发生了变化，自动更新 title, checksum, mtime
+        if art_cfg.checksum != art_cfg_new.checksum:
+            print(f"更新: {art_cfg_new.title}")
+            art_cfg.title = art_cfg_new.title
+            art_cfg.checksum = art_cfg_new.checksum
+            art_cfg.mtime = model.now()
+            need_to_render = True
+
+    # 文章内容有变化，需要渲染 toml
+    if need_to_render:
+        tmpl = jinja_env.get_template(tmplfile["art_cfg"])
+        art_toml_data = tmpl.render(dict(art=art_cfg))
+        print(f"render and write {art_toml_path}")
+        art_toml_path.write_text(art_toml_data, encoding="utf-8")
+
+    # 需要渲染 html
+    if need_to_render or force:
+        html_path = html_path_from_md_path(md_file)
+        render_article_html(html_path, md_file_data.decode(), blog_cfg, art_cfg)
+
+    return None, need_to_render
+
+
+def art_cfg_path_from_md_path(md_path):
+    """根据 markdown 文件的路径得出 toml 文件的路径"""
+    name = md_path.with_suffix(TOML_Suffix).name
+    return Metadata_Folder_Path.joinpath(name)
+
+
+def html_path_from_md_path(article_path):
+    """根据文章 (markdown 或 toml) 的路径得出 html 文件的路径"""
+    name = article_path.with_suffix(HTML_Suffix).name
+    return Output_Folder_Path.joinpath(name)
```

### Comparing `pyboke-0.0.4/src/pyboke/util.py` & `pyboke-0.0.5/src/pyboke/util.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,183 +1,184 @@
-import hashlib
-import os
-import shutil
-from pathlib import Path
-
-from . import model
-from .model import Blog_Config_Path, CWD, Templates_Folder_Name, Articles_Folder_Path, \
-    Templates_Folder_Path, Output_Folder_Path, BlogConfig, Pics_Folder_Path, RSS_Atom_XML, \
-    Metadata_Folder_Path, Drafts_Folder_Path, Default_Theme_Name, Themes_Folder_Path, \
-    Theme_CSS_Path, MD_Suffix
-from .tmpl_render import render_blog_config, tmplfile, art_cfg_path_from_md_path, \
-    html_path_from_md_path
-
-
-def dir_not_empty(path):
-    return True if os.listdir(path) else False
-
-
-def copy_templates():
-    src_folder = Path(__file__).parent.joinpath(Templates_Folder_Name)
-    shutil.copytree(src_folder, Templates_Folder_Path)
-
-
-def copy_static_files():
-    static_files = Templates_Folder_Path.glob("*")
-    for src in static_files:
-        if src.is_file() and src.name not in tmplfile.values():
-            dst = Output_Folder_Path.joinpath(src.name)
-            print(f"Copy static file to {dst}")
-            shutil.copyfile(src, dst)
-    rgignore_src = Output_Folder_Path.joinpath(".rgignore")
-    rgignore_dst = CWD.joinpath(".rgignore")
-    print(f"Move {rgignore_src} to {rgignore_dst}")
-    shutil.move(rgignore_src, rgignore_dst)
-
-
-def copy_theme_css(name):
-    name = name.lower()
-    theme_css_file = Themes_Folder_Path.joinpath(f"{name}.css")
-    shutil.copyfile(theme_css_file, Theme_CSS_Path)
-    print(f"Using theme: {name}")
-
-
-def init_blog():
-    """
-    在一个空文件夹中初始化一个博客。
-
-    :return: 发生错误时返回 err_msg: str, 没有错误则返回 False 或空字符串。
-    """
-    if dir_not_empty(CWD):
-        return f"Folder Not Empty: {CWD}"
-
-    Drafts_Folder_Path.mkdir()
-    Articles_Folder_Path.mkdir()
-    Metadata_Folder_Path.mkdir()
-    Output_Folder_Path.mkdir()
-    Pics_Folder_Path.mkdir()
-    copy_templates()
-    copy_static_files()
-    copy_theme_css(Default_Theme_Name)
-    render_blog_config(BlogConfig.default())
-    print(f"请用文本编辑器打开 {Blog_Config_Path} 填写博客名称、作者名称等。")
-
-
-def blog_file_folders_exist():
-    return Drafts_Folder_Path.exists()\
-        and Articles_Folder_Path.exists()\
-        and Pics_Folder_Path.exists()\
-        and Metadata_Folder_Path.exists()\
-        and Output_Folder_Path.exists()\
-        and Templates_Folder_Path.exists()\
-        and Blog_Config_Path.exists()
-
-
-def ensure_blog_config(check_website=False):
-    """
-    :return: 发生错误时返回 (err_msg, None), 没有错误则返回 (False, BlogConfig)
-    """
-    cfg = BlogConfig.loads()
-    default_cfg = BlogConfig.default()
-
-    cfg.name = cfg.name.strip()
-    if not cfg.name or cfg.name == default_cfg.name:
-        return f"请用文本编辑器打开 {Blog_Config_Path} 填写博客名称", None
-
-    cfg.author = cfg.author.strip()
-    if not cfg.author or cfg.author == default_cfg.author:
-        return f"请用文本编辑器打开 {Blog_Config_Path} 填写作者名称", None
-
-    if cfg.home_recent_max <= 0:
-        return f"请用文本编辑器打开 {Blog_Config_Path} 填写 home_recent_max, 必须大于零", None
-
-    if cfg.home_recent_max <= 0:
-        return f"请用文本编辑器打开 {Blog_Config_Path} 填写 title_length_max, 必须大于零", None
-
-    cfg.website = cfg.website.strip()
-    if check_website:
-        if cfg.website == "" or cfg.website == default_cfg.website:
-            return f"为了生成 RSS, 请用文本编辑器打开 {Blog_Config_Path} 填写博客网址(website)", None
-
-    changed = False
-
-    if cfg.website and cfg.website != default_cfg.website:
-        cfg.website = cfg.website.removesuffix("/") + "/"
-        rss_link = cfg.website + RSS_Atom_XML
-        if cfg.rss_link != rss_link:
-            cfg.rss_link = rss_link
-            changed = True
-
-    cfg.uuid = cfg.uuid.strip()
-    if not cfg.uuid:
-        cfg.uuid = hashlib.sha1(
-            (cfg.name + cfg.author + str(model.now())).encode()
-        ).hexdigest()
-        changed = True
-
-    if changed:
-        render_blog_config(cfg)
-
-    return False, cfg
-
-
-def check_filename(file: Path, parent_dir: Path, ensure_not_exist=False):
-    """
-    确保 filepath 只包含合法字符，后缀名为 '.md', 并确保其在 parent_dir 里。
-    如果 ensure_not_exist 为真，则需要确保 parent_dir 里没有同名文件。
-
-    :return: 发生错误时返回 err_msg: str, 没有错误则返回 False 或空字符串。
-    """
-    if file.suffix != MD_Suffix:
-        return f"后缀名不是 '{MD_Suffix}': {file}"
-
-    names = ["index.md", "years.md", "random.md", "title-index.md", "temp.md"]
-    if file.name.lower() in names:
-        return f"文件名不可用 {file.name}"
-    if err := model.check_filename(file.name):
-        return err
-
-    if ensure_not_exist:
-        file_path = parent_dir.joinpath(file.name)
-        if file_path.exists():
-            return f"文件已存在: {file_path}"
-    else:
-        if not file.parent.samefile(parent_dir):
-            return f"不在 {parent_dir.name} 文件夹内: {file}"
-
-    return False
-
-
-def get_themes():
-    themes = Themes_Folder_Path.glob("*.css")
-    return [theme.stem for theme in themes]
-
-
-def change_theme(name, blog_cfg):
-    copy_theme_css(name)
-    blog_cfg.current_theme = name.lower()
-    render_blog_config(blog_cfg)
-
-
-def rename(old_path, new_path):
-    if not old_path.exists():
-        return f"文件不存在: {old_path}"
-    if err := check_filename(old_path, Articles_Folder_Path):
-        return err
-    if err := check_filename(new_path, Articles_Folder_Path, ensure_not_exist=True):
-        return err
-
-    print(f"rename(md/toml/html): {old_path.stem} => {new_path.stem}")
-    new_md_path = Articles_Folder_Path.joinpath(new_path.name)
-    old_path.rename(new_md_path)
-    old_toml_path = art_cfg_path_from_md_path(old_path)
-    new_toml_path = art_cfg_path_from_md_path(new_md_path)
-    old_toml_path.rename(new_toml_path)
-    old_html_path = html_path_from_md_path(old_path)
-    new_html_path = html_path_from_md_path(new_md_path)
-    old_html_path.rename(new_html_path)
-    return False
-
-
-def articles_count():
-    files = Metadata_Folder_Path.glob("*.toml")
-    return sum(1 for _ in files)
+import hashlib
+import os
+import shutil
+from pathlib import Path
+
+from . import model
+from .model import Blog_Config_Path, CWD, Templates_Folder_Name, Articles_Folder_Path, \
+    Templates_Folder_Path, Output_Folder_Path, BlogConfig, Pics_Folder_Path, RSS_Atom_XML, \
+    Metadata_Folder_Path, Drafts_Folder_Path, Default_Theme_Name, Themes_Folder_Path, \
+    Theme_CSS_Path, MD_Suffix
+from .tmpl_render import render_blog_config, tmplfile, art_cfg_path_from_md_path, \
+    html_path_from_md_path
+
+
+def dir_not_empty(path):
+    return True if os.listdir(path) else False
+
+
+def copy_templates():
+    src_folder = Path(__file__).parent.joinpath(Templates_Folder_Name)
+    shutil.copytree(src_folder, Templates_Folder_Path)
+
+
+def copy_static_files():
+    static_files = Templates_Folder_Path.glob("*")
+    for src in static_files:
+        if src.is_file() and src.name not in tmplfile.values():
+            dst = Output_Folder_Path.joinpath(src.name)
+            print(f"Copy static file to {dst}")
+            shutil.copyfile(src, dst)
+    rgignore_src = Output_Folder_Path.joinpath(".rgignore")
+    rgignore_dst = CWD.joinpath(".rgignore")
+    print(f"Move {rgignore_src} to {rgignore_dst}")
+    shutil.move(rgignore_src, rgignore_dst)
+
+
+def copy_theme_css(name):
+    name = name.lower()
+    theme_css_file = Themes_Folder_Path.joinpath(f"{name}.css")
+    shutil.copyfile(theme_css_file, Theme_CSS_Path)
+    print(f"Using theme: {name}")
+
+
+def init_blog():
+    """
+    在一个空文件夹中初始化一个博客。
+
+    :return: 发生错误时返回 err_msg: str, 没有错误则返回空字符串。
+    """
+    if dir_not_empty(CWD):
+        return f"Folder Not Empty: {CWD}"
+
+    Drafts_Folder_Path.mkdir()
+    Articles_Folder_Path.mkdir()
+    Metadata_Folder_Path.mkdir()
+    Output_Folder_Path.mkdir()
+    Pics_Folder_Path.mkdir()
+    copy_templates()
+    copy_static_files()
+    copy_theme_css(Default_Theme_Name)
+    render_blog_config(BlogConfig.default())
+    print(f"请用文本编辑器打开 {Blog_Config_Path} 填写博客名称、作者名称等。")
+    return ""
+
+
+def blog_file_folders_exist():
+    return Drafts_Folder_Path.exists()\
+        and Articles_Folder_Path.exists()\
+        and Pics_Folder_Path.exists()\
+        and Metadata_Folder_Path.exists()\
+        and Output_Folder_Path.exists()\
+        and Templates_Folder_Path.exists()\
+        and Blog_Config_Path.exists()
+
+
+def ensure_blog_config(check_website=False):
+    """
+    :return: 发生错误时返回 (err_msg, None), 没有错误则返回 (False, BlogConfig)
+    """
+    cfg = BlogConfig.loads()
+    default_cfg = BlogConfig.default()
+
+    cfg.name = cfg.name.strip()
+    if not cfg.name or cfg.name == default_cfg.name:
+        return f"请用文本编辑器打开 {Blog_Config_Path} 填写博客名称", None
+
+    cfg.author = cfg.author.strip()
+    if not cfg.author or cfg.author == default_cfg.author:
+        return f"请用文本编辑器打开 {Blog_Config_Path} 填写作者名称", None
+
+    if cfg.home_recent_max <= 0:
+        return f"请用文本编辑器打开 {Blog_Config_Path} 填写 home_recent_max, 必须大于零", None
+
+    if cfg.home_recent_max <= 0:
+        return f"请用文本编辑器打开 {Blog_Config_Path} 填写 title_length_max, 必须大于零", None
+
+    cfg.website = cfg.website.strip()
+    if check_website:
+        if cfg.website == "" or cfg.website == default_cfg.website:
+            return f"为了生成 RSS, 请用文本编辑器打开 {Blog_Config_Path} 填写博客网址(website)", None
+
+    changed = False
+
+    if cfg.website and cfg.website != default_cfg.website:
+        cfg.website = cfg.website.removesuffix("/") + "/"
+        rss_link = cfg.website + RSS_Atom_XML
+        if cfg.rss_link != rss_link:
+            cfg.rss_link = rss_link
+            changed = True
+
+    cfg.uuid = cfg.uuid.strip()
+    if not cfg.uuid:
+        cfg.uuid = hashlib.sha1(
+            (cfg.name + cfg.author + str(model.now())).encode()
+        ).hexdigest()
+        changed = True
+
+    if changed:
+        render_blog_config(cfg)
+
+    return False, cfg
+
+
+def check_filename(file: Path, parent_dir: Path, ensure_not_exist=False):
+    """
+    确保 filepath 只包含合法字符，后缀名为 '.md', 并确保其在 parent_dir 里。
+    如果 ensure_not_exist 为真，则需要确保 parent_dir 里没有同名文件。
+
+    :return: 发生错误时返回 err_msg: str, 没有错误则返回 False 或空字符串。
+    """
+    if file.suffix != MD_Suffix:
+        return f"后缀名不是 '{MD_Suffix}': {file}"
+
+    names = ["index.md", "years.md", "random.md", "title-index.md", "temp.md"]
+    if file.name.lower() in names:
+        return f"文件名不可用 {file.name}"
+    if err := model.check_filename(file.name):
+        return err
+
+    if ensure_not_exist:
+        file_path = parent_dir.joinpath(file.name)
+        if file_path.exists():
+            return f"文件已存在: {file_path}"
+    else:
+        if not file.parent.samefile(parent_dir):
+            return f"不在 {parent_dir.name} 文件夹内: {file}"
+
+    return False
+
+
+def get_themes():
+    themes = Themes_Folder_Path.glob("*.css")
+    return [theme.stem for theme in themes]
+
+
+def change_theme(name, blog_cfg):
+    copy_theme_css(name)
+    blog_cfg.current_theme = name.lower()
+    render_blog_config(blog_cfg)
+
+
+def rename(old_path, new_path):
+    if not old_path.exists():
+        return f"文件不存在: {old_path}"
+    if err := check_filename(old_path, Articles_Folder_Path):
+        return err
+    if err := check_filename(new_path, Articles_Folder_Path, ensure_not_exist=True):
+        return err
+
+    print(f"rename(md/toml/html): {old_path.stem} => {new_path.stem}")
+    new_md_path = Articles_Folder_Path.joinpath(new_path.name)
+    old_path.rename(new_md_path)
+    old_toml_path = art_cfg_path_from_md_path(old_path)
+    new_toml_path = art_cfg_path_from_md_path(new_md_path)
+    old_toml_path.rename(new_toml_path)
+    old_html_path = html_path_from_md_path(old_path)
+    new_html_path = html_path_from_md_path(new_md_path)
+    old_html_path.rename(new_html_path)
+    return False
+
+
+def articles_count():
+    files = Metadata_Folder_Path.glob("*.toml")
+    return sum(1 for _ in files)
```

### Comparing `pyboke-0.0.4/PKG-INFO` & `pyboke-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyboke
-Version: 0.0.4
+Version: 0.0.5
 Summary: pyboke: Static Blog Generator. (尽可能简单的静态博客生成器)
 Author-email: ahui <102419@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: arrow
 Requires-Dist: click
@@ -41,44 +41,47 @@
 推荐使用 [pyenv](https://github.com/pyenv/pyenv) 或
 [miniconda](https://docs.conda.io/en/latest/miniconda.html)
 来安装最新版本的 Python。
 
 例如，安装 miniconda 后，可以这样创建 3.10 环境：
 
 ```sh
-$ conda create --name py310 python=3.10
+$ conda create --name py310 python=3.10.6
 $ conda activate py310
 ```
 
 安装非常简单，只要 `pip install pyboke` 即可。  
-另外推荐采用 [pipx](https://pypa.github.io/pipx/) 进行安装。
+
+(另外推荐了解一下 [pipx](https://pypa.github.io/pipx/)
+这是用来安装 Python 命令行软件的优秀工具）
 
 ## 创建一个新博客
 
 1. `mkdir my-blog` _(新建一个空文件夹)_
 2. `cd my-blog` _(进入空文件夹内)_
-3. `boke init` _(初始化博客，创建一些必要的文件和文件夹)_
+3. `boke init` _(初始化博客)_
 
-然后可以在当前文件内看到以下文件与文件夹：
+成功后，可以在当前文件夹内看到以下文件与文件夹：
 
 - **articles** (全部文章都在这里，采用 markdown 格式, `.md` 后缀名)
 - **articles/metadata** (与 markdown 文件一一对应的 toml 文件)
 - **drafts** (待发布的草稿放在这里)
 - **output** (程序生成的 HTML, RSS 等文件将会输出到该文件夹)
 - **templates** (Jinja2模板 与 CSS文件)
-- **boke.toml** (博客名称、作者名称等)
+- **blog.toml** (博客名称、作者名称等)
 
-请用文本编辑器打开 boke.toml 填写博客名称、作者名称等。
+请用文本编辑器打开 blog.toml 填写博客名称、作者名称等。
 
 执行命令 `boke -info` 查看博客信息。
 
 ## 添加文章
 
 - 文件后缀必须是 ".md", 文件内容必须采用 Markdown 格式, 使用 utf-8 编码。
 - 文件名只能使用 0-9, a-z, A-Z, _(下划线), -(短横线), .(点)。
+- 文件名会成为网址的一部分, 因此建议尽量短一点.
 - 把 md 文件放入 articles 文件夹，执行 `boke render articles/filename`,
   会在 **articles/metadata** 文件夹里生成 TOML 文件，
   在 **output** 文件夹生成 HTML 文件。
 - 其中, TOML 里有文章的标题、作者、创建日期、修改日期等信息。
 - 大多数情况下你都可以忘记 articles/metadata 里的 toml 文件，不需要修改它。
 - 推荐使用 `boke new` 和 `boke post` 命令，详见后文 **草稿** 部分。
 
@@ -261,14 +264,27 @@
 
 例如可以使用 [ripgrep](https://github.com/BurntSushi/ripgrep), 在博客的根目录执行
 `rg -i 'keyword' articles` 即可查找包含 `keyword` 的文章，其中 `-i` 表示不分大小写。
 
 如果不搜索文章正文内容，只搜索文章标题，可打开网页 title-index.html(标题索引),
 按 `Ctrl+F` 在页面内搜索。
 
+## 建议使用终端文本编辑器
+
+本软件的大部分操作都需要在终端输入命令, 有时需要稍稍修改一下 toml,
+这种情况下如果切换到文本编辑器去操作, 会感觉有点麻烦, 因此建议使用类似
+Vim/Emacs 的终端文本编辑器, 就很方便.
+
+我找到了 [micro](https://github.com/zyedidia/micro), 它类似 Vim/Emacs
+并且更轻, 也更易学易用, 优点:
+
+- 启动速度飞快, 感觉非常轻巧.
+- 非常易学易用, 支持鼠标选择, 以及用 Ctrl-C / Ctrl-V 来复制黏贴.  
+  支持 Ctrl-S 保存 / Ctrl-A 全选等符合现代习惯的快捷键.
+
 
 [^css-themes]: 例如这里就有一些极简 CSS 主题: [github.com/dohliam/dropin-minimal-css](https://github.com/dohliam/dropin-minimal-css)
 
 ## 我的博客
 
 作为参考，可以看看我的博客，就是用 PyBoke 生成的。
 <https://ahui2016.github.io/>
```

