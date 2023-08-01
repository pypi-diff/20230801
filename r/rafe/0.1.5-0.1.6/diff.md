# Comparing `tmp/rafe-0.1.5-py3-none-any.whl.zip` & `tmp/rafe-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,22 @@
-Zip file size: 23624 bytes, number of entries: 19
--rw-r--r--  2.0 unx       71 b- defN 23-Jul-05 19:23 rafe/__init__.py
--rw-r--r--  2.0 unx       63 b- defN 23-Jul-05 19:23 rafe/__main__.py
--rw-r--r--  2.0 unx     2415 b- defN 23-Jul-05 19:23 rafe/build.py
--rw-r--r--  2.0 unx    26009 b- defN 23-Jul-05 19:23 rafe/cfgraph.py
--rw-r--r--  2.0 unx    13854 b- defN 23-Jul-05 19:23 rafe/cli.py
--rw-r--r--  2.0 unx     9039 b- defN 23-Jul-05 19:23 rafe/cli_api.py
--rw-r--r--  2.0 unx     2639 b- defN 23-Jul-05 19:23 rafe/config.py
--rw-r--r--  2.0 unx     1286 b- defN 23-Jul-05 19:23 rafe/logger.py
--rw-r--r--  2.0 unx      302 b- defN 23-Jul-05 19:23 rafe/main.py
--rw-r--r--  2.0 unx     2068 b- defN 23-Jul-05 19:23 rafe/metadata.py
--rw-r--r--  2.0 unx     3998 b- defN 23-Jul-05 19:23 rafe/plugin.py
--rw-r--r--  2.0 unx     2217 b- defN 23-Jul-05 19:23 rafe/source.py
--rw-r--r--  2.0 unx     4044 b- defN 23-Jul-05 19:23 rafe/utils.py
--rw-r--r--  2.0 unx     1455 b- defN 23-Jul-05 19:24 rafe-0.1.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1878 b- defN 23-Jul-05 19:24 rafe-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-05 19:24 rafe-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 23-Jul-05 19:24 rafe-0.1.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-05 19:24 rafe-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1387 b- defN 23-Jul-05 19:24 rafe-0.1.5.dist-info/RECORD
-19 files, 72862 bytes uncompressed, 21422 bytes compressed:  70.6%
+Zip file size: 26964 bytes, number of entries: 20
+-rw-r--r--  2.0 unx       71 b- defN 23-Aug-01 00:04 rafe/__init__.py
+-rw-r--r--  2.0 unx       63 b- defN 23-Aug-01 00:04 rafe/__main__.py
+-rw-r--r--  2.0 unx     2394 b- defN 23-Aug-01 00:04 rafe/build.py
+-rw-r--r--  2.0 unx    26009 b- defN 23-Aug-01 00:04 rafe/cfgraph.py
+-rw-r--r--  2.0 unx    16579 b- defN 23-Aug-01 00:04 rafe/cli.py
+-rw-r--r--  2.0 unx     9014 b- defN 23-Aug-01 00:04 rafe/cli_api.py
+-rw-r--r--  2.0 unx     3316 b- defN 23-Aug-01 00:04 rafe/config.py
+-rw-r--r--  2.0 unx     6898 b- defN 23-Aug-01 00:04 rafe/griffe_util.py
+-rw-r--r--  2.0 unx     1286 b- defN 23-Aug-01 00:04 rafe/logger.py
+-rw-r--r--  2.0 unx      302 b- defN 23-Aug-01 00:04 rafe/main.py
+-rw-r--r--  2.0 unx     1958 b- defN 23-Aug-01 00:04 rafe/metadata.py
+-rw-r--r--  2.0 unx     3998 b- defN 23-Aug-01 00:04 rafe/plugin.py
+-rw-r--r--  2.0 unx     3401 b- defN 23-Aug-01 00:04 rafe/source.py
+-rw-r--r--  2.0 unx     4006 b- defN 23-Aug-01 00:04 rafe/utils.py
+-rw-r--r--  2.0 unx     1455 b- defN 23-Aug-01 00:04 rafe-0.1.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     3005 b- defN 23-Aug-01 00:04 rafe-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-01 00:04 rafe-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 23-Aug-01 00:04 rafe-0.1.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Aug-01 00:04 rafe-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1463 b- defN 23-Aug-01 00:04 rafe-0.1.6.dist-info/RECORD
+20 files, 85355 bytes uncompressed, 24648 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -15,14 +15,17 @@
 
 Filename: rafe/cli_api.py
 Comment: 
 
 Filename: rafe/config.py
 Comment: 
 
