# Comparing `tmp/dronefly_core-0.3.6.dev6.tar.gz` & `tmp/dronefly_core-0.3.6.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dronefly_core-0.3.6.dev6.tar", max compression
+gzip compressed data, was "dronefly_core-0.3.6.dev7.tar", max compression
```

## Comparing `dronefly_core-0.3.6.dev6.tar` & `dronefly_core-0.3.6.dev7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    56815 2023-04-16 13:37:18.956988 dronefly_core-0.3.6.dev6/LICENSE
--rw-r--r--   0        0        0      702 2023-01-28 19:16:26.368426 dronefly_core-0.3.6.dev6/README.md
--rw-r--r--   0        0        0       53 2023-01-29 15:27:41.654095 dronefly_core-0.3.6.dev6/dronefly/core/__init__.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev6/dronefly/core/clients/__init__.py
--rw-r--r--   0        0        0     1028 2023-03-13 15:05:57.725989 dronefly_core-0.3.6.dev6/dronefly/core/clients/inat.py
--rw-r--r--   0        0        0     9888 2023-06-25 13:22:40.463140 dronefly_core-0.3.6.dev6/dronefly/core/commands/__init__.py
--rw-r--r--   0        0        0      635 2023-03-19 08:14:11.111276 dronefly_core-0.3.6.dev6/dronefly/core/constants.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev6/dronefly/core/formatters/__init__.py
--rw-r--r--   0        0        0      445 2023-04-16 10:53:39.829302 dronefly_core-0.3.6.dev6/dronefly/core/formatters/constants.py
--rw-r--r--   0        0        0    37682 2023-06-25 13:22:17.490660 dronefly_core-0.3.6.dev6/dronefly/core/formatters/generic.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.624333 dronefly_core-0.3.6.dev6/dronefly/core/models/__init__.py
--rw-r--r--   0        0        0     1753 2023-04-09 09:38:32.529718 dronefly_core-0.3.6.dev6/dronefly/core/models/controlled_terms.py
--rw-r--r--   0        0        0      188 2023-03-13 15:15:33.501579 dronefly_core-0.3.6.dev6/dronefly/core/models/user.py
--rw-r--r--   0        0        0       49 2023-01-29 15:28:49.919496 dronefly_core-0.3.6.dev6/dronefly/core/parsers/__init__.py
--rw-r--r--   0        0        0     3721 2023-06-14 15:48:19.092273 dronefly_core-0.3.6.dev6/dronefly/core/parsers/constants.py
--rw-r--r--   0        0        0     9291 2023-02-18 13:51:02.476816 dronefly_core-0.3.6.dev6/dronefly/core/parsers/natural.py
--rw-r--r--   0        0        0     6329 2023-03-19 08:21:31.268129 dronefly_core-0.3.6.dev6/dronefly/core/parsers/unixlike.py
--rw-r--r--   0        0        0     2346 2023-01-29 15:35:29.175688 dronefly_core-0.3.6.dev6/dronefly/core/parsers/url.py
--rw-r--r--   0        0        0       51 2023-01-29 15:27:27.497804 dronefly_core-0.3.6.dev6/dronefly/core/query/__init__.py
--rw-r--r--   0        0        0    21941 2023-06-18 15:05:34.396886 dronefly_core-0.3.6.dev6/dronefly/core/query/query.py
--rw-r--r--   0        0        0     1366 2023-06-18 14:57:16.774410 dronefly_core-0.3.6.dev6/dronefly/core/utils/__init__.py
--rw-r--r--   0        0        0      741 2023-06-25 13:23:17.247908 dronefly_core-0.3.6.dev6/pyproject.toml
--rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev6/setup.py
--rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev6/PKG-INFO
+-rw-r--r--   0        0        0    56815 2023-04-16 13:37:18.956988 dronefly_core-0.3.6.dev7/LICENSE
+-rw-r--r--   0        0        0      702 2023-01-28 19:16:26.368426 dronefly_core-0.3.6.dev7/README.md
+-rw-r--r--   0        0        0       53 2023-01-29 15:27:41.654095 dronefly_core-0.3.6.dev7/dronefly/core/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev7/dronefly/core/clients/__init__.py
+-rw-r--r--   0        0        0     1028 2023-03-13 15:05:57.725989 dronefly_core-0.3.6.dev7/dronefly/core/clients/inat.py
+-rw-r--r--   0        0        0    10512 2023-07-28 21:03:19.134549 dronefly_core-0.3.6.dev7/dronefly/core/commands/__init__.py
+-rw-r--r--   0        0        0      630 2023-07-28 21:03:19.134549 dronefly_core-0.3.6.dev7/dronefly/core/constants.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev7/dronefly/core/formatters/__init__.py
+-rw-r--r--   0        0        0      445 2023-04-16 10:53:39.829302 dronefly_core-0.3.6.dev7/dronefly/core/formatters/constants.py
+-rw-r--r--   0        0        0    45805 2023-07-28 21:03:19.138549 dronefly_core-0.3.6.dev7/dronefly/core/formatters/generic.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.624333 dronefly_core-0.3.6.dev7/dronefly/core/models/__init__.py
+-rw-r--r--   0        0        0     1753 2023-04-09 09:38:32.529718 dronefly_core-0.3.6.dev7/dronefly/core/models/controlled_terms.py
+-rw-r--r--   0        0        0      188 2023-03-13 15:15:33.501579 dronefly_core-0.3.6.dev7/dronefly/core/models/user.py
+-rw-r--r--   0        0        0       49 2023-01-29 15:28:49.919496 dronefly_core-0.3.6.dev7/dronefly/core/parsers/__init__.py
+-rw-r--r--   0        0        0     3721 2023-06-14 15:48:19.092273 dronefly_core-0.3.6.dev7/dronefly/core/parsers/constants.py
+-rw-r--r--   0        0        0     9291 2023-02-18 13:51:02.476816 dronefly_core-0.3.6.dev7/dronefly/core/parsers/natural.py
+-rw-r--r--   0        0        0     6329 2023-03-19 08:21:31.268129 dronefly_core-0.3.6.dev7/dronefly/core/parsers/unixlike.py
+-rw-r--r--   0        0        0     2346 2023-01-29 15:35:29.175688 dronefly_core-0.3.6.dev7/dronefly/core/parsers/url.py
+-rw-r--r--   0        0        0       51 2023-01-29 15:27:27.497804 dronefly_core-0.3.6.dev7/dronefly/core/query/__init__.py
+-rw-r--r--   0        0        0    21941 2023-06-18 15:05:34.396886 dronefly_core-0.3.6.dev7/dronefly/core/query/query.py
+-rw-r--r--   0        0        0     1366 2023-06-18 14:57:16.774410 dronefly_core-0.3.6.dev7/dronefly/core/utils/__init__.py
+-rw-r--r--   0        0        0      720 2023-07-28 21:08:13.132486 dronefly_core-0.3.6.dev7/pyproject.toml
+-rw-r--r--   0        0        0     1575 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev7/setup.py
+-rw-r--r--   0        0        0     1457 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev7/PKG-INFO
```

### Comparing `dronefly_core-0.3.6.dev6/LICENSE` & `dronefly_core-0.3.6.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev6/README.md` & `dronefly_core-0.3.6.dev7/README.md`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev6/dronefly/core/clients/inat.py` & `dronefly_core-0.3.6.dev7/dronefly/core/clients/inat.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev6/dronefly/core/commands/__init__.py` & `dronefly_core-0.3.6.dev7/dronefly/core/commands/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     # - Every command providing paged results must:
     #   - Set page_formatter to the formatter for the new results.
     #   - Set page to the initial page number (default: 0).
     # - Therefore, only a single command providing paged results can
     #   be active at a time.
     page_formatter: Union[BaseFormatter, ListFormatter] = None
     page: int = 0
+    per_page: int = 0
 
     def get_inat_user_default(self, inat_param: str):
         """Return iNat API default for user param default, if any, otherwise global default."""
         if inat_param not in INAT_USER_DEFAULT_PARAMS:
             return None
         if self.author:
             default = getattr(self.author, inat_param, None) or INAT_DEFAULTS.get(
@@ -84,19 +85,27 @@
     inat_client: iNatClient = iNatClient()
     parser: NaturalParser = NaturalParser()
     format: Format = Format.discord_markdown
 
     def _parse(self, query_str):
         return self.parser.parse(query_str)
 
-    def _format_markdown(self, formatter, page: int = 0):
+    def _get_formatted_page(self, formatter, page: int = 0):
         if getattr(formatter, "format_page", None):
             markdown_text = formatter.format_page(page)
+            last_page = formatter.last_page()
+            if last_page > 0:
+                markdown_text = "\n\n".join(
+                    [markdown_text, f"Page {page + 1}/{last_page + 1}"]
+                )
         else:
             markdown_text = formatter.format()
+        return self._format_markdown(markdown_text)
+
+    def _format_markdown(self, markdown_text: str):
         if self.format == Format.rich:
             # Richify the markdown:
             # - In Discord markdown, all newlines are rendered as line breaks
             # - In Rich:
             #   - Before every newline, emit " \" to force a line break, except
             #     for these exceptions to handle blockquotes:
             #     - Don't do this for a line preceding a blockquote
@@ -117,15 +126,15 @@
             # Return the literal markdown for Discord to render
             response = markdown_text
         return response
 
     def life(self, ctx: Context, *args):
         _args = " ".join(args) or "by me"
         query = self._parse(_args)
-        per_rank = query.per or "leaf"
+        per_rank = query.per or "main"
         if per_rank not in [*RANK_KEYWORDS, "leaf", "main", "any"]:
             return "Specify `per <rank-or-keyword>`"
 
         query_args = get_base_query_args(query)
         with self.inat_client.set_ctx(ctx) as client:
             # Handle a useful subset of query args in a simplistic way for now
             # (i.e. no config table lookup yet) to model full query in bot
@@ -150,48 +159,54 @@
             query_response = QueryResponse(**query_args)
             obs_args = query_response.obs_args()
             life_list = client.observations.life_list(**obs_args)
 
         if not life_list:
             return f"No life list {query_response.obs_query_description()}"
 
+        per_page = ctx.per_page
         formatter = LifeListFormatter(
-            life_list, per_rank, query_response, with_taxa=True, per_page=20
+            life_list, per_rank, query_response, with_indent=True, per_page=per_page
         )
         ctx.page_formatter = formatter
         ctx.page = 0
-        return self._format_markdown(formatter)
+        title = formatter.format_title()
+        first_page = formatter.get_first_page() or ""
+        if first_page:
+            first_page = "\n".join([title, "", first_page])
+            formatter.pages[0] = first_page
+        return self._get_formatted_page(formatter, 0)
 
     def next(self, ctx: Context):
         if not ctx.page_formatter:
             return "Type a command that has pages first"
         ctx.page += 1
         if ctx.page > ctx.page_formatter.last_page():
             ctx.page = 0
-        return self._format_markdown(ctx.page_formatter, ctx.page)
+        return self._get_formatted_page(ctx.page_formatter, ctx.page)
 
     def page(self, ctx: Context, page: int = 1):
         if not ctx.page_formatter:
             return "Type a command that has pages first"
         last_page = ctx.page_formatter.last_page() + 1
         if page > last_page or page < 1:
             msg = "Specify page 1"
             if last_page > 1:
                 msg += f" through {last_page}"
             return msg
         ctx.page = page - 1
-        return self._format_markdown(ctx.page_formatter, ctx.page)
+        return self._get_formatted_page(ctx.page_formatter, ctx.page)
 
     def prev(self, ctx: Context):
         if not ctx.page_formatter:
             return "Type a command that has pages first"
         ctx.page -= 1
         if ctx.page < 0:
             ctx.page = ctx.page_formatter.last_page()
-        return self._format_markdown(ctx.page_formatter, ctx.page)
+        return self._get_formatted_page(ctx.page_formatter, ctx.page)
 
     def taxon(self, ctx: Context, *args):
         query = self._parse(" ".join(args))
         # TODO: Handle all query clauses, not just main.terms
         # TODO: Doesn't do any ranking or filtering of results
         if not query.main or not query.main.terms:
             return "Not a taxon"
@@ -204,15 +219,15 @@
             taxon = client.taxa.populate(taxon)
 
         formatter = TaxonFormatter(
             taxon,
             lang=ctx.get_inat_user_default("inat_lang"),
             with_url=True,
         )
-        response = self._format_markdown(formatter)
+        response = self._get_formatted_page(formatter)
 
         return response
 
     def obs(self, ctx: Context, *args):
         query = self._parse(" ".join(args))
         # TODO: Handle all query clauses, not just main.terms
         # TODO: Doesn't do any ranking or filtering of results
@@ -248,10 +263,10 @@
         formatter = ObservationFormatter(
             obs,
             taxon_summary=taxon_summary,
             community_taxon=community_taxon,
             community_taxon_summary=community_taxon_summary,
             with_link=True,
         )
-        response = self._format_markdown(formatter)
+        response = self._get_formatted_page(formatter)
 
         return response
```

