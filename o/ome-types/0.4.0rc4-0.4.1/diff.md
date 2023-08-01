# Comparing `tmp/ome_types-0.4.0rc4.tar.gz` & `tmp/ome_types-0.4.1.tar.gz`

## Comparing `ome_types-0.4.0rc4.tar` & `ome_types-0.4.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    23306 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_autogen/__init__.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_autogen/__main__.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_autogen/_config.py
--rw-r--r--   0        0        0    11409 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_autogen/_generator.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_autogen/_transformer.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_autogen/_util.py
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_autogen/main.py
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_autogen/templates/class.jinja2
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_autogen/templates/docstrings.numpy.jinja2
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_autogen/templates/enum.jinja2
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/__init__.py
--rw-r--r--   0        0        0    19822 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_conversion.py
--rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_pydantic_compat.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/etree_fixes.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/napari.yaml
--rw-r--r--   0        0        0   285655 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/ome-2016-06.xsd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/py.typed
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/units.py
--rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/widget.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_mixins/__init__.py
--rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_mixins/_base_type.py
--rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_mixins/_ids.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_mixins/_instrument.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_mixins/_kinded.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_mixins/_ome.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_mixins/_reference.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_mixins/_util.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_mixins/_validators.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_vendor/__init__.py
--rw-r--r--   0        0        0    16940 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_vendor/_pydantic_color_v1.py
--rw-r--r--   0        0        0    21521 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_vendor/_pydantic_color_v2.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/model/__init__.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/model/_color.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/model/_converters.py
--rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/model/_shape_union.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/model/_structured_annotations.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/model/_user_sequence.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/model/simple_types.py
--rw-r--r--   0        0        0    51712 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2003-FC-to-2008-09.xsl
--rw-r--r--   0        0        0    33502 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2007-06-to-2008-09.xsl
--rw-r--r--   0        0        0    31797 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2008-02-to-2008-09.xsl
--rw-r--r--   0        0        0    67202 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2008-09-to-2009-09.xsl
--rw-r--r--   0        0        0    18678 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2009-09-to-2010-04.xsl
--rw-r--r--   0        0        0    10744 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2010-04-to-2010-06.xsl
--rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2010-06-to-2011-06.xsl
--rw-r--r--   0        0        0    21773 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2011-06-to-2012-06.xsl
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2012-06-to-2013-06.xsl
--rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2013-06-to-2015-01.xsl
--rw-r--r--   0        0        0     9282 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2015-01-to-2016-06.xsl
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/__init__.py
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/bindings.py
--rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/compat.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/config.py
--rw-r--r--   0        0        0     4581 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/py.typed
--rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/pydantic_compat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/hooks/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/hooks/class_type.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/hooks/cli.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/LICENSE
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/README.md
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/hatch_build.py
--rw-r--r--   0        0        0     6397 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/pyproject.toml
--rw-r--r--   0        0        0    10335 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/PKG-INFO
+-rw-r--r--   0        0        0    23797 2020-02-02 00:00:00.000000 ome_types-0.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_autogen/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_autogen/__main__.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_autogen/_config.py
+-rw-r--r--   0        0        0    11409 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_autogen/_generator.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_autogen/_transformer.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_autogen/_util.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_autogen/main.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_autogen/templates/class.jinja2
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_autogen/templates/docstrings.numpy.jinja2
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_autogen/templates/enum.jinja2
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/__init__.py
+-rw-r--r--   0        0        0    19822 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/_conversion.py
+-rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/_pydantic_compat.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/etree_fixes.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/napari.yaml
+-rw-r--r--   0        0        0   285655 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/ome-2016-06.xsd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/py.typed
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/units.py
+-rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/widget.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/_mixins/__init__.py
+-rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/_mixins/_base_type.py
+-rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/_mixins/_ids.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/_mixins/_instrument.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/_mixins/_kinded.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/_mixins/_ome.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/_mixins/_reference.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/_mixins/_util.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/_mixins/_validators.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/_vendor/__init__.py
+-rw-r--r--   0        0        0    16940 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/_vendor/_pydantic_color_v1.py
+-rw-r--r--   0        0        0    21521 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/_vendor/_pydantic_color_v2.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/model/__init__.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/model/_color.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/model/_converters.py
+-rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/model/_shape_union.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/model/_structured_annotations.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/model/_user_sequence.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/model/simple_types.py
+-rw-r--r--   0        0        0    51712 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/transforms/2003-FC-to-2008-09.xsl
+-rw-r--r--   0        0        0    33502 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/transforms/2007-06-to-2008-09.xsl
+-rw-r--r--   0        0        0    31797 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/transforms/2008-02-to-2008-09.xsl
+-rw-r--r--   0        0        0    67202 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/transforms/2008-09-to-2009-09.xsl
+-rw-r--r--   0        0        0    18678 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/transforms/2009-09-to-2010-04.xsl
+-rw-r--r--   0        0        0    10744 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/transforms/2010-04-to-2010-06.xsl
+-rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/transforms/2010-06-to-2011-06.xsl
+-rw-r--r--   0        0        0    21773 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/transforms/2011-06-to-2012-06.xsl
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/transforms/2012-06-to-2013-06.xsl
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/transforms/2013-06-to-2015-01.xsl
+-rw-r--r--   0        0        0     9282 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/ome_types/transforms/2015-01-to-2016-06.xsl
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/xsdata_pydantic_basemodel/__init__.py
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/xsdata_pydantic_basemodel/bindings.py
+-rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/xsdata_pydantic_basemodel/compat.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/xsdata_pydantic_basemodel/config.py
+-rw-r--r--   0        0        0     4581 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/xsdata_pydantic_basemodel/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/xsdata_pydantic_basemodel/py.typed
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/xsdata_pydantic_basemodel/pydantic_compat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/xsdata_pydantic_basemodel/hooks/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/xsdata_pydantic_basemodel/hooks/class_type.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 ome_types-0.4.1/src/xsdata_pydantic_basemodel/hooks/cli.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 ome_types-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ome_types-0.4.1/LICENSE
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 ome_types-0.4.1/README.md
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ome_types-0.4.1/hatch_build.py
+-rw-r--r--   0        0        0     6397 2020-02-02 00:00:00.000000 ome_types-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    10332 2020-02-02 00:00:00.000000 ome_types-0.4.1/PKG-INFO
```

### Comparing `ome_types-0.4.0rc4/CHANGELOG.md` & `ome_types-0.4.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,28 @@
 # Changelog
 