+Filename: rafe/griffe_util.py
+Comment: 
+
 Filename: rafe/logger.py
 Comment: 
 
 Filename: rafe/main.py
 Comment: 
 
 Filename: rafe/metadata.py
@@ -33,26 +36,26 @@
 
 Filename: rafe/source.py
 Comment: 
 
 Filename: rafe/utils.py
 Comment: 
 
-Filename: rafe-0.1.5.dist-info/LICENSE.txt
+Filename: rafe-0.1.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: rafe-0.1.5.dist-info/METADATA
+Filename: rafe-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: rafe-0.1.5.dist-info/WHEEL
+Filename: rafe-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: rafe-0.1.5.dist-info/entry_points.txt
+Filename: rafe-0.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: rafe-0.1.5.dist-info/top_level.txt
+Filename: rafe-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: rafe-0.1.5.dist-info/RECORD
+Filename: rafe-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rafe/__init__.py

```diff
@@ -1,3 +1,3 @@
 # rafe: Reproducible Artifacts for Environments
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
```

## rafe/build.py

```diff
@@ -22,16 +22,15 @@
 
 def build_package(recipe_dir):
     """
     Builds a package for the platform that is being used to build.
     """
 
     recipe_dir = recipe_dir.resolve()
-    source.provide(recipe_dir)
-    src_dir = source.get_dir()
+    src_dir = source.provide(recipe_dir)
 
     logger.info(
         f"""
 	Building Pacakge: {recipe_dir}
 	Source Tree: 	  {src_dir}
 	"""
     )
```

## rafe/cli.py

```diff
@@ -8,14 +8,15 @@
 from rich import print
 from rich.console import Console
 from rich.table import Table
 from rich.progress import Progress
 from rich.prompt import Prompt
 
 from rafe import __version__
+from rafe.griffe_util import check_breaks, verify_removals
 from rafe.cfgraph import CFGraph
 from rafe.build import build_package
 from rafe.config import create_app_dirs
 from rafe.logger import logger, setFileHandle
 
 from rafe.plugin import RafePluginManager
 
@@ -370,14 +371,93 @@
         table.add_row(r["name"], r["entrypoint"], r["path"])
 
     console = Console()
     console.print(table)
     return
 
 
+check_api_breaks_options = {
+    "package": typer.Option(
+        ..., "--package", help="Name of package folder name to check"
+    ),
+    "old_tag": typer.Option(..., "--old", help="First package version in comparison"),
+    "new_tag": typer.Option(..., "--new", help="Second package version in comparison"),
+    "path": typer.Option(
+        None,
+        "--path",
+        help="Path to package source. Default behavior expects folder in .rafe/work/{package}",
+    ),
+    "break_type": typer.Option(
+        None,
+        "--type",
+        help="Type of api breakage to check. Default behavior dumps all breaks.",
+    ),
+    "output": typer.Option(
+        None, "--out", help="Path for output json. Default behavior dumps to pwd."
+    ),
+}
+
+
+@app.command(rich_help_panel="API Breaks")
+def check_api_breaks(
+    package: str = check_api_breaks_options["package"],
+    old_tag: str = check_api_breaks_options["old_tag"],
+    new_tag: str = check_api_breaks_options["new_tag"],
+    path: pathlib.Path = check_api_breaks_options["path"],
+    break_type: str = check_api_breaks_options["break_type"],
+    output_path: pathlib.Path = check_api_breaks_options["output"],
+):
+    """
+    Compares two instances of the same package to check for API breaking changes between versions.
+    Default behavior is to expect you have a source copy of the package in .rafe/work/{package} with .git info
+    """
+    if path is None:
+        path = pathlib.Path.home().joinpath(".rafe", "work", package)
+
+    # could consider setting up an auto-acquire here
+    if not path.exists():
+        raise FileNotFound()
+    if output_path is None:
+        output_path = pathlib.Path.cwd()
+
+    temp = check_breaks(
+        package, old_tag, new_tag, path, break_type, output_path, logger
+    )
+
+    return
+
+
+verify_breaks_options = {
+    "package": typer.Option(
+        ...,
+        "--package",
+        help="Import name of package to check. May be different than package name.",
+    ),
+    "path": typer.Option(..., "--path", help="Path to breakage json source."),
+}
+
+
+@app.command(rich_help_panel="API Breaks")
+def verify_breaks(
+    package: str = check_api_breaks_options["package"],
+    path: pathlib.Path = check_api_breaks_options["path"],
+):
+    """
+    Assumes 'new' package version has been installed in some way and added to the pythonpath
+    The easiest route would likely be to unzip a wheel into a working folder and add that folder
+    to $PYTHONPATH. e.g. on linux: export PYTHONPATH=<local path>:$PYTHONPATH
+    """
+    if pathlib.Path(path).exists():
+        verify_removals(package, path, logger)
+    else:
+        logger.error(f"Did not find {path}.")
+
+    return
+
+
 plugin_configuration_options = {
     "add": typer.Option(
         None, "--add", help="Add a plugin given a folder", callback=callback_plugin_add
     ),
     "list": typer.Option(
         None,
         "--list",
```