### Comparing `dronefly_core-0.3.6.dev6/dronefly/core/constants.py` & `dronefly_core-0.3.6.dev7/dronefly/core/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 INAT_USER_DEFAULTS = {"locale": None, "preferred_place_id": 1}
 # All defaults:
 INAT_DEFAULTS = {**INAT_USER_DEFAULTS, "all_names": True}
 
 PLANTAE_ID = 47126
 TRACHEOPHYTA_ID = 211194
 RANK_KEYWORDS = tuple(RANK_LEVELS.keys()) + tuple(RANK_EQUIVALENTS.keys())
-TAXON_PRIMARY_RANKS = COMMON_RANKS[-5:]
+TAXON_PRIMARY_RANKS = COMMON_RANKS
 TRINOMIAL_ABBR = {"variety": "var.", "subspecies": "ssp.", "form": "f."}
```

### Comparing `dronefly_core-0.3.6.dev6/dronefly/core/formatters/generic.py` & `dronefly_core-0.3.6.dev7/dronefly/core/formatters/generic.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,22 +16,23 @@
 import html2markdown
 import inflect
 from pyinaturalist import (
     ConservationStatus,
     EstablishmentMeans,
     JsonResponse,
     LifeList,
-    LifeListTaxon,
     ListedTaxon,
     Observation,
     Taxon,
+    TaxonCount,
     TaxonSummary,
     User,
 )