+## [v0.4.1](https://github.com/tlambert03/ome-types/tree/v0.4.1) (2023-08-01)
+
+[Full Changelog](https://github.com/tlambert03/ome-types/compare/v0.4.0...v0.4.1)
+
+**Merged pull requests:**
+
+- fix: remove print [\#211](https://github.com/tlambert03/ome-types/pull/211) ([tlambert03](https://github.com/tlambert03))
+
 ## [v0.4.0](https://github.com/tlambert03/ome-types/tree/v0.4.0) (2023-07-16)
 
-[Full Changelog](https://github.com/tlambert03/ome-types/compare/v0.4.0rc3...v0.4.0)
+[Full Changelog](https://github.com/tlambert03/ome-types/compare/v0.4.0rc4...v0.4.0)
+
+**Merged pull requests:**
+
+- fix: update stacklevel for deprecation warning [\#210](https://github.com/tlambert03/ome-types/pull/210) ([tlambert03](https://github.com/tlambert03))
+
+## [v0.4.0rc4](https://github.com/tlambert03/ome-types/tree/v0.4.0rc4) (2023-07-16)
+
+[Full Changelog](https://github.com/tlambert03/ome-types/compare/v0.4.0rc3...v0.4.0rc4)
 
 **Implemented enhancements:**
 
 - feat: catch and fix lowercase 'ome' in schemas [\#209](https://github.com/tlambert03/ome-types/pull/209) ([tlambert03](https://github.com/tlambert03))
 - feat: add transformations to from\_xml [\#208](https://github.com/tlambert03/ome-types/pull/208) ([tlambert03](https://github.com/tlambert03))
 
 ## [v0.4.0rc3](https://github.com/tlambert03/ome-types/tree/v0.4.0rc3) (2023-07-14)
@@ -110,24 +126,20 @@
 
 **Tests & CI:**
 
 - test: add more tests [\#177](https://github.com/tlambert03/ome-types/pull/177) ([tlambert03](https://github.com/tlambert03))
 
 ## [v0.4.0a1](https://github.com/tlambert03/ome-types/tree/v0.4.0a1) (2023-07-02)
 
-[Full Changelog](https://github.com/tlambert03/ome-types/compare/ruff-panic...v0.4.0a1)
+[Full Changelog](https://github.com/tlambert03/ome-types/compare/v0.3.4...v0.4.0a1)
 
 **Merged pull requests:**
 
 - ci\(pre-commit.ci\): autoupdate [\#172](https://github.com/tlambert03/ome-types/pull/172) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
 
-## [ruff-panic](https://github.com/tlambert03/ome-types/tree/ruff-panic) (2023-06-20)
-
-[Full Changelog](https://github.com/tlambert03/ome-types/compare/v0.3.4...ruff-panic)
-
 ## [v0.3.4](https://github.com/tlambert03/ome-types/tree/v0.3.4) (2023-04-06)
 
 [Full Changelog](https://github.com/tlambert03/ome-types/compare/v0.3.3...v0.3.4)
 
 **Implemented enhancements:**
 
 - feat: make lxml optional \(but don't yet remove from requirements\) [\#166](https://github.com/tlambert03/ome-types/pull/166) ([tlambert03](https://github.com/tlambert03))
```

### Comparing `ome_types-0.4.0rc4/src/ome_autogen/_config.py` & `ome_types-0.4.1/src/ome_autogen/_config.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_autogen/_generator.py` & `ome_types-0.4.1/src/ome_autogen/_generator.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_autogen/_transformer.py` & `ome_types-0.4.1/src/ome_autogen/_transformer.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_autogen/_util.py` & `ome_types-0.4.1/src/ome_autogen/_util.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_autogen/main.py` & `ome_types-0.4.1/src/ome_autogen/main.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_autogen/templates/class.jinja2` & `ome_types-0.4.1/src/ome_autogen/templates/class.jinja2`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_autogen/templates/enum.jinja2` & `ome_types-0.4.1/src/ome_autogen/templates/enum.jinja2`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/__init__.py` & `ome_types-0.4.1/src/ome_types/__init__.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/_conversion.py` & `ome_types-0.4.1/src/ome_types/_conversion.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/_pydantic_compat.py` & `ome_types-0.4.1/src/ome_types/_pydantic_compat.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/etree_fixes.py` & `ome_types-0.4.1/src/ome_types/etree_fixes.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/ome-2016-06.xsd` & `ome_types-0.4.1/src/ome_types/ome-2016-06.xsd`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/units.py` & `ome_types-0.4.1/src/ome_types/units.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/widget.py` & `ome_types-0.4.1/src/ome_types/widget.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/_mixins/_base_type.py` & `ome_types-0.4.1/src/ome_types/_mixins/_base_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         _move_deprecated_fields(data, field_names)
         super().__init__(**data)
         kwargs = set(data.keys())
         extra = kwargs - field_names
         if extra and warn_extra:
             warnings.warn(
                 f"Unrecognized fields for type {type(self)}: {kwargs - field_names}",
-                stacklevel=2,
+                stacklevel=3,
             )
 
     def __init_subclass__(cls) -> None:
         """Add `*_quantity` property for fields that have both a value and a unit.
 
         where `*_quantity` is a pint `Quantity`.
         """
```

### Comparing `ome_types-0.4.0rc4/src/ome_types/_mixins/_ids.py` & `ome_types-0.4.1/src/ome_types/_mixins/_ids.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/_mixins/_instrument.py` & `ome_types-0.4.1/src/ome_types/_mixins/_instrument.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/_mixins/_kinded.py` & `ome_types-0.4.1/src/ome_types/_mixins/_kinded.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/_mixins/_ome.py` & `ome_types-0.4.1/src/ome_types/_mixins/_ome.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/_mixins/_reference.py` & `ome_types-0.4.1/src/ome_types/_mixins/_reference.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/_mixins/_validators.py` & `ome_types-0.4.1/src/ome_types/_mixins/_validators.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/_vendor/__init__.py` & `ome_types-0.4.1/src/ome_types/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/_vendor/_pydantic_color_v1.py` & `ome_types-0.4.1/src/ome_types/_vendor/_pydantic_color_v1.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/_vendor/_pydantic_color_v2.py` & `ome_types-0.4.1/src/ome_types/_vendor/_pydantic_color_v2.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/model/__init__.py` & `ome_types-0.4.1/src/ome_types/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/model/_color.py` & `ome_types-0.4.1/src/ome_types/model/_color.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/model/_converters.py` & `ome_types-0.4.1/src/ome_types/model/_converters.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/model/_shape_union.py` & `ome_types-0.4.1/src/ome_types/model/_shape_union.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/model/_structured_annotations.py` & `ome_types-0.4.1/src/ome_types/model/_structured_annotations.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/model/_user_sequence.py` & `ome_types-0.4.1/src/ome_types/model/_user_sequence.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/model/simple_types.py` & `ome_types-0.4.1/src/ome_types/model/simple_types.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/transforms/2003-FC-to-2008-09.xsl` & `ome_types-0.4.1/src/ome_types/transforms/2003-FC-to-2008-09.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/transforms/2007-06-to-2008-09.xsl` & `ome_types-0.4.1/src/ome_types/transforms/2007-06-to-2008-09.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/transforms/2008-02-to-2008-09.xsl` & `ome_types-0.4.1/src/ome_types/transforms/2008-02-to-2008-09.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/transforms/2008-09-to-2009-09.xsl` & `ome_types-0.4.1/src/ome_types/transforms/2008-09-to-2009-09.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/transforms/2009-09-to-2010-04.xsl` & `ome_types-0.4.1/src/ome_types/transforms/2009-09-to-2010-04.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/transforms/2010-04-to-2010-06.xsl` & `ome_types-0.4.1/src/ome_types/transforms/2010-04-to-2010-06.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/transforms/2010-06-to-2011-06.xsl` & `ome_types-0.4.1/src/ome_types/transforms/2010-06-to-2011-06.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/transforms/2011-06-to-2012-06.xsl` & `ome_types-0.4.1/src/ome_types/transforms/2011-06-to-2012-06.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/transforms/2012-06-to-2013-06.xsl` & `ome_types-0.4.1/src/ome_types/transforms/2012-06-to-2013-06.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/transforms/2013-06-to-2015-01.xsl` & `ome_types-0.4.1/src/ome_types/transforms/2013-06-to-2015-01.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/ome_types/transforms/2015-01-to-2016-06.xsl` & `ome_types-0.4.1/src/ome_types/transforms/2015-01-to-2016-06.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/bindings.py` & `ome_types-0.4.1/src/xsdata_pydantic_basemodel/bindings.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/compat.py` & `ome_types-0.4.1/src/xsdata_pydantic_basemodel/compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from contextlib import suppress
 from typing import Any, Callable, Dict, Generic, List, Optional, Tuple, Type, TypeVar
 
 try:
     from lxml import etree as ET
 except ImportError:
     import xml.etree.ElementTree as ET  # type: ignore
 
@@ -145,11 +146,9 @@
         def get_core_schema(*args: Any) -> cs.PlainValidatorFunctionSchema:
             return cs.general_plain_validator_function(validator)
 
         return get_core_schema
 
     for type_, val in _validators.items():
         get_schema = _make_get_core_schema(val[0])
-        try:
+        with suppress(TypeError):
             type_.__get_pydantic_core_schema__ = get_schema  # type: ignore
-        except TypeError as e:
-            print(e)
```

### Comparing `ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/config.py` & `ome_types-0.4.1/src/xsdata_pydantic_basemodel/config.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/generator.py` & `ome_types-0.4.1/src/xsdata_pydantic_basemodel/generator.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/pydantic_compat.py` & `ome_types-0.4.1/src/xsdata_pydantic_basemodel/pydantic_compat.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/.gitignore` & `ome_types-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/LICENSE` & `ome_types-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/README.md` & `ome_types-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/pyproject.toml` & `ome_types-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc4/PKG-INFO` & `ome_types-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ome-types
-Version: 0.4.0rc4
+Version: 0.4.1
 Summary: Python dataclasses for the OME data model
 Project-URL: Source, https://github.com/tlambert03/ome-types
 Project-URL: Tracker, https://github.com/tlambert03/ome-types/issues
 Project-URL: Documentation, https://ome-types.readthedocs.io/en/latest/
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: MIT
 License-File: LICENSE
```