## rafe/cli_api.py

```diff
@@ -203,15 +203,14 @@
             i["version"] = ""
 
         matched_package = cfgraph.match_versioned_packages(
             i["name"], i["version"], python_version_matches
         )
 
         if len(matched_package) > 0:
-            breakpoint()
             cfgraph.fetch_package_json(i["name"], matched_package[0], package_arch)
             package_report["matched_packages"].append(
                 {"name": i["name"], "version": i["version"]}
             )
             cfgraph.logger.info(
                 "[bold green] Match Found [/bold green]"
                 + f"{i['name']}=={i['version']}",
```

## rafe/config.py

```diff
@@ -49,14 +49,35 @@
             logger.warn(
                 "[bold yellow] DIRECOTRY EXISTS: [/bold yellow]" + str(folder),
                 extra={"markup": True},
             )
     return
 
 
+def create_work_subfolder(rootdir: pathlib.Path) -> None:
+    """
+    Given a root directory, create general work folder
+    """
+    folders = ["work"]
+    for sf in folders:
+        folder = rootdir.joinpath(sf)
+        if not folder.exists():
+            folder.mkdir(parents=True, exist_ok=True)
+            logger.info(
+                "[bold green] CREATE DIRECTORY: [/bold green]" + str(folder),
+                extra={"markup": True},
+            )
+        else:
+            logger.warn(
+                "[bold yellow] DIRECOTRY EXISTS: [/bold yellow]" + str(folder),
+                extra={"markup": True},
+            )
+    return
+
+
 def create_plugin_config(rootdir: pathlib.Path) -> None:
     """
     Given the root directory, create a plugin json.
     """
     plugin_configuration_json: pathlib.Path = rootdir.joinpath("plugins_conf.json")
 
     if not plugin_configuration_json.exists():
@@ -84,13 +105,14 @@
     """
     Given a root directory, create it inside the homedir and then create
     subfolders for neccesary functions.
     """
     create_rafe_rootdir(rootdir)
     create_cfcache_subfolder(rootdir)
     create_plugin_config(rootdir)
+    create_work_subfolder(rootdir)
     return 0
 
 
 root_dir = dirname(dirname(__file__))
 src_cache = join(root_dir, "src_cache")
 work_dir = join(root_dir, "work")
```

## rafe/metadata.py

```diff
@@ -74,13 +74,7 @@
 def render_recipe(recipe_dir, cfg=None):
     path = join(recipe_dir, "meta.yaml")
     if not isfile(path):
         return None
     data = open(path).read()
     meta = parse(data, cfg)
     return meta
-
-
-if __name__ == "__main__":
-    from pprint import pprint
-
-    pprint(render_recipe("../examples/bitarray"))
```

## rafe/source.py