-from pyinaturalist.constants import COMMON_RANKS
+from pyinaturalist.models.taxon import make_tree
+from pyinaturalist.constants import COMMON_RANKS, ROOT_TAXON_ID
 
 from dronefly.core.constants import (
     TAXON_PRIMARY_RANKS,
     TRINOMIAL_ABBR,
     RANK_EQUIVALENTS,
     RANK_LEVELS,
 )
@@ -74,14 +75,18 @@
 
 p = inflect.engine()
 p.defnoun("phylum", "phyla")
 p.defnoun("subphylum", "subphyla")
 p.defnoun("subgenus", "subgenera")
 
 
+def protect_leading_blanks(text: str = ""):
+    return re.sub(r"^( +)", "\N{ZERO WIDTH SPACE}" + r"**\1**", text)
+
+
 def escape_markdown(
     text: str, *, as_needed: bool = False, ignore_links: bool = True
 ) -> str:
     r"""A helper function that escapes Discord's markdown.
 
     Parameters
     -----------
@@ -121,14 +126,43 @@
             regex = f"(?:{_URL_REGEX}|{regex})"
         return re.sub(regex, replacement, text, 0, re.MULTILINE)
     else:
         text = re.sub(r"\\", r"\\\\", text)
         return _MARKDOWN_ESCAPE_REGEX.sub(r"\\\1", text)
 
 
+def taxa_per_rank(
+    life_list: LifeList,
+    ranks_to_count: Union(list[str], str),
+    root_taxon_id: int = None,
+):
+    """Generate taxa matching ranks to count in treewise order."""
+    options = {}
+    subtree = (
+        lambda t: True
+        if root_taxon_id is None
+        else root_taxon_id in [t.id] + [a.id for a in t.ancestors]
+    )
+    if isinstance(ranks_to_count, list):
+        options["include_ranks"] = ranks_to_count
+        include = lambda t: subtree(t)  # noqa: E731
+    else:
+        if ranks_to_count == "leaf":
+            include = (
+                lambda t: subtree(t) and t.count == t.descendant_obs_count
+            )  # noqa: E731
+        else:
+            options["include_ranks"] = [ranks_to_count]
+            include = lambda t: subtree(t) and t.rank == ranks_to_count  # noqa: E731
+    tree = make_tree(life_list.data, **options)
+    for taxon_count in tree.flatten(hide_root=tree.id == ROOT_TAXON_ID):
+        if include(taxon_count):
+            yield taxon_count
+
+
 def format_datetime(time, compact=False):
     """Format datetime with compact option that drops less relevant parts."""
     hour = time.strftime("%I").lstrip("0")
     minute = time.strftime("%M")
     am_pm = time.strftime("%p").lower()
     day = time.strftime("%d").lstrip("0")
     mon = time.strftime("%b")
@@ -142,65 +176,82 @@
             formatted_time = f"{mon}-{year}"
     else:
         wday = time.strftime("%a")
         formatted_time = f"{wday} {mon} {day}, {year} · {hour}:{minute} {am_pm}"
     return formatted_time
 
 
-def filter_life_list(life_list: LifeList, per_rank: str, taxon: Taxon):
+def included_ranks(per_rank):
+    if per_rank == "main":
+        ranks = COMMON_RANKS
+    else:
+        ranks = list(RANK_LEVELS.keys())
+    return ranks
+
+
+def filter_life_list(
+    life_list: LifeList, per_rank: str, taxon: Taxon, root_taxon_id: int = None
+):
     ranks = None
     rank_totals = {}
-    if per_rank in ["main", "any"]:
-        ranks_to_count = (
-            COMMON_RANKS[-8:] if per_rank == "main" else list(RANK_LEVELS.keys())
-        )
+    if per_rank in ("main", "any"):
+        ranks_to_count = included_ranks(per_rank)
         if taxon:
             if per_rank == "main" and taxon.rank not in ranks_to_count:
                 rank_level = RANK_LEVELS[taxon.rank]
                 ranks_to_count = [
                     rank for rank in ranks_to_count if RANK_LEVELS[rank] < rank_level
                 ]
                 ranks_to_count.append(taxon.rank)
             else:
                 ranks_to_count = ranks_to_count[: ranks_to_count.index(taxon.rank) + 1]
         ranks = "main ranks" if per_rank == "main" else "ranks"
-        taxa = [
-            life_list_taxon
-            for life_list_taxon in life_list.data
-            if life_list_taxon.rank in ranks_to_count
-        ]
-        tot = {}
-        for taxon in taxa:
-            rank = taxon.rank
-            tot[rank] = tot.get(taxon.rank, 0) + 1
-        max_digits = len(str(max(tot.values())))
-        rank_totals = {
-            rank: f"`{str(tot[rank]).rjust(max_digits)}` {p.plural_noun(rank, tot[rank])}"
-            for rank in tot
-        }
+        generate_taxa = taxa_per_rank(life_list, ranks_to_count, root_taxon_id)
     elif per_rank == "leaf":
         ranks = "leaf taxa"
-        taxa = [
-            life_list_taxon
-            for life_list_taxon in life_list.data
-            if life_list_taxon.direct_obs_count == life_list_taxon.descendant_obs_count
-        ]
+        generate_taxa = taxa_per_rank(life_list, per_rank, root_taxon_id)
     else:
         rank = RANK_EQUIVALENTS[per_rank] if per_rank in RANK_EQUIVALENTS else per_rank
         ranks = p.plural_noun(rank)
-        taxa = [
-            life_list_taxon
-            for life_list_taxon in life_list.data
-            if life_list_taxon.rank == rank
-        ]
-    return (taxa, ranks, rank_totals)
+        generate_taxa = taxa_per_rank(life_list, per_rank, root_taxon_id)
+    counted_taxa = []
+    counted_taxon_ids = []
+    tot = {}
+    max_taxon_count_digits = 1
+    max_direct_count_digits = 1
+    for taxon_count in generate_taxa:
+        counted_taxon_ids.append(taxon_count.id)
+        taxon_count_digits = len(str(taxon_count.descendant_obs_count))
+        if taxon_count_digits > max_taxon_count_digits:
+            max_taxon_count_digits = taxon_count_digits
+        direct_count_digits = len(str(taxon_count.count))
+        if direct_count_digits > max_direct_count_digits:
+            max_direct_count_digits = direct_count_digits
+        counted_taxa.append(taxon_count)
+        rank = taxon_count.rank
+        tot[rank] = tot.get(taxon_count.rank, 0) + 1
+    max_rank_digits = len(str(max(tot.values()))) if tot else 1
+    rank_totals = {
+        rank: f"`{str(tot[rank]).rjust(max_rank_digits)}` {p.plural_noun(rank, tot[rank])}"
+        for rank in tot
+    }
+    if per_rank == "leaf":
+        counted_taxa.sort(key=lambda t: t.name)
+    return (
+        counted_taxa,
+        counted_taxon_ids,
+        ranks,
+        rank_totals,
+        max_taxon_count_digits,
+        max_direct_count_digits,
+    )
 
 
 def format_life_list_summary(
-    taxa: list[LifeListTaxon], ranks: str, rank_totals: list[int]
+    taxa: list[TaxonCount], ranks: str, rank_totals: list[int]
 ):
     total = f"Total: {len(taxa)} {ranks}"
     if rank_totals:
         rank_keys = reversed(
             [rank for rank in RANK_LEVELS.keys() if rank != "stateofmatter"]
         )
         rank_totals_by_rank = [
@@ -436,15 +487,15 @@
         - italicize the name (minus any rank abbreviations; see next point) for genus
         level and lower
         - for trinomials (must be subspecies level & have exactly 3 names to qualify),
         insert the appropriate abbreviation, unitalicized, between the 2nd and 3rd
         name (e.g. "Anser anser domesticus" -> "*Anser anser* var. *domesticus*")
     """
 
