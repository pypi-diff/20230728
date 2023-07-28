# Comparing `tmp/mdx_gh_links-0.3.tar.gz` & `tmp/mdx_gh_links-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mdx_gh_links-0.3.tar", last modified: Mon Jul 18 19:44:40 2022, max compression
+gzip compressed data, was "mdx_gh_links-0.3.1.tar", last modified: Fri Jul 28 19:09:31 2023, max compression
```

## Comparing `mdx_gh_links-0.3.tar` & `mdx_gh_links-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2022-07-18 19:44:40.330225 mdx_gh_links-0.3/
--rw-rw-rw-   0        0        0     1554 2022-07-18 19:14:10.000000 mdx_gh_links-0.3/LICENSE
--rw-rw-rw-   0        0        0       36 2022-07-18 19:14:10.000000 mdx_gh_links-0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1141 2022-07-18 19:44:40.330225 mdx_gh_links-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     7580 2022-07-18 19:38:17.000000 mdx_gh_links-0.3/README.md
-drwxrwxrwx   0        0        0        0 2022-07-18 19:44:40.314603 mdx_gh_links-0.3/mdx_gh_links.egg-info/
--rw-rw-rw-   0        0        0     1141 2022-07-18 19:44:40.000000 mdx_gh_links-0.3/mdx_gh_links.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2022-07-18 19:44:40.000000 mdx_gh_links-0.3/mdx_gh_links.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-18 19:44:40.000000 mdx_gh_links-0.3/mdx_gh_links.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2022-07-18 19:44:40.000000 mdx_gh_links-0.3/mdx_gh_links.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-07-18 19:44:40.000000 mdx_gh_links-0.3/mdx_gh_links.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5002 2022-07-18 19:14:10.000000 mdx_gh_links-0.3/mdx_gh_links.py
--rw-rw-rw-   0        0        0      112 2022-07-18 19:44:40.330225 mdx_gh_links-0.3/setup.cfg
--rw-rw-rw-   0        0        0     2865 2022-07-18 19:38:17.000000 mdx_gh_links-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:09:31.951486 mdx_gh_links-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-28 19:09:21.000000 mdx_gh_links-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-07-28 19:09:31.951486 mdx_gh_links-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-28 19:09:21.000000 mdx_gh_links-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:09:31.951486 mdx_gh_links-0.3.1/mdx_gh_links.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-07-28 19:09:31.000000 mdx_gh_links-0.3.1/mdx_gh_links.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-28 19:09:31.000000 mdx_gh_links-0.3.1/mdx_gh_links.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:09:31.000000 mdx_gh_links-0.3.1/mdx_gh_links.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 19:09:31.000000 mdx_gh_links-0.3.1/mdx_gh_links.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 19:09:31.000000 mdx_gh_links-0.3.1/mdx_gh_links.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-28 19:09:21.000000 mdx_gh_links-0.3.1/mdx_gh_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-28 19:09:21.000000 mdx_gh_links-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:09:31.951486 mdx_gh_links-0.3.1/setup.cfg
```

### Comparing `mdx_gh_links-0.3/LICENSE` & `mdx_gh_links-0.3.1/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-Python-Markdown Github-Links Extension is Copyright (c) 2017-2018 by Waylan
-Limberg. All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-*   Redistributions of source code must retain the above copyright
-    notice, this list of conditions and the following disclaimer.
-*   Redistributions in binary form must reproduce the above copyright
-    notice, this list of conditions and the following disclaimer in the
-    documentation and/or other materials provided with the distribution.
-*   Neither the name of HTMLTree nor the names of its contributors may be
-    used to endorse or promote products derived from this software without
-    specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY WAYLAN LIMBERG ''AS IS'' AND ANY
-EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL ANY CONTRIBUTORS TO Github-Links Extension
-BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
-CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
-SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
-INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
-CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
-ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-POSSIBILITY OF SUCH DAMAGE.
+Python-Markdown Github-Links Extension is Copyright (c) 2017-2018 by Waylan
+Limberg. All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+*   Redistributions of source code must retain the above copyright
+    notice, this list of conditions and the following disclaimer.
+*   Redistributions in binary form must reproduce the above copyright
+    notice, this list of conditions and the following disclaimer in the
+    documentation and/or other materials provided with the distribution.
+*   Neither the name of HTMLTree nor the names of its contributors may be
+    used to endorse or promote products derived from this software without
+    specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY WAYLAN LIMBERG ''AS IS'' AND ANY
+EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL ANY CONTRIBUTORS TO Github-Links Extension
+BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `mdx_gh_links-0.3/README.md` & `mdx_gh_links-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,155 +1,159 @@
-# Python-Markdown Github-Links Extension
-
-An extension to Python-Markdown which adds support for shorthand links to GitHub
-users, repositories, issues and commits.
-
-## Installation
-
-To install the extension run the following command:
-
-```sh
-pip install mdx-gh-links
-```
-
-## Usage
-
-To use the extension simply include its name in the list of extensions passed to
-Python-Markdown.
-
-```python
-import markdown
-markdown.markdown(src, extensions=['mdx_gh_links'])
-```
-
-### Configuration Options
-
-To set configuration options, you may pass them to Markdown's `exension_configs`
-keyword...
-
-```python
-markdown.markdown(
-    src,
-    extensions=['mdx_gh_links'],
-    extension_configs={
-        'mdx_gh_links': {'user': 'foo', 'repo': 'bar'}
-    }
-)
-```
-
-... or you may import and pass the configs directly to an instance of the
-`mdx_gh_links.GithubLinks` class...
-
-```python
-from mdx_gh_links import GithubLinks
-markdown.markdown(src, extensions=[GithubLinks(user='foo', repo='bar')])
-```
-
-The following configuration options are available:
-
-#### user
-
-A GitHub user name or organization. If no user or organization is specified in
-a GitHub link, then the value of this option will be used.
-
-#### repo
-
-A GitHub repository. If no repository is specified in a GitHub link, then the
-value of this option will be used.
-
-## Syntax
-
-This extension implements shorthand to specify links to GitHub in various ways.
-
-All links in the generated HTML are assigned a `gh-link` class as well as a class
-unique to that type of link. See each type for the specific class assigned.
-
-### Mentions
-
-Link directly to a GitHub user, organization or repository. Note that no
-verification is made that an actual user, organization or repository exists. As
-the syntax does not differentiate between users and organizations, all
-organizations are assumed to be users. However, this assumption is only
-reflected in the title of a link.
-
-Mentions use the format `@{user}` to link to a user or organization and
-`@{user}/{repo}` to link to a repository. The defaults defined in the
-configuration options are ignored by mentions. A mention may be escaped by
-adding a backslash immediately before the at sign (`@`).
-
-All mentions are assigned the `gh-mention` class.
-
-The following table provides some examples:
-
-| shorthand   | href                         | rendered result                                                                     |
-| ----------- | ---------------------------- | -------------------------------------------------------------------- |
-| `@foo`      | `https://github.com/foo`     | [@foo](https://github.com/foo "GitHub User: @foo")                   |
-| `@foo/bar`  | `https://github.com/foo/bar` | [@foo/bar](https://github.com/foo/bar "GitHub Repository: @foo/bar") |
-| `\@foo`     |                              | @foo                                                                 |
-| `\@foo/bar` |                              | @foo/bar                                                             |
-
-### Issues
-
-Link directly to a GitHub issue or pull request (PR). Note that no verification
-is made that an actual issue or PR exists. As the syntax does not differentiate
-between Issues and PRs, all URLs point to "issues". Fortunately, GitHub will
-properly redirect an issue URL to a PR URL if appropriate.
-
-Issue links use the format `#{num}` or `{user}/{repo}#{num}`. `{num}` is the
-number assigned to the issue or PR. `{user}` and `{repo}` will use the
-defaults defined in the configuration options if not provided. An issue link may
-be escaped by adding a backslash immediately before the hash mark (`#`).
-
-All issue links are assigned the `gh-issue` class.
-
-The following table provides various examples (with the defaults set as
-`user='user', repo='repo'`):
-
-| shorthand      | href                                         | rendered result                                                                     |
-| -------------- | -------------------------------------------- | ----------------------------------------------------------------------------------- |
-| `#123`         | `https://github.com/user/repo/issues/123`    | [#123](https://github.com/user/repo/issues/123 "GitHub Issue user/repo #123")       |
-| `foo/bar#123`  | `https://github.com/foo/bar/issues/123`      | [foo/bar#123](https://github.com/foo/bar/issues/123 "GitHub Issue foo/bar #123")    |
-| `\#123`        |                                              | #123                                                                                |
-| `foo/bar\#123` |                                              | foo/bar#123                                                                         |
-
-### Commits
-
-Link directly to a GitHub Commit. Note that no verification is made that an
-actual commit exists.
-
-Commit links consist of a complete 40 character SHA hash and may optionally be
-prefaced by `{user}@` or `{user/repo}@`. `{user}` and `{repo}` will use the
-defaults defined in the configuration options if not provided. To avoid a 40
-character hash from being linked, wrap it in a code span.
-
-All commit links are assigned the `gh-commit` class.
-
-The following table provides various examples (with the defaults set as
-`user='user', repo='repo'`):
-
-| shorthand                                          | href                                                                              | rendered result                                                                                                                                                 |
-| -------------------------------------------------- | --------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `72df691791fb36f00cf5363fefe757c8d3042656`         | `https://github.com/user/repo/commit/72df691791fb36f00cf5363fefe757c8d3042656`    | [72df691](https://github.com/user/repo/commit/72df691791fb36f00cf5363fefe757c8d3042656 "GitHub Commit: user/repo@72df691791fb36f00cf5363fefe757c8d3042656")     |
-| `foo@72df691791fb36f00cf5363fefe757c8d3042656`     | `https://github.com/foo/repo/commit/72df691791fb36f00cf5363fefe757c8d3042656`     | [foo@72df691](https://github.com/foo/repo/commit/72df691791fb36f00cf5363fefe757c8d3042656 "GitHub Commit: foo/repo@72df691791fb36f00cf5363fefe757c8d3042656")   |
-| `foo/bar@72df691791fb36f00cf5363fefe757c8d3042656` | `https://github.com/foo/bar/commit/72df691791fb36f00cf5363fefe757c8d3042656`      | [foo/bar@72df691](https://github.com/foo/bar/commit/72df691791fb36f00cf5363fefe757c8d3042656 "GitHub Commit: foo/bar@72df691791fb36f00cf5363fefe757c8d3042656") |
-| `` `72df691791fb36f00cf5363fefe757c8d3042656` ``   |                                                                                   | `72df691791fb36f00cf5363fefe757c8d3042656`                                                                                                                      |
-
-## License
-
-The Python-Markdown Github-Links Extension is licensed under the [BSD License] as
-defined in `LICENSE`.
-
-[BSD License]: http://opensource.org/licenses/BSD-3-Clause
-
-## Change Log
-
-### Version 0.3 (2022/07/18)
-
-Update dependencies.
-
-### Version 0.2 (2018/03/09)
-
-Ignore mentions/issues/commits within Markdown links.
-
-### Version 0.1 (2017/11/10)
-
-The initial release.
+# Python-Markdown Github-Links Extension
+
+An extension to Python-Markdown which adds support for shorthand links to GitHub
+users, repositories, issues and commits.
+
+## Installation
+
+To install the extension run the following command:
+
+```sh
+pip install mdx-gh-links
+```
+
+## Usage
+
+To use the extension simply include its name in the list of extensions passed to
+Python-Markdown.
+
+```python
+import markdown
+markdown.markdown(src, extensions=['mdx_gh_links'])
+```
+
+### Configuration Options
+
+To set configuration options, you may pass them to Markdown's `exension_configs`
+keyword...
+
+```python
+markdown.markdown(
+    src,
+    extensions=['mdx_gh_links'],
+    extension_configs={
+        'mdx_gh_links': {'user': 'foo', 'repo': 'bar'}
+    }
+)
+```
+
+... or you may import and pass the configs directly to an instance of the
+`mdx_gh_links.GithubLinks` class...
+
+```python
+from mdx_gh_links import GithubLinks
+markdown.markdown(src, extensions=[GithubLinks(user='foo', repo='bar')])
+```
+
+The following configuration options are available:
+
+#### user
+
+A GitHub user name or organization. If no user or organization is specified in
+a GitHub link, then the value of this option will be used.
+
+#### repo
+
+A GitHub repository. If no repository is specified in a GitHub link, then the
+value of this option will be used.
+
+## Syntax
+
+This extension implements shorthand to specify links to GitHub in various ways.
+
+All links in the generated HTML are assigned a `gh-link` class as well as a class
+unique to that type of link. See each type for the specific class assigned.
+
+### Mentions
+
+Link directly to a GitHub user, organization or repository. Note that no
+verification is made that an actual user, organization or repository exists. As
+the syntax does not differentiate between users and organizations, all
+organizations are assumed to be users. However, this assumption is only
+reflected in the title of a link.
+
+Mentions use the format `@{user}` to link to a user or organization and
+`@{user}/{repo}` to link to a repository. The defaults defined in the
+configuration options are ignored by mentions. A mention may be escaped by
+adding a backslash immediately before the at sign (`@`).
+
+All mentions are assigned the `gh-mention` class.
+
+The following table provides some examples:
+
+| shorthand   | href                         | rendered result                                                                     |
+| ----------- | ---------------------------- | -------------------------------------------------------------------- |
+| `@foo`      | `https://github.com/foo`     | [@foo](https://github.com/foo "GitHub User: @foo")                   |
+| `@foo/bar`  | `https://github.com/foo/bar` | [@foo/bar](https://github.com/foo/bar "GitHub Repository: @foo/bar") |
+| `\@foo`     |                              | @foo                                                                 |
+| `\@foo/bar` |                              | @foo/bar                                                             |
+
+### Issues
+
+Link directly to a GitHub issue or pull request (PR). Note that no verification
+is made that an actual issue or PR exists. As the syntax does not differentiate
+between Issues and PRs, all URLs point to "issues". Fortunately, GitHub will
+properly redirect an issue URL to a PR URL if appropriate.
+
+Issue links use the format `#{num}` or `{user}/{repo}#{num}`. `{num}` is the
+number assigned to the issue or PR. `{user}` and `{repo}` will use the
+defaults defined in the configuration options if not provided. An issue link may
+be escaped by adding a backslash immediately before the hash mark (`#`).
+
+All issue links are assigned the `gh-issue` class.
+
+The following table provides various examples (with the defaults set as
+`user='user', repo='repo'`):
+
+| shorthand      | href                                         | rendered result                                                                     |
+| -------------- | -------------------------------------------- | ----------------------------------------------------------------------------------- |
+| `#123`         | `https://github.com/user/repo/issues/123`    | [#123](https://github.com/user/repo/issues/123 "GitHub Issue user/repo #123")       |
+| `foo/bar#123`  | `https://github.com/foo/bar/issues/123`      | [foo/bar#123](https://github.com/foo/bar/issues/123 "GitHub Issue foo/bar #123")    |
+| `\#123`        |                                              | #123                                                                                |
+| `foo/bar\#123` |                                              | foo/bar#123                                                                         |
+
+### Commits
+
+Link directly to a GitHub Commit. Note that no verification is made that an
+actual commit exists.
+
+Commit links consist of a complete 40 character SHA hash and may optionally be
+prefaced by `{user}@` or `{user/repo}@`. `{user}` and `{repo}` will use the
+defaults defined in the configuration options if not provided. To avoid a 40
+character hash from being linked, wrap it in a code span.
+
+All commit links are assigned the `gh-commit` class.
+
+The following table provides various examples (with the defaults set as
+`user='user', repo='repo'`):
+
+| shorthand                                          | href                                                                              | rendered result                                                                                                                                                 |
+| -------------------------------------------------- | --------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `72df691791fb36f00cf5363fefe757c8d3042656`         | `https://github.com/user/repo/commit/72df691791fb36f00cf5363fefe757c8d3042656`    | [72df691](https://github.com/user/repo/commit/72df691791fb36f00cf5363fefe757c8d3042656 "GitHub Commit: user/repo@72df691791fb36f00cf5363fefe757c8d3042656")     |
+| `foo@72df691791fb36f00cf5363fefe757c8d3042656`     | `https://github.com/foo/repo/commit/72df691791fb36f00cf5363fefe757c8d3042656`     | [foo@72df691](https://github.com/foo/repo/commit/72df691791fb36f00cf5363fefe757c8d3042656 "GitHub Commit: foo/repo@72df691791fb36f00cf5363fefe757c8d3042656")   |
+| `foo/bar@72df691791fb36f00cf5363fefe757c8d3042656` | `https://github.com/foo/bar/commit/72df691791fb36f00cf5363fefe757c8d3042656`      | [foo/bar@72df691](https://github.com/foo/bar/commit/72df691791fb36f00cf5363fefe757c8d3042656 "GitHub Commit: foo/bar@72df691791fb36f00cf5363fefe757c8d3042656") |
+| `` `72df691791fb36f00cf5363fefe757c8d3042656` ``   |                                                                                   | `72df691791fb36f00cf5363fefe757c8d3042656`                                                                                                                      |
+
+## License
+
+The Python-Markdown Github-Links Extension is licensed under the [BSD License] as
+defined in `LICENSE`.
+
+[BSD License]: http://opensource.org/licenses/BSD-3-Clause
+
+## Change Log
+
+### Version 0.3.1 (2023/07/28)
+
+Include README in release.
+
+### Version 0.3 (2022/07/18)
+
+Update dependencies.
+
+### Version 0.2 (2018/03/09)
+
+Ignore mentions/issues/commits within Markdown links.
+
+### Version 0.1 (2017/11/10)
+
+The initial release.
```

### Comparing `mdx_gh_links-0.3/mdx_gh_links.py` & `mdx_gh_links-0.3.1/mdx_gh_links.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-"""
-Github Links - A Python-Markdown Extension.
-
-BSD License
-
-Copyright (c) 2017-2018 by Waylan Limberg. All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-*   Redistributions of source code must retain the above copyright
-    notice, this list of conditions and the following disclaimer.
-*   Redistributions in binary form must reproduce the above copyright
-    notice, this list of conditions and the following disclaimer in the
-    documentation and/or other materials provided with the distribution.
-*   Neither the name of HTMLTree nor the names of its contributors may be
-    used to endorse or promote products derived from this software without
-    specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY WAYLAN LIMBERG ''AS IS'' AND ANY
-EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL ANY CONTRIBUTORS TO Github-Links Extension
-BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
-CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
-SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
-INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
-CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
-ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-POSSIBILITY OF SUCH DAMAGE.
-"""
-
-from markdown.extensions import Extension
-from markdown.inlinepatterns import Pattern
-from xml.etree import ElementTree
-
-
-URL_BASE = 'https://github.com'
-RE_PARTS = dict(
-    USER=r'[-_\w]{1,39}\b',
-    REPO=r'[-_.\w]+\b'
-)
-
-
-def _build_link(label, title, href, classes):
-    el = ElementTree.Element('a')
-    el.text = label
-    el.set('title', title)
-    el.set('href', href)
-    el.set('class', classes)
-    return el
-
-
-class MentionPattern(Pattern):
-    ANCESTOR_EXCLUDES = ('a',)
-
-    def __init__(self, config, md):
-        MENTION_RE = r'(@({USER})(?:\/({REPO}))?)'.format(**RE_PARTS)
-        super(MentionPattern, self).__init__(MENTION_RE, md)
-        self.config = config
-
-    def handleMatch(self, m):
-        label = m.group(2)
-        user = m.group(3)
-        repo = m.group(4)
-        if repo:
-            title = 'GitHub Repository: @{0}/{1}'.format(user, repo)
-            href = '{0}/{1}/{2}'.format(URL_BASE, user, repo)
-        else:
-            title = 'GitHub User: @{0}'.format(user)
-            href = '{0}/{1}'.format(URL_BASE, user)
-        return _build_link(label, title, href, 'gh-link gh-mention')
-
-
-class IssuePattern(Pattern):
-    ANCESTOR_EXCLUDES = ('a',)
-
-    def __init__(self, config, md):
-        ISSUE_RE = r'((?:({USER})\/({REPO}))?#([0-9]+))'.format(**RE_PARTS)
-        super(IssuePattern, self).__init__(ISSUE_RE, md)
-        self.config = config
-
-    def handleMatch(self, m):
-        label = m.group(2)
-        user = m.group(3) or self.config['user']
-        repo = m.group(4) or self.config['repo']
-        num = m.group(5).lstrip('0')
-        title = 'GitHub Issue {0}/{1} #{2}'.format(user, repo, num)
-        href = '{0}/{1}/{2}/issues/{3}'.format(URL_BASE, user, repo, num)
-        return _build_link(label, title, href, 'gh-link gh-issue')
-
-
-class CommitPattern(Pattern):
-    ANCESTOR_EXCLUDES = ('a',)
-
-    def __init__(self, config, md):
-        COMMIT_RE = r'((?:({USER})(?:\/({REPO}))?@|\b)([a-f0-9]{{40}})\b)'.format(**RE_PARTS)
-        super(CommitPattern, self).__init__(COMMIT_RE, md)
-        self.config = config
-
-    def handleMatch(self, m):
-        user = m.group(3)
-        repo = m.group(4) or self.config['repo']
-        commit = m.group(5)
-        short = commit[:7]
-        if user:
-            label = '{0}@{1}'.format(m.group(2).split('@')[0], short)
-        else:
-            label = short
-            user = self.config['user']
-        title = 'GitHub Commit: {0}/{1}@{2}'.format(user, repo, commit)
-        href = '{0}/{1}/{2}/commit/{3}'.format(URL_BASE, user, repo, commit)
-        return _build_link(label, title, href, 'gh-link gh-commit')
-
-
-class GithubLinks(Extension):
-    def __init__(self, *args, **kwargs):
-        self.config = {
-            'user': ['', 'GitHub user or organization.'],
-            'repo': ['', 'Repository name.']
-        }
-        super(GithubLinks, self).__init__(*args, **kwargs)
-
-    def extendMarkdown(self, md):
-        md.ESCAPED_CHARS.append('@')
-        md.inlinePatterns.register(IssuePattern(self.getConfigs(), md), 'issue', 20)
-        md.inlinePatterns.register(MentionPattern(self.getConfigs(), md), 'mention', 20)
-        md.inlinePatterns.register(CommitPattern(self.getConfigs(), md), 'commit', 20)
-
-
-def makeExtension(*args, **kwargs):  # pragma: no cover
-    return GithubLinks(*args, **kwargs)
+"""
+Github Links - A Python-Markdown Extension.
+
+BSD License
+
+Copyright (c) 2017-2018 by Waylan Limberg. All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+*   Redistributions of source code must retain the above copyright
+    notice, this list of conditions and the following disclaimer.
+*   Redistributions in binary form must reproduce the above copyright
+    notice, this list of conditions and the following disclaimer in the
+    documentation and/or other materials provided with the distribution.
+*   Neither the name of HTMLTree nor the names of its contributors may be
+    used to endorse or promote products derived from this software without
+    specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY WAYLAN LIMBERG ''AS IS'' AND ANY
+EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL ANY CONTRIBUTORS TO Github-Links Extension
+BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+POSSIBILITY OF SUCH DAMAGE.
+"""
+
+from markdown.extensions import Extension
+from markdown.inlinepatterns import Pattern
+from xml.etree import ElementTree
+
+
+URL_BASE = 'https://github.com'
+RE_PARTS = dict(
+    USER=r'[-_\w]{1,39}\b',
+    REPO=r'[-_.\w]+\b'
+)
+
+
+def _build_link(label, title, href, classes):
+    el = ElementTree.Element('a')
+    el.text = label
+    el.set('title', title)
+    el.set('href', href)
+    el.set('class', classes)
+    return el
+
+
+class MentionPattern(Pattern):
+    ANCESTOR_EXCLUDES = ('a',)
+
+    def __init__(self, config, md):
+        MENTION_RE = r'(@({USER})(?:\/({REPO}))?)'.format(**RE_PARTS)
+        super(MentionPattern, self).__init__(MENTION_RE, md)
+        self.config = config
+
+    def handleMatch(self, m):
+        label = m.group(2)
+        user = m.group(3)
+        repo = m.group(4)
+        if repo:
+            title = 'GitHub Repository: @{0}/{1}'.format(user, repo)
+            href = '{0}/{1}/{2}'.format(URL_BASE, user, repo)
+        else:
+            title = 'GitHub User: @{0}'.format(user)
+            href = '{0}/{1}'.format(URL_BASE, user)
+        return _build_link(label, title, href, 'gh-link gh-mention')
+
+
+class IssuePattern(Pattern):
+    ANCESTOR_EXCLUDES = ('a',)
+
+    def __init__(self, config, md):
+        ISSUE_RE = r'((?:({USER})\/({REPO}))?#([0-9]+))'.format(**RE_PARTS)
+        super(IssuePattern, self).__init__(ISSUE_RE, md)
+        self.config = config
+
+    def handleMatch(self, m):
+        label = m.group(2)
+        user = m.group(3) or self.config['user']
+        repo = m.group(4) or self.config['repo']
+        num = m.group(5).lstrip('0')
+        title = 'GitHub Issue {0}/{1} #{2}'.format(user, repo, num)
+        href = '{0}/{1}/{2}/issues/{3}'.format(URL_BASE, user, repo, num)
+        return _build_link(label, title, href, 'gh-link gh-issue')
+
+
+class CommitPattern(Pattern):
+    ANCESTOR_EXCLUDES = ('a',)
+
+    def __init__(self, config, md):
+        COMMIT_RE = r'((?:({USER})(?:\/({REPO}))?@|\b)([a-f0-9]{{40}})\b)'.format(**RE_PARTS)
+        super(CommitPattern, self).__init__(COMMIT_RE, md)
+        self.config = config
+
+    def handleMatch(self, m):
+        user = m.group(3)
+        repo = m.group(4) or self.config['repo']
+        commit = m.group(5)
+        short = commit[:7]
+        if user:
+            label = '{0}@{1}'.format(m.group(2).split('@')[0], short)
+        else:
+            label = short
+            user = self.config['user']
+        title = 'GitHub Commit: {0}/{1}@{2}'.format(user, repo, commit)
+        href = '{0}/{1}/{2}/commit/{3}'.format(URL_BASE, user, repo, commit)
+        return _build_link(label, title, href, 'gh-link gh-commit')
+
+
+class GithubLinks(Extension):
+    def __init__(self, *args, **kwargs):
+        self.config = {
+            'user': ['', 'GitHub user or organization.'],
+            'repo': ['', 'Repository name.']
+        }
+        super(GithubLinks, self).__init__(*args, **kwargs)
+
+    def extendMarkdown(self, md):
+        md.ESCAPED_CHARS.append('@')
+        md.inlinePatterns.register(IssuePattern(self.getConfigs(), md), 'issue', 20)
+        md.inlinePatterns.register(MentionPattern(self.getConfigs(), md), 'mention', 20)
+        md.inlinePatterns.register(CommitPattern(self.getConfigs(), md), 'commit', 20)
+
+
+def makeExtension(*args, **kwargs):  # pragma: no cover
+    return GithubLinks(*args, **kwargs)
```