```diff
@@ -1,57 +1,90 @@
 import os
+import pathlib
 import sys
+import git
+import shutil
 from subprocess import check_call
 from os.path import basename, join, isdir, isfile
 from urllib.parse import urlparse
 
+from rafe.logger import logger
 from rafe.utils import download, hashsum_file, rm_rf, tar_xf
 from rafe.config import work_dir, src_cache
 from rafe.metadata import render_recipe
 
 
-def get_dir():
-    lst = [fn for fn in os.listdir(work_dir) if not fn.startswith(".")]
+def get_dir(package):
+    lst = list(pathlib.Path(work_dir).glob(f'{package["name"]}-{package["version"]}*'))
     if len(lst) == 1:
         dir_path = join(work_dir, lst[0])
         if isdir(dir_path):
             return dir_path
     return work_dir
 
 
-def download_to_cache(source):
+def download_to_cache(source, package):
     if not isdir(src_cache):
+        logger.info(f"CREATE | Directory at: {src_cache}")
         os.makedirs(src_cache)
 
-    fn = basename(urlparse(source["url"]).path)
-    md5 = source.get("md5")
-    path = join(src_cache, fn)
-
-    if not isfile(path):
-        download(source["url"], path, md5)
-
-    assert isfile(path)
-    for ht in "md5", "sha1", "sha256":
-        if ht in source and hashsum_file(path, ht) != source[ht]:
-            raise Exception("%s mismatch: %r" % (ht.upper(), source))
+    filename = basename(urlparse(source["url"]).path)
+
+    if filename.endswith((".tar.gz", ".tar.bz2", ".tgz", ".tar.xz", ".tar")):
+        md5 = source.get("md5")
+        path = join(src_cache, filename)
+
+        if not isfile(path):
+            download(source["url"], path, md5)
+
+        assert isfile(path)
+
+        for ht in "md5", "sha1", "sha256":
+            if ht in source and hashsum_file(path, ht) != source[ht]:
+                raise Exception("%s mismatch: %r" % (ht.upper(), source))
+
+    else:
+        path = src_cache + f'/{package["name"]}-{package["version"]}-{source["sha"]}/'
+        if pathlib.Path(path).exists():
+            logger.info(f"Source exists at: {path}")
+            return path
+
+        logger.info(f"CLONE | Repo: {source['url']} -> {path}")
+        sha = source.get("sha")
+
+        branch = source.get("branch")
+        if branch is None:
+            branch = "main"
+
+        repo = git.Repo.clone_from(source["url"], path, branch=branch)
+        repo.commit(rev=sha)
+
     return path
 
 
-def unpack(source):
-    src_path = download_to_cache(source)
+def unpack(source, package):
+    src_path = download_to_cache(source, package)
+
+    if not pathlib.Path(work_dir).exists():
+        os.makedirs(work_dir)
 
-    os.makedirs(work_dir)
     if src_path.endswith((".tar.gz", ".tar.bz2", ".tgz", ".tar.xz", ".tar")):
+        logger.info(f"UNPACK | {src_cache} -> {work_dir}")
         tar_xf(src_path, work_dir)
-    else:
-        raise Exception("not a vaild source")
+
+    elif isdir(src_path):
+        logger.info(f"MOVE | {src_cache} -> {work_dir}")
+        new_work_dir = work_dir + "/" + pathlib.Path(src_path).name.__str__() + "/"
+        shutil.move(src_path, new_work_dir)
+
+    return src_path
 
 
 def apply_patch(src_dir, path):
-    print("Applying patch: %r" % path)
+    logger.info("Applying patch: %r" % path)
     assert isfile(path), path
     args = ["-p0", "-i", path]
     check_call(
         [
             "patch",
         ]
         + args,
@@ -66,23 +99,24 @@
     given the metadata:
       - download (if necessary)
       - unpack
       - apply patches (if any)
     """
     meta = render_recipe(recipe_dir)
     source = meta.get("source", {})
-    rm_rf(work_dir)
+    package = meta.get("package", {})
+
     if "url" in source:
-        unpack(source)
-    else:  # no source
+        source_path = unpack(source, package)
+    else:
         os.makedirs(work_dir)
 
     if "patch" in source:
-        src_dir = get_dir()
+        if not os.path.isdir(source_path):
+            source_path = get_dir(package)
         for patch in source.get("patches", []):
-            apply_patch(src_dir, recipe_dir, patch)
-
+            apply_patch(source_path, recipe_dir, patch)
 
-if __name__ == "__main__":
-    from rafe.config import recipes_dir
+    if not os.path.isdir(source_path):
+        source_path = get_dir(package)
 
-    provide(join(recipes_dir, "bitarray"))
+    return source_path
```

## rafe/utils.py

```diff
@@ -147,11 +147,7 @@
     # write to a temp file and rename afterwards
     tmp_path = path + ".tmp"
 
     with open(tmp_path, mode=mode) as fo:
         yield fo
 
     os.rename(tmp_path, path)
-
-
-if __name__ == "__main__":
-    pass
```

## Comparing `rafe-0.1.5.dist-info/LICENSE.txt` & `rafe-0.1.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `rafe-0.1.5.dist-info/RECORD` & `rafe-0.1.6.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-rafe/__init__.py,sha256=obdvdtCKFshboHg0vZumZJzdjxmTu2iEgo7KGIu1b8M,71
+rafe/__init__.py,sha256=shsR5U2V1up6Y3qXzrv2Qm1MCYq9VmppuFNjWEidmpI,71
 rafe/__main__.py,sha256=qF8ob9wqPM7eJ1JheF-fyHg39ixJiFyvLvhgBW1tbqY,63