-    if with_common:
+    def get_common_name():
         preferred_common_name = None
         if lang and taxon.names:
             name = next(
                 iter([name for name in taxon.names if name.get("locale") == lang]), None
             )
             if name:
                 preferred_common_name = name.get("name")
@@ -457,22 +508,28 @@
                 else preferred_common_name
             )
         else:
             if hierarchy:
                 common = None
             else:
                 common = preferred_common_name
-    else:
-        common = None
+        return common
+
+    common = get_common_name() if with_common else None
     name = taxon.name
 
     rank = taxon.rank
     rank_level = RANK_LEVELS[rank]
 
-    if rank_level <= RANK_LEVELS["genus"]:
+    # Note: We follow how iNat uses italics taxon names on the website, i.e. we:
+    # - don't apply italics to the name when it is rank Genushybrid or Subgenus
+    # - do italicize the name for Genus and every rank at species or below
+    # - any abbreviated english keywords within italicized intraspecific ranks
+    #   are not italicized (spp. var. f.)
+    if rank == "genus" or rank_level <= RANK_LEVELS["species"]:
         name = f"*{name}*"
     if rank_level > RANK_LEVELS["species"]:
         if hierarchy:
             bold = ("\n> **", "**") if rank in TAXON_PRIMARY_RANKS else ("", "")
             name = f"{bold[0]}{name}{bold[1]}"
         elif with_rank:
             name = f"{rank.capitalize()} {name}"