-rafe/build.py,sha256=lIwiMq8cB6yYsn7hsZqMoM05WS0dT8NwgmBs6BYIwHk,2415
+rafe/build.py,sha256=n86nUE6qU7z6189FSx03s4p89l_c0Z_icXaxzXeTm0I,2394
 rafe/cfgraph.py,sha256=lX-9niyalbb7PUuzSMaAykZhyk5K6t2qDDZFzbYN5AM,26009
-rafe/cli.py,sha256=VG_iiYT8_puS4C8g7smHR9zfmf5d5rM7L7JOKBAEuas,13854
-rafe/cli_api.py,sha256=jq34twMfqXmGifE9p5nQNx7AGl-fMjeJUVP1O97PsEQ,9039
-rafe/config.py,sha256=Pam2-2cxGr8y-LnglnCn-5YZ95xHc8KvBeJpTzrG0yk,2639
+rafe/cli.py,sha256=i2I91Npx0fbjtZLyJYoB7D6xf5m10NQOwAXxvzmFYAc,16579
+rafe/cli_api.py,sha256=9KLVJGcmREvc32cSm0WBrOF5BJoRzzXM-lkMdeaMOh4,9014
+rafe/config.py,sha256=FtISl0PhSdFjzKTV4cFTo0-PV34fhUAB5AyiXsaXUOU,3316
+rafe/griffe_util.py,sha256=5BFwr3BhvuYbLZqi6tDC4YJat-S1G4aMt_R-FnxXhdM,6898
 rafe/logger.py,sha256=tfmaFwDnlBnXhzNZOPpScAsizcnwUtcik1fxuENN_Xs,1286
 rafe/main.py,sha256=VfruOJEUIKlKWbtuVzxiqi5yM5ePiAcqbD8ZQDAsj1M,302
-rafe/metadata.py,sha256=IzbUBadd_8WDAXcG4MCgXJAXU2C7qE0eRvcruvRU6Y4,2068
+rafe/metadata.py,sha256=VTVHjBx81gAcWIW2A5d7tYOZAgS3ddctjb7-0-CsrE8,1958
 rafe/plugin.py,sha256=3U_3mbJUkrI7jhjHB2Uro5MNdIELOypyWhM-mH7k_OU,3998
-rafe/source.py,sha256=WTpf0YE0eeIyie1gX4qfuVIl_PNSz7oRXyYsleCPd_4,2217
-rafe/utils.py,sha256=CcMijLcc6KNdA4vWlfuqFRASNvKq4vvcfg6PWkLHseY,4044
-rafe-0.1.5.dist-info/LICENSE.txt,sha256=bk8H6oMXQAcDs6uLXh0jCW-6bcz7HAvG5yO1DpA9uBA,1455
-rafe-0.1.5.dist-info/METADATA,sha256=nron6FfOZOAjSG64DnmAMQoui9LieP9hHzbxQhZTmlo,1878
-rafe-0.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rafe-0.1.5.dist-info/entry_points.txt,sha256=648OfD-f-wH9Xb2Xfwt-b-5WugCsqUsOHh2WFvWtuRA,40
-rafe-0.1.5.dist-info/top_level.txt,sha256=t4Lb6m-BEtVPU2Zx8g-0oMvlWBtYQWXQpWuHJeOkKYU,5
-rafe-0.1.5.dist-info/RECORD,,
+rafe/source.py,sha256=7NzfgNLmts2aH86jYgVrDCbBwpGcZTccrI1RActV8lg,3401
+rafe/utils.py,sha256=2y-1mh5-arbCQZ7y6CuhvKLB4tk3DAAYSYSWGe1JXTI,4006
+rafe-0.1.6.dist-info/LICENSE.txt,sha256=bk8H6oMXQAcDs6uLXh0jCW-6bcz7HAvG5yO1DpA9uBA,1455
+rafe-0.1.6.dist-info/METADATA,sha256=I3nszxfElHKxk5jetTRXql3oaSPDAvUn7KIxqxw3VDk,3005
+rafe-0.1.6.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+rafe-0.1.6.dist-info/entry_points.txt,sha256=648OfD-f-wH9Xb2Xfwt-b-5WugCsqUsOHh2WFvWtuRA,40
+rafe-0.1.6.dist-info/top_level.txt,sha256=t4Lb6m-BEtVPU2Zx8g-0oMvlWBtYQWXQpWuHJeOkKYU,5
+rafe-0.1.6.dist-info/RECORD,,
```