@@ -552,16 +609,20 @@
 class LifeListFormatter(ListFormatter):
     def __init__(
         self,
         life_list: LifeList,
         per_rank: str,
         query_response: QueryResponse,
         with_url: bool = True,
-        with_taxa: bool = False,
+        with_taxa: bool = True,
+        with_indent: bool = False,
+        with_direct: bool = False,
+        with_common: bool = False,
         per_page: int = 20,
+        root_taxon_id: int = None,
     ):
         """
         Parameters
         ----------
         life_list: LifeList
             Life list of all taxa matching the observations query in
             query_response.
@@ -586,29 +647,58 @@
 
             The first page links to the observations in the query
             and the last page ends with a total per rank in the query.
 
             When False, only page 0 can be formatted with the observations link
             and per rank summary alone.
 
+        with_indent: bool, optional
+            When with_indent is True, per_rank is 'main' or 'any', and with_taxa
+            is also True, the taxon names on the life list are displayed as
+            children of higher taxa on the same page using indent levels and "└"
+            to indicate child relationships.
+
+        with_direct: bool, optional
+            When with_direct is True, a column of direct observations counts of
+            each taxon is shown. The number is only shown when non-zero. If the
+            direct obs count is equal to the total obs count, then the total obs
+            count is omitted. When shown, the direct obs count is enclosed in
+            parentheses.
+
+        with_common: bool, optional
+            When with_common is True, if the life_list contains common names, then
+            common names are included in the output.
+
         per_page: int, optional
             The number of taxa to include in each page.
+
+        root_taxon_id: int, optional
+            If specified, make the taxon with this ID the root. The taxon with
+            this ID must be in the life list data.
         """
         self.life_list = life_list
         self.per_rank = per_rank
         self.query_response = query_response
         self.with_url = with_url
         self.with_taxa = with_taxa
-        self.per_page = per_page
-        (taxa, self.ranks, self.rank_totals) = filter_life_list(
-            self.life_list, self.per_rank, self.query_response.taxon
-        )
-        self.taxa = list(taxa)
-        self.max_digits = len(
-            str(max([taxon.descendant_obs_count for taxon in self.taxa]))
+        self.with_indent = with_indent
+        self.with_direct = with_direct
+        self.with_common = with_common
+        self.pages = []
+        self.per_page = per_page if per_page >= 0 else 0
+        self.root_taxon_id = root_taxon_id
+        (
+            self.taxa,
+            self.taxon_ids,
+            self.ranks,
+            self.rank_totals,
+            self.count_digits,
+            self.direct_digits,
+        ) = filter_life_list(
+            self.life_list, self.per_rank, self.query_response.taxon, self.root_taxon_id
         )
 
     def format(self, with_title: bool = True, page: int = 0):
         """Format the life list as markdown."""
         description = self.format_page(page)
         if with_title:
             description = "\n\n".join([self.format_title(), description])
@@ -631,59 +721,159 @@
             if self.query_response.user:
                 url = lifelists_url_from_query_response(self.query_response)
                 title = format_link(title, url)
         return title
 
     def format_page(self, page: int = 0):
         """Format the life list description."""
-        description = []
-        query_response = self.query_response
-        if page == 0:
-            obs_link = format_link(
-                "All Life List Observations",
-                obs_url_from_v1(query_response.obs_args()),
+
+        def indent_level(taxon: Taxon):
+            if self.per_rank not in ("main", "any"):
+                return 0
+            root_indent_level = self.taxa[0].indent_level
+            return taxon.indent_level - root_indent_level
+
+        def indent_child(taxon: Taxon):
+            level = indent_level(taxon)
+            return protect_leading_blanks(
+                "\N{EN SPACE}\N{THIN SPACE}" * (level - 1) + "└\N{THIN SPACE}"
+                if level >= 1
+                else ""
             )
-            description.append(obs_link)
-        # TODO: if more than max_taxa, support paged result
-        if self.taxa and self.with_taxa:
-            page_start = page * self.per_page
-            page_end = page_start + self.per_page
-            page_of_taxa = self.taxa[page_start:page_end]
+
+        def make_page_header(taxon: Taxon):
+            """Make a page header for non-top-level taxa."""
+            ancestors = taxon.ancestors
+            if ancestors:
+                if ancestors[0].id == ROOT_TAXON_ID:
+                    del ancestors[0]
+                if ancestors:
+                    header_ranks = included_ranks(self.per_rank)
+                    header_names = [
+                        format_taxon_name(parent, with_rank=False)
+                        for parent in ancestors
+                        if parent.rank in header_ranks
+                    ]
+                    if header_names:
+                        counts_width = self.count_digits
+                        if self.with_direct:
+                            counts_width += self.direct_digits + 2
+                        return (
+                            f"`{' ' * counts_width}` __"
+                            + " > ".join(header_names)
+                            + "__"
+                        )
+            return None
+
+        def format_page_of_taxa(page_of_taxa):
+            query_response = self.query_response
             formatted_taxa = []
-            obs_args = query_response.obs_args()
             for taxon in page_of_taxa:
-                # Replace any taxa in the original query with just the one:
-                if "taxon_ids" in obs_args:
-                    del obs_args["taxon_ids"]
-                taxon_obs_url = obs_url_from_v1(
-                    {
-                        **obs_args,
-                        "taxon_id": taxon.id,
-                    }
+                formatted_count = str(taxon.descendant_obs_count).rjust(
+                    self.count_digits
+                )
+                formatted_direct = ""
+                # Format the direct column similarly to Dynamic Life Lists on
+                # iNat web, i.e.
+                # - never show direct count on non-leaves when it is zero
+                # - only show one column at the leaves, as the counts are equal
+                # - show the leaf count as "direct" at ranks above species,
+                #   a cue that the species count might be improved with more
+                #   ID refinements
+                if self.with_direct:
+                    formatted_direct = " " * (self.direct_digits + 2)
+                    if taxon.count > 0:
+                        formatted_direct = f"({taxon.count})".rjust(
+                            self.direct_digits + 2
+                        )
+                        is_leaf = taxon.count == taxon.descendant_obs_count
+                        terminal_rank = taxon.rank_level <= RANK_LEVELS["species"]
+                        if is_leaf:
+                            if terminal_rank:
+                                formatted_direct = " " * (self.direct_digits + 2)
+                            else:
+                                formatted_count = " " * self.count_digits
+                taxon_name = format_taxon_name(taxon, with_common=False)
+                formatted_name = format_link(
+                    taxon_name, taxon_obs_url(query_response, taxon)
                 )
-                formatted_count = str(taxon.descendant_obs_count).rjust(self.max_digits)
-                formatted_name = format_link(taxon.name, taxon_obs_url)
-                formatted_taxa.append(f"`{formatted_count}` {formatted_name}")
-            description.append("\n".join(formatted_taxa))
-        if page == self.last_page():
-            life_list_summary = format_life_list_summary(
-                self.taxa, self.ranks, self.rank_totals
+                if self.with_common and taxon.preferred_common_name:
+                    formatted_name = f"{formatted_name} ({taxon.preferred_common_name})"
+                formatted_taxa.append(
+                    f"`{formatted_count}{formatted_direct}` {indent_child(taxon)}{formatted_name}"
+                )
+            return formatted_taxa
+
+        def make_page(page):
+            sections = []
+            query_response = self.query_response
+            with_page_headers = self.per_rank in ("main", "any")
+            if page == 0:
+                obs_link = format_link(
+                    "Observations",
+                    obs_url_from_v1(query_response.obs_args()),
+                )
+                sections.append(obs_link)
+            if self.taxa and self.with_taxa:
+                page_of_taxa = self.get_page_of_taxa(page)
+                if page_of_taxa:
+                    formatted_taxa = format_page_of_taxa(page_of_taxa)
+                    if with_page_headers and indent_level(page_of_taxa[0]) > 1:
+                        formatted_taxa.insert(0, make_page_header(page_of_taxa[0]))
+                    sections.append("\n".join(formatted_taxa))
+            if page == self.last_page():
+                life_list_summary = format_life_list_summary(
+                    self.taxa, self.ranks, self.rank_totals
+                )
+                sections.append(life_list_summary)
+            return "\n\n".join(sections)
+
+        def taxon_obs_url(query_response, taxon):
+            obs_args = query_response.obs_args()
+            # Replace multiple taxa in the original query with just the one:
+            if "taxon_ids" in obs_args:
+                del obs_args["taxon_ids"]
+            return obs_url_from_v1(
+                {
+                    **obs_args,
+                    "taxon_id": taxon.id,
+                }
             )
-            description.append(life_list_summary)
-        return "\n\n".join(description)
 
-    def format_all(self):
-        return [self.format_page(page) for page in range(0, self.last_page() + 1)]
+        last_cached_page = len(self.pages) - 1
+        # Extend page cache with new formatted pages up to and including
+        # requested page. Normally the user advances a page at a time, so this
+        # formats and caches new pages efficiently for for the normal case,
+        # while still supporting random access.
+        for new_page in range(last_cached_page + 1, page + 1):
+            self.pages.append(make_page(new_page))
+        return self.pages[page]
+
+    def generate_pages(self):
+        for page in range(0, self.last_page() + 1):
+            formatted_page = self.format_page(page)
+            yield formatted_page
+
+    def get_first_page(self):
+        first_page = self.format_page(0)
+        return first_page
+
+    def get_page_of_taxa(self, page: int):
+        if self.per_page > 0:
+            page_start = page * self.per_page
+            page_end = page_start + self.per_page
+        else:
+            page_start = 0
+            page_end = len(self.taxa) + 1
+        return self.taxa[page_start:page_end]
 
     def last_page(self):
-        return (
-            ceil(len(self.taxa) / self.per_page) - 1
-            if self.with_taxa and self.taxa
-            else 0
-        )
+        if not (self.with_taxa and self.per_page > 0 and self.taxa):
+            return 0
+        return ceil(len(self.taxa) / self.per_page) - 1
 
 
 class TaxonFormatter(BaseFormatter):
     def __init__(
         self,
         taxon: Taxon,
         lang: str = None,
```

### Comparing `dronefly_core-0.3.6.dev6/dronefly/core/models/controlled_terms.py` & `dronefly_core-0.3.6.dev7/dronefly/core/models/controlled_terms.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev6/dronefly/core/parsers/constants.py` & `dronefly_core-0.3.6.dev7/dronefly/core/parsers/constants.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev6/dronefly/core/parsers/natural.py` & `dronefly_core-0.3.6.dev7/dronefly/core/parsers/natural.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev6/dronefly/core/parsers/unixlike.py` & `dronefly_core-0.3.6.dev7/dronefly/core/parsers/unixlike.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev6/dronefly/core/parsers/url.py` & `dronefly_core-0.3.6.dev7/dronefly/core/parsers/url.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev6/dronefly/core/query/query.py` & `dronefly_core-0.3.6.dev7/dronefly/core/query/query.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev6/dronefly/core/utils/__init__.py` & `dronefly_core-0.3.6.dev7/dronefly/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev6/setup.py` & `dronefly_core-0.3.6.dev7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,24 +11,23 @@
  'core.query',
  'core.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['attrs>=21.2',
- 'dateparser>=1.1.1,<2.0.0',
+['dateparser>=1.1.1,<2.0.0',
  'html2markdown>=0.1.7,<0.2.0',
  'inflect>=5.3.0,<6.0.0',
- 'pyinaturalist>=0.19.0.dev2,<0.20',
- 'rich>=10.9,<14']
+ 'pyinaturalist>=0.19.0.dev3,<0.20',
+ 'rich==13.4.2']
 
 setup_kwargs = {
     'name': 'dronefly-core',
-    'version': '0.3.6.dev6',
+    'version': '0.3.6.dev7',
     'description': 'Core dronefly components',
     'long_description': "# Dronefly core\n\nThis is an incomplete rewrite of [Dronefly](https://dronefly.readthedocs.io)\nDiscord bot's core components. We're not yet making version guarantees until\nit is more usable.\n\n# Related packages\n\n## Dronefly command-line client\n\nThe [dronefly-cli](https://github.com/dronefly-garden/dronefly-cli) command-line\nclient will provide a standalone text user interface that can perform a usable\nsubset of Dronefly Discord bot's capabilities, built solely with Dronefly core.\n\n## Dronefly Discord bot\n\nDronefly Discord bot brings [iNaturalist](https://www.inaturalist.org) taxa,\nobservations, and other data from the site into conversations on the\n[Discord](https://discord.com) chat platform.\n",
     'author': 'Ben Armstrong',
     'author_email': 'synrg@debian.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dronefly_core-0.3.6.dev6/PKG-INFO` & `dronefly_core-0.3.6.dev7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: dronefly-core
-Version: 0.3.6.dev6
+Version: 0.3.6.dev7
 Summary: Core dronefly components
 License: AGPL-3.0-or-later
 Author: Ben Armstrong
 Author-email: synrg@debian.org
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: attrs (>=21.2)
 Requires-Dist: dateparser (>=1.1.1,<2.0.0)
 Requires-Dist: html2markdown (>=0.1.7,<0.2.0)
 Requires-Dist: inflect (>=5.3.0,<6.0.0)
-Requires-Dist: pyinaturalist (>=0.19.0.dev2,<0.20)
-Requires-Dist: rich (>=10.9,<14)
+Requires-Dist: pyinaturalist (>=0.19.0.dev3,<0.20)
+Requires-Dist: rich (==13.4.2)
 Description-Content-Type: text/markdown
 
 # Dronefly core
 
 This is an incomplete rewrite of [Dronefly](https://dronefly.readthedocs.io)
 Discord bot's core components. We're not yet making version guarantees until
 it is more usable.
```

