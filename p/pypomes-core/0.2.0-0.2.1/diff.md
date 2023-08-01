# Comparing `tmp/pypomes_core-0.2.0.tar.gz` & `tmp/pypomes_core-0.2.1.tar.gz`

## Comparing `pypomes_core-0.2.0.tar` & `pypomes_core-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 pypomes_core-0.2.0/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes_core-0.2.0/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    27087 2020-02-02 00:00:00.000000 pypomes_core-0.2.0/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 pypomes_core-0.2.0/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes_core-0.2.0/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pypomes_core-0.2.0/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes_core-0.2.0/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes_core-0.2.0/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     7094 2020-02-02 00:00:00.000000 pypomes_core-0.2.0/src/pypomes_core/http_pomes.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 pypomes_core-0.2.0/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 pypomes_core-0.2.0/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 pypomes_core-0.2.0/src/pypomes_core/logging_pomes.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes_core-0.2.0/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0    13830 2020-02-02 00:00:00.000000 pypomes_core-0.2.0/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 pypomes_core-0.2.0/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_core-0.2.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.2.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.2.0/README.md
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pypomes_core-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 pypomes_core-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    27260 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4585 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/http_pomes.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6296 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/logging_pomes.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0    20320 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/README.md
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 pypomes_core-0.2.1/PKG-INFO
```

### Comparing `pypomes_core-0.2.0/src/pypomes_core/__init__.py` & `pypomes_core-0.2.1/src/pypomes_core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,16 @@
     # file_pomes
     file_from_request,
     # http_pomes
     MIMETYPE_BINARY, MIMETYPE_CSS, MIMETYPE_CSV, MIMETYPE_HTML, MIMETYPE_JAVASCRIPT,
     MIMETYPE_JSON, MIMETYPE_MULTIPART, MIMETYPE_PDF, MIMETYPE_PKCS7, MIMETYPE_SOAP,
     MIMETYPE_TEXT, MIMETYPE_URLENCODED, MIMETYPE_XML, MIMETYPE_ZIP,
     http_status_name, http_status_description,
-    http_json_from_form, http_json_from_request, http_json_from_get, http_json_from_post,
+    http_json_from_form, http_json_from_request,
+    http_json_from_get, http_json_from_post,
     # json_pomes
     json_normalize_dict, json_normalize_iterable,
     # list_pomes
     list_compare, list_flatten, list_unflatten,
     list_find_coupled, list_elem_starting_with, list_transform,
     # logging_pomes
     LOGGING_ID, LOGGING_LEVEL, LOGGING_FORMAT, LOGGING_STYLE,
@@ -96,9 +97,9 @@
     validate_format_error, validate_format_errors,
     # str_pomes
     str_between, str_split_on_mark, str_find_whitespace,
     # xml_pomes
     XML_FILE_HEADER, xml_to_dict, xml_normalize_keys
 ]
 
-__version__ = "0.2.0"
-__version_info__ = (0, 2, 0)
+__version__ = "0.2.1"
+__version_info__ = (0, 2, 1)
```

### Comparing `pypomes_core-0.2.0/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.2.1/src/pypomes_core/datetime_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 DATETIME_FORMAT_COMPACT: Final[str] = "%Y%m%d%H%M%S"
 DATETIME_FORMAT_INV: Final[str] = "%Y-%m-%d %H:%M:%S"
 
 
 def date_reformat(dt_str: str, to_format: str, **kwargs: any) -> str:
     """
     Convert the date in *dt_str* to the format especified in *to_format*.
+
     The argument *dt_str* must represent a valid date, with or without time-of-day information.
     The argument *to_format* must be a valid format for *date* ou *datetime*.
 
     :param dt_str: The date to convert.
     :param to_format: The format for the conversion.
     :param kwargs: Optional arguments for the parser in python-dateutil ('dayfirst' is a common argument).
     :return:  The converted date.
@@ -29,14 +30,15 @@
 
     return result
 
 
 def date_parse(dt_str: str, **kwargs: any) -> date:
     """
     Obtain and return the *date* object corresponding to *dt_str*.
+
     Return *None* se *dt_str* does not contain a valid date.
 
     :param dt_str: The date, in a supported format.
     :param kwargs: Optional arguments for the parser in python-dateutil ('dayfirst' is a common argument).
     :return: The corresponding date object, or None.
     """
     result: date | None = None
@@ -44,15 +46,16 @@
         result = parser.parse(dt_str, **kwargs).date()
 
     return result
 
 
 def datetime_parse(dt_str: str, **kwargs: any) -> datetime:
     """
-   Obtain and return the *datetime* object corresponding to *dt_str*.
+    Obtain and return the *datetime* object corresponding to *dt_str*.
+
    Return *None* se *dt_str* does not contain a valid date.
 
     :param dt_str: The date, in a supported format.
     :param kwargs: Optional arguments for the parser in python-dateutil ('dayfirst' is a common argument).
     :return: The corresponding datetime object, or None.
     """
     result: datetime | None = None
```

### Comparing `pypomes_core-0.2.0/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.2.1/src/pypomes_core/dict_pomes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import inspect
 import types
 
 
 def dict_has_key_chain(source: dict, key_chain: list[str]) -> bool:
     """
-    Indicate the existence of an element in *source* pointed to by the nested keys chain
-    *[keys[0]: ... :keys[n]*. The path up to he last key in the chain must point to an existing element.
+    Indicate the existence of an element in *source* pointed to by the nested keys chain *[keys[0]: ... :keys[n]*.
+
+    The path up to he last key in the chain must point to an existing element.
     A given key may indicate the element's position within a *list*, using the format *<key>[<pos>]*.
 
-    :param source: The reference dict.
-    :param key_chain: The nested keys chain.
-    :return: Whether the element exists.
+    :param source: the reference dict
+    :param key_chain: the nested keys chain
+    :return: whether the element exists
     """
     # initialize the return variable
     result: bool = False
 
     # define the parent el;ement
     parent: dict | None = None
 
@@ -49,123 +50,126 @@
 
     return result
 
 
 def dict_get_value(source: dict, key_chain: list[str]) -> any:
     """
     Obtain the value of the element in *source* pointed to by the nested keys chain *[keys[0]: ... :keys[n]*.
+
     The path up to the last key in the chain must point to an existing element.
     A given key may indicate the element's position within a *list*, using the format *<key>[<pos>]*.
     Return *None* if the sought after value is not found.
     Note that returning *None* might not be indicative of the absence of the element in *source*,
     since that element might exist therein with the value *None*. To determine whether this is the case,
     use the operation *dict_has_value*.
 
-    :param source: o dict de referência
-    :param key_chain: a cadeia de chaves
-    :return: o valor obtido
+    :param source: the reference dict
+    :param key_chain: the key chain
+    :return: the value obtained
     """
-    # inicializa a variável de retorno
+    # inicializa
     result: any = source
 
-    # percorre as chaves da cadeia
+    # traverse the keys in the chain
     for key in key_chain:
 
-        # é possível prosseguir ?
+        # is it possible to proceed ?
         if not isinstance(result, dict):
-            # não, encerre a operação
+            # no, terminate the operation
             result = None
             break
 
-        # a chave denota um elemento de lista ?
+        # dos the key refer to an elemenent in a list ?
         if key[-1] == "]":
-            # sim, recupere-o
+            # yes, retrieve it
             pos: int = key.find("[")
             inx: int = int(key[pos+1:-1])
             result = result.get(key[:pos])
 
-            # é possível prosseguir ?
+            # is it possible to proceed ?
             if isinstance(result, list) and len(result) > inx:
-                # sim, prossiga
+                # yes, proceed
                 result = result[inx]
             else:
-                # não, aborte a operação
+                # no, abort the operation
                 result = None
         else:
-            # não, recupere o elemento 'key' do dicionário
+            # no, retrieve the element corresponding to 'key' in the dictionary
             result = result.get(key)
 
     return result
 
 
 def dict_set_value(target: dict, key_chain: list[str], value: any):
     """
-    Atribui ao elemento de *source*, apontado pela cadeia de chaves aninhadas *[keys[0]: ... :keys[n]*,
-    o valor *value*. Caso o elemento final não exista, será criado com o valor especificado.
-    Os elementos intermediários, caso não existam, serão criados com o valor de um *dict* vazio.
+    Assign to an element of *source* the value *value*.
 
-    Uma chave pode indicar a posição do elemento dentro de uma lista, utilizando para tanto
-    o formato *<key>[<pos>]*, e nesse caso, o elemento deve existir.
-
-    :param target: o dict de referência
-    :param key_chain: a cadeia de chaves
-    :param value: o valor a ser atribuído ao elemento
+    The element in question is appointed to by the key chain *[keys[0]: ... :keys[n]*.
+    If the element does not exist, it is created with the specified value.
+    Any non-existing intermediate elements are created with the value of an empty *dict*.
+    A key might indicate the position of the element within a list, using the format *<key>[<pos>]*.
+    In such a case, that element must exist.
+
+    :param target: the reference dict
+    :param key_chain: the key chain
+    :param value: the value to be assigned
     """
     dict_item: any = target
-    # percorre a cadeia até a penúltima chave
+    # traverse the chain, up to end including its penultimate element
     for key in key_chain[:-1]:
 
-        # é possível prosseguir ?
+        # is it possible to proceed ?
         if not isinstance(dict_item, dict):
-            # não, aborte a operação
+            # no, abort the operation
             break
 
-        # a chave denota um elemento de lista ?
+        # does 'key' refer to a list element ?
         if key[-1] == "]":
-            # sim, recupere-o
+            # yes, retrieve it
             pos: int = key.find("[")
             inx: int = int(key[pos+1:-1])
             dict_item = dict_item.get(key[:pos])
-            # é possível prosseguir ?
+            # is it possible to proceed ?
             if isinstance(dict_item, list) and len(dict_item) > inx:
-                # sim, prossiga
+                # yes, proceed
                 dict_item = dict_item[inx]
             else:
-                # não aborte a operação
+                # no, abort the operation
                 dict_item = None
         else:
-            # não, dict_item tem a chave como elemento ?
+            # no, does 'dict_item' have 'key' as one of its elements ?
             if key not in dict_item:
-                # não, atribua a dict_item a chave com valor de um dicionário vazio
+                # não, assign to 'dict_item' the element 'key' with an empty dict as value
                 dict_item[key] = {}
             dict_item = dict_item.get(key)
 
-    # existe chave e dict_item é um dicionário ?
+    # does a key exist and is 'dict_item'a dict ?
     if len(key_chain) > 0 and isinstance(dict_item, dict):
-        # sim, prossiga
+        # yes, proceed
         key: str = key_chain[-1]
-        # a chave denota um elemento de lista ?
+        # does 'key' refer to a list element ?
         if key[-1] == "]":
-            # sim, recupere-o
+            # yes, retrieve it
             pos: int = key.find("[")
             inx: int = int(key[pos+1:-1])
             dict_item = dict_item.get(key[:pos])
-            # a atribuição é possível ?
+            # is the assignment possible ?
             if isinstance(dict_item, list) and len(dict_item) > inx:
-                # sim, faça-a
+                # yes, do it
                 dict_item[inx] = value
         else:
-            # não, faça a atribuição ao elemento 'key' do dicionário
+            # no, assign 'value' to the element 'key' in the dictionary
             dict_item[key] = value
 
 
 def dict_pop_value(target: dict, key_chain: list[str]) -> any:
     """
-    Remove e retorna o valor do elemento de *source* apontado pela cadeia de chaves aninhadas
-    *[keys[0]: ... :keys[n]*. O caminho até a última chave deve apontar para elementos existentes.
+    Remove e retorna o valor do elemento de *source* apontado pela cadeia de chaves *[keys[0]: ... :keys[n]*.
+
+    O caminho até a última chave deve apontar para elementos existentes.
     Uma chave pode indicar a posição do elemento dentro de uma lista, utilizando para tanto
     o formato *<key>[<pos>]*. Retorna *None* se o valor procurado não for encontrado.
 
     Note que o retorno do valor *None* pode não ser indicativo da ausência do elemento em *source*, quando
     da invocaçxão dessa operação, uma vez que esse elemento pode ter existido com o próprio valor *None*.
     Para certificar-se disso, use antes a operação *dict_has_value*.
 
@@ -213,57 +217,58 @@
             result = parent.pop(key)
 
     return result
 
 
 def dict_replace_value(target: dict, old_value: any, new_value: any):
     """
-    Substitui em *target* todas as ocorrências de *old_value* por *new_value*.
+    Replace in *target* all occurrences of *old_value* with *new_value*.
 
-    :param target: o dict de referência
-    :param old_value: o valor a ser substituído
-    :param new_value: o novo valor
+    :param target: the reference dict
+    :param old_value: the value to be replaced
+    :param new_value: the new value
     """
     def list_replace_value(items: list[any], old_val: any, new_val: any):
-        # percorre a lista
+        # traverse the list
         for item in items:
 
-            # o item é um dicionário ?
+            # is 'item' a dict ?
             if isinstance(item, dict):
-                # sim, processe-o recursivamente
+                # yes, process it recursively
                 dict_replace_value(item, old_val, new_val)
 
-            # o item é uma lista ?
+            # is 'item' a list ?
             elif isinstance(item, list):
-                # sim, processe-o recursivamente
+                # yes, process it recursively
                 list_replace_value(item, old_val, new_val)
 
-    # percorre o dicionário
+    # traverse the dict
     for curr_key, curr_value in target.items():
 
-        # o valor atual é o valor buscado ?
+        # is 'curr_value' the value to be replaced ?
         if curr_value == old_value:
-            # sim, substitua-o
+            # yes, replace it
             target[curr_key] = new_value
 
-        # o valor atual é um dicionário ?
+        # is 'curr_value' a dict ?
         elif isinstance(curr_value, dict):
-            # sim, processe-o recursivamente
+            # yes, process it recursively
             dict_replace_value(curr_value, old_value, new_value)
 
-        # o valor atual é uma lista ?
+        # is 'curr_value' a list ?
         elif isinstance(curr_value, list):
-            # sim, processe-o recursivamente
+            # yes, process it recursively
             list_replace_value(curr_value, old_value, new_value)
 
 
 def dict_get_key(source: dict, value: any) -> any:
     """
-    Retorna a chave em *source*, associada à primeira ocorrência de *value* encontrada,
-    ou *None*, se nenhuma chave for encontrada. Apenas os atributos no primeiro nível
+    Retorna a chave em *source*, associada à primeira ocorrência de *value* encontrada.
+
+    Retorna *None*, se nenhuma chave for encontrada. Apenas os atributos no primeiro nível
     em *source* são inspecionados.
 
     :param source: dicionário a ser pesquisado
     :param value: valor de referência
     :return: primeira chave associada ao valor de referência
     """
     result: any = None
@@ -273,34 +278,36 @@
             break
 
     return result
 
 
 def dict_get_keys(source: dict, value: any) -> list[str]:
     """
-    Restorna lista com todas as chaves ne primeiro nível em *source*, associadas a *value*,
-    ou *[]* se nenhuma chave for encontrada.
+    Restorna lista com todas as chaves ne primeiro nível em *source*, associadas a *value*.
+
+    Retorna *[]* se nenhuma chave for encontrada.
 
     :param source: dicionário a ser pesquisado
     :param value: valor de referência
     :return: lista de chaves associadas ao valor de referência
     """
     return [key for key, val in source.items() if val == value]
 
 
 def dict_merge(target: dict, source: dict):
     """
-    Percorre os elementos de *source* para atualizar *target*, obedecendo aos seguintes os critérios:
-
-    - acrescentar o elemento a *target*, se não existir
-    - se o elemento existir em *target*:
+    Percorre os elementos de *source* para atualizar *target*, obedecendo um conjunto de critérios.
 
-      -   processar recursivamente os dois elementos, se ambos forem do tipo *dict*
-      -   acrescentar os itens faltantes, se ambos forem do tipo *list*
-      -   substituir o elemento em *target* se for de outro tipo, ou se os tipos forem diferentes entre si
+    Os critérios a sere mseguidos são:
+      - acrescentar o elemento a *target*, se não existir
+      - se o elemento existir em *target*:
+
+        - processar recursivamente os dois elementos, se ambos forem do tipo *dict*
+        - acrescentar os itens faltantes, se ambos forem do tipo *list*
+        - substituir o elemento em *target* se for de outro tipo, ou se os tipos forem diferentes entre si
 
     :param target: o dicionário a ser atualizado
     :param source: o dicionário com os novos elementos
     """
     # percorre o dicionário com os novos elementos
     for skey, svalue in source.items():
 
@@ -326,16 +333,17 @@
         else:
             # não, acrescente-o
             target[skey] = svalue
 
 
 def dict_coalesce(target: dict, key_chain: list[str]):
     """
-    Coalesce o elemento do tipo *list* em *target* no nível *n*, apontado pela cadeia de
-    chaves aninhadas *[keys[0]: ... :keys[n]*, com a lista no nível imediatamente anterior,
+    Coalesce o elemento do tipo *list* em *target* no nível *n*, com a lista no nível imediatamente anterior.
+
+    Esse elemento é apontado pela cadeia de chaves aninhadas *[keys[0]: ... :keys[n]*, e é processado
     como uma sequência de multiplos elementos. Para tanto, as duas últimas chaves da cadeia
     *key_chain* devem estar associadas a valores do tipo *list*.
 
     :param target: o dicionário a ser coalescido
     :param key_chain: a cadeia de chaves
     """
     # a cadeia de chaves contem mais de 2 chaves ?
@@ -422,17 +430,18 @@
 
             # substitue a lista original associada à penúltima chave com a nova lista coalescida
             curr_dict[key_chain[-2]] = penultimate_list
 
 
 def dict_reduce(target: dict, key_chain: list[str]):
     """
-    Realoca os elementos de *target* no nível *n*, apontados pela cadeia de chaves aninhadas
-    *[keys[0]: ... :keys[n]*, para o nível imediatamente acima, e remove o elemento no nivel *n*
-    ao final.
+    Realoca os elementos de *target* no nível *n*, para o nível imediatamente acima.
+
+    Esses elementos são apontados pela cadeia de chaves aninhadas *[keys[0]: ... :keys[n]*.
+    O elemento no nivel *n* é removido, ao final.
 
     :param target: o dicionário a ser reduzido
     :param key_chain: a cadeia de chaves
     """
     # a cadeia de chaves contem pelo menos 1 chave ?
     if len(key_chain) > 0:
         # sim, prossiga
@@ -470,16 +479,17 @@
             last: dict = curr_dict.pop(last_key)
             for key, value in last.items():
                 curr_dict[key] = value
 
 
 def dict_from_list(source: list[dict], key_chain: list[str], value: any) -> dict:
     """
-    Localiza em *source*, e retorna, o elemento do tipo *dict* contendo a cadeia de chaves
-    *key_chain* com o valor *value*. Retorna *None* se esse *dict* não for encontrado.
+    Localiza em *source*, e retorna, o elemento do tipo *dict* com o valor *value* na cadeia de chaves *key_chain*.
+
+    Retorna *None* se esse *dict* não for encontrado.
 
     :param source: a lista a ser inspecionada
     :param key_chain: a cadeia de chaves usada na busca
     :param value: o valor associado à cadeia de chaves
     :return: o dict procurado
     """
     # inicializa a variável de retorno
@@ -492,16 +502,17 @@
             break
 
     return result
 
 
 def dict_from_object(source: object) -> dict:
     """
-    Percorre *source* e cria um *dict* com seus atributos contendo valores não nulos. *source* pode ser
-    qualquer objeto, especialmente aqueles que tenham sido decorados com *@dataclass*.
+    Percorre *source* e cria um *dict* com seus atributos contendo valores não nulos.
+
+    *source* pode ser qualquer objeto, especialmente aqueles que tenham sido decorados com *@dataclass*.
 
     :param source: o objeto de referência
     :return: dicionário com estrutura equivalente ao objeto de referência
     """
     # inicializa a variável de retorno
     result: dict = {}
 
@@ -536,15 +547,17 @@
 
     return result
 
 
 def dict_transform(source: dict, from_to_keys: list[tuple[str, str]],
                    prefix_from: str = None, prefix_to: str = None) -> dict:
     """
-    Constrói um novo *dict*, atribuindo a cada elemento indicado pelo segundo elemento de uma
+    Constrói um novo *dict*, segundo as regras seguintes.
+
+    Esse dicionário é construído atribuindo-se a cada elemento indicado pelo segundo elemento de uma
     tupla contendo uma cadeia de chaves aninhadas em *from_to_keys*, o valor do elemento
     de *source* indicado pelo primeiro elemento da tupla, também contendo uma cadeia de chaves
     aninhadas, respectivamente para todos os elementos mapeados em *from_to_keys*.
 
     Os prefixos para as chaves de origem e de destino, se definidos, tem tratamentos distintos.
     São acrescentados na busca de valores em *Source*, e removidos na atribuição de valores
     ao *dict* de retorno.
@@ -596,16 +609,17 @@
             dict_set_value(result, to_keys_deep, to_value)
 
     return result
 
 
 def dict_listify(target: dict, key_chain: list[str]):
     """
-    Insere o valor do item de *target* apontado pela cadeia de chaves aninhadas
-    *[keys[0]: ... :keys[n]* em uma lista, se esse valor já não for uma lista.
+    Insere o valor do item de *target* apontado pela cadeia de chaves *[keys[0]: ... :keys[n]* em uma lista.
+
+    Essa inserção ocorrerá apenas se esse valor já não for uma lista.
     Todas as listas eventualmente encontradas no percurso até a penúltima chava
     da cadeia serão recursivamente processadas.
 
     :param target: dicionário a ser modificado
     :param key_chain: cadeia de chaves aninhadas apontando para o item em questão
     """
     def items_listify(in_targets: list, in_keys: list[str]):
```

### Comparing `pypomes_core-0.2.0/src/pypomes_core/email_pomes.py` & `pypomes_core-0.2.1/src/pypomes_core/email_pomes.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,30 +7,37 @@
 EMAIL_ACCOUNT: Final[str] = env_get_str(f"{APP_PREFIX}_EMAIL_ACCOUNT")
 EMAIL_PWD: Final[str] = env_get_str(f"{APP_PREFIX}_EMAIL_PWD")
 EMAIL_PORT: Final[int] = env_get_int(f"{APP_PREFIX}_EMAIL_PORT")
 EMAIL_SERVER: Final[str] = env_get_str(f"{APP_PREFIX}_EMAIL_SERVER")
 
 
 def email_send(errors: list[str], user_email: str, subject: str, content: str):
+    """
+    Send email, to *user_email", with *subject* as the email subject, and *content* as the email message.
 
+    :param errors: incidental error messages
+    :param user_email: the address to send the email to
+    :param subject: the email subject
+    :param content: the email message
+    """
     # import needed function
     from .exception_pomes import exc_format
 
-    # connstrói o email
+    # build the email object
     email_msg = EmailMessage()
     email_msg.set_content(content)
     email_msg["Subject"] = subject
     email_msg["From"] = EMAIL_ACCOUNT
     email_msg["To"] = user_email
 
-    # instancia o email server
+    # instanciate the email server
     server = SMTP(host=EMAIL_SERVER, port=EMAIL_PORT)
     server.starttls()
     server.login(user=EMAIL_ACCOUNT, password=EMAIL_PWD)
 
-    # envia a mensagem
+    # send the message
     try:
         server.send_message(email_msg)
         server.quit()
     except Exception as e:
-        # a operação resultou em exceção
-        errors.append(f"Erro no envio de email: {exc_format(e, sys.exc_info())}")
+        # the operatin raised an exception
+        errors.append(f"Error sending the email: {exc_format(e, sys.exc_info())}")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypomes_core-0.2.0/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.2.1/src/pypomes_core/encoding_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 def encode_ascii_hex(source: bytes) -> bytes:
-    """
-    Codifica o conteúdo binário em texto, com caracteres para bytes no intervalo ASCII,
+    r"""
+    Codifica o conteúdo binário em texto.
+
+    Essa codificação é feita com caracteres para bytes no intervalo ASCII,
     com a representação *backslash-escaped* para os caracteres especiais LF, HT, CR, VT, FF e BS,
-    e com a representação *\\\\xNN* para os demais (onde *N* é um dígito hexadecimal [0-9] e [a-f]).
+    e com a representação *\\xNN* para os demais (onde *N* é um dígito hexadecimal [0-9] e [a-f]).
 
     :param source: o conteúdo binário a ser codificado
     :return: o conteúdo texto codificado
     """
     # inicializa a variável de retorno
     result: bytes = b""
 
@@ -41,18 +43,20 @@
             result += byte_str.encode()
         pos += 1
 
     return result
 
 
 def decode_ascii_hex(source: bytes) -> bytes:
-    """
-    Decodifica em binário o conteúdo texto codificado com caracteres para bytes no intervalo ASCII,
+    r"""
+    Decodifica em binário o conteúdo texto.
+
+    Essa decodificação é feita para texto codificado com caracteres para bytes no intervalo ASCII,
     com a representação *backslash-escaped* para os caracteres especiais LF, HT, CR, VT, FF e BS,
-    e com a representação *\\\\xNN* para os demais (onde *N* é um dígito hexadecimal [0-9] e [a-f]).
+    e com a representação *\\xNN* para os demais (onde *N* é um dígito hexadecimal [0-9] e [a-f]).
 
     :param source: o conteúdo texto a ser decodificado
     :return: o conteúdo binário decodificado
     """
     # inicializa a variável de retorno
     result: bytes = b""
```

### Comparing `pypomes_core-0.2.0/src/pypomes_core/env_pomes.py` & `pypomes_core-0.2.1/src/pypomes_core/env_pomes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,73 @@
 import os
 
 
 def env_get_str(key: str, def_value: str = None) -> str:
     """
-    Return the string value defined for *key* in the current operating environment.
+    Retrieve and return the string value defined for *key* in the current operating environment.
 
-    :param key: The key the value is associated with.
-    :param def_value: The default value to return, if the key has not been defined.
-    :return: The int value associated with the key.
+    :param key: The key the value is associated with
+    :param def_value: The default value to return, if the key has not been defined
+    :return: The int value associated with the key
     """
     result: str
     try:
         result = os.environ[key]
     except (KeyError, TypeError):
         result = def_value
 
     return result
 
 
 def env_get_bool(key: str, def_value: bool = None) -> bool:
     """
-    Return the boolean value defined for *key* in the current operating environment.
+    Retrieve and return the boolean value defined for *key* in the current operating environment.
 
-    :param key: The key the value is associated with.
-    :param def_value: The default value to return, if the key has not been defined.
-    :return: The boolean value associated with the key.
+    :param key: The key the value is associated with
+    :param def_value: The default value to return, if the key has not been defined
+    :return: The boolean value associated with the key
     """
     result: bool
     try:
         result = bool(os.environ[key])
     except (KeyError, TypeError):
         result = def_value
 
     return result
 
 
 def env_get_int(key: str, def_value: int = None) -> int:
     """
-    Return the int value defined for *key* in the current operating environment.
+    Retrieve and return the int value defined for *key* in the current operating environment.
 
-    :param key: The key the value is associated with.
-    :param def_value: The default value to return, if the key has not been defined.
-    :return: The int value associated with the key.
+    :param key: The key the value is associated with
+    :param def_value: The default value to return, if the key has not been defined
+    :return: The int value associated with the key
     """
     result: int
     try:
         result = int(os.environ[key])
     except (KeyError, TypeError):
         result = def_value
 
     return result
 
 
 def env_get_float(key: str, def_value: float = None) -> float:
     """
-    Return the float value defined for *key* in the current operating environment.
+    Retrieve and return the float value defined for *key* in the current operating environment.
 
-    :param key: The key the value is associated with.
-    :param def_value: The default value to return, if the key has not been defined.
-    :return: The float value associated with the key.
+    :param key: The key the value is associated with
+    :param def_value: The default value to return, if the key has not been defined
+    :return: The float value associated with the key
     """
     result: float
     try:
         result = int(os.environ[key])
     except (KeyError, TypeError):
         result = def_value
 
     return result
 
 
+# the prefix to the names of the environment variables
 APP_PREFIX = env_get_str("PYPOMES_APP_PREFIX", "PYPOMES")
```

### Comparing `pypomes_core-0.2.0/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.2.1/src/pypomes_core/exception_pomes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from types import TracebackType
-from typing import Type
 import os
 import traceback
 
 
-def exc_format(exc: Exception, exc_info: tuple[Type[BaseException], BaseException, TracebackType]) -> str:
+def exc_format(exc: Exception,
+               exc_info: tuple[type[BaseException], BaseException, TracebackType]) -> str:
     """
-    Formata a mensagem de erro decorrente da exceção levantada em tempo de execução, no formato:
+    Format the error message resulting from the exception raised in execution time.
 
-    <python_module>, <line_number>: <exc_class> - <exc_text>
+    The format to use: <python_module>, <line_number>: <exc_class> - <exc_text>
 
-    :param exc: a exceção levantada
-    :param exc_info: informações associadas à exceção
-    :return: a mensagem de erro formatada
+    :param exc: the exception raised
+    :param exc_info: information associated with the exception
+    :return: the formatted message
     """
     tback: TracebackType = exc_info[2]
     cls: str = str(exc.__class__)
 
-    # obtem o ponto de execução que provocou a exceção (última posição na pilha)
+    # retrieve the execution point where the exception was raised (bottom of the stack)
     tlast: traceback = tback
     while tlast.tb_next is not None:
         tlast = tlast.tb_next
 
-    # obtem nome do módulo e linha do código (origem da exceção)
+    # retrieve the module name and the line number within the module
     try:
         fname: str = os.path.split(tlast.tb_frame.f_code.co_filename)[1]
     except Exception:
         fname: str = "<unknow module>"
     fline: int = tlast.tb_lineno
     return f"{fname}, {fline}, {cls[8:-2]} - {exc}"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypomes_core-0.2.0/src/pypomes_core/json_pomes.py` & `pypomes_core-0.2.1/src/pypomes_core/json_pomes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import base64
-from typing import Iterable
+from collections.abc import Iterable
 
 
 def json_normalize_dict(source: dict):
     """
-    Turns the values in *source* into values that can be serialized to JSON, avoiding *TypeError*:
+    Turn the values in *source* into values that can be serialized to JSON, avoiding *TypeError*.
 
-    - *bytes* e *bytearray* are changed to *str* in *Base64* format
-    - *Iterable* is changed into a *list*
-    - all other types kept as they are
+    Possible transformations:
+        - *bytes* e *bytearray* are changed to *str* in *Base64* format
+        - *Iterable* is changed into a *list*
+        - all other types kept as they are
     HAZARD: depending on the type of object contained in *source*, the final result may not be serializable.
 
     :param source: the dict to be made serializable
     """
     for key, value in source.items():
         if isinstance(value, dict):
             json_normalize_dict(value)
@@ -20,22 +21,24 @@
             source[key] = base64.b64encode(value).decode()
         elif isinstance(value, Iterable) and not isinstance(value, str):
             source[key] = json_normalize_iterable(value)
 
 
 def json_normalize_iterable(source: Iterable) -> list[any]:
     """
-    Turns the values in *source* into values that can be serialized to JSON, avoiding *TypeError*:
+    Turn the values in *source* into values that can be serialized to JSON, avoiding *TypeError*.
 
-    - *bytes* e *bytearray* are changed to *str* in *Base64* format
-    - *Iterable* is changed into a *list*
-    - all other types kept as they are
+    Possible operations:
+        - *bytes* e *bytearray* are changed to *str* in *Base64* format
+        - *Iterable* is changed into a *list*
+        - all other types kept as they are
     HAZARD: depending on the type of object contained in *source*, the final result may not be serializable.
 
     :param source: the dict to be made serializable
+    :return
     """
     result: list[any] = []
     for value in source:
         if isinstance(value, dict):
             json_normalize_dict(value)
             result.append(value)
         elif isinstance(value, bytes) or isinstance(value, bytearray):
```

### Comparing `pypomes_core-0.2.0/src/pypomes_core/list_pomes.py` & `pypomes_core-0.2.1/src/pypomes_core/list_pomes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 def list_compare(list1: list[any], list2: list[any]) -> bool:
     """
-    Compare o conteúdo de duas listas *list1* e *list2*, e retorna *True* se todos os elementos de *list1*
-    estão em *list2*, e vice-versa, na mesma quantidade.
+    Compare the contents of the two lists *list1* e *list2*.
 
-    :param list1: a primeira lista
-    :param list2: a segunda lista
-    :return: True se as duas listas contem os mesmos elementos, na mesma quantidade, em qualquer ordem
+    Return *True* if all the elements in *list1* are also in *list2*, and vice-versa, in the same quantity.
+
+    :param list1: the first list
+    :param list2: the second list
+    :return: True if the two lists contain the same elements, in the same quantity, in any order
     """
     # inicializa variável de retorno
     result: bool = True
 
     # os parâmetros são listas, e contêm o mesmo número de elementos ?
     if isinstance(list1, list) and isinstance(list2, list) and len(list1) == len(list2):
         # sim, verifique se todos os elementos de 'list1' estão em 'list2', na mesma quantidade
@@ -24,56 +25,59 @@
         result = False
 
     return result
 
 
 def list_flatten(source: list[str]) -> str:
     """
-    Transforma uma lista de *str* em uma *str* consistindo na concatenação com "." dos elementos da lista. Exemplos:
+    Transforma uma lista de *str* em uma *str* consistindo na concatenação com "." dos elementos da lista.
 
-    - ['1', '2', '']     -> '1.2.'
-    - ['', 'a', 'b']     -> '.a.b'
-    - ['x', '', '', 'y'] -> 'x...y'
-    - ['z']              -> 'z'
+    Exemplos:
+        - ['1', '2', '']     -> '1.2.'
+        - ['', 'a', 'b']     -> '.a.b'
+        - ['x', '', '', 'y'] -> 'x...y'
+        - ['z']              -> 'z'
 
     :param source: a lista de strings
     :return: a string concatenada
     """
     result: str = ""
     for item in source:
         result += "." + item
     result = result[1:]
 
     return result
 
 
 def list_unflatten(source: str) -> list[str]:
     """
-    Transforma uma *str* contendo elementos concatenados por "." em uma lista de *str*,
-    contendo os sub_elementos extraídos. Exemplos:
+    Transforma uma *str* contendo elementos concatenados por "." em uma lista de *str*.
 
-    - '1.2.'  -> ['1', '2', '']
-    - '.a.b'  -> ['', 'a', 'b']
-    - 'x...y' -> ['x', '', '', 'y']
-    - 'z'     -> ['z']
+    Essa lista contem os sub_elementos extraídos. Exemplos:
+        - '1.2.'  -> ['1', '2', '']
+        - '.a.b'  -> ['', 'a', 'b']
+        - 'x...y' -> ['x', '', '', 'y']
+        - 'z'     -> ['z']
 
     :param source: string com elementos concatenados por "."
     :return: a lista de strings contendo os elementos da concatenação
     """
     # import the needed function
     from .str_pomes import str_split_on_mark
 
     return str_split_on_mark(source, ".")
 
 
 def list_find_coupled(coupled_elements: list[tuple[str, str]], primary_element: str) -> str:
     """
-    Localiza em *coupled_elements* o elemento acoplado ao *primary_element* dado. Se *primary_element* contiver
-    indicação de índice (denotado por *[<pos>]*), essa indicação é removida. Essa função é utilizada na transformação
-    de *dicts* (*dict_transform*) e *lists* (*list_transform*) a partir de sequências de pares de chaves.
+    Localiza em *coupled_elements* o elemento acoplado ao *primary_element* dado.
+
+    Se *primary_element* contiver indicação de índice (denotado por *[<pos>]*), essa indicação é removida.
+    Essa função é utilizada na transformação de *dicts* (*dict_transform*) e *lists* (*list_transform*),
+    a partir de sequências de pares de chaves.
 
     :param coupled_elements: a lista de tuplas contendo os pares de elementos.
     :param primary_element: o elemento primário
     :return: o elemento acoplado, ou None se não for encontrado
     """
     # remove a indicação de elemento de lista
     pos1: int = primary_element.find("[")
@@ -95,29 +99,28 @@
 
     return result
 
 
 def list_transform(source: list[any], from_to_keys: list[tuple[str, str]],
                    prefix_from: str = None, prefix_to: str = None) -> list[any]:
     """
-    Constrói uma nova *list*, transformando elementos do tipo *list* e *dict*
-    que estejam contidos em *source*. A conversão dos elementos tipo *dict* está
-    documentada na função *dict_transform*.
+    Constrói uma nova *list*, transformando elementos do tipo *list* e *dict* encontrados em *source*.
+
+    A conversão dos elementos tipo *dict* está documentada na função *dict_transform*.
 
     Os prefixos para as chaves de origem e de destino, se definidos, tem tratamentos distintos.
     São acrescentados na busca de valores em *Source*, e removidos na atribuição de valores
     ao *dict* de retorno.
 
     :param source: o dict de origem dos valores
     :param from_to_keys: a lista de tuplas contendo as sequências de chaves de origem e destino
     :param prefix_from: prefixo a ser acrescentado às chaves de origem
     :param prefix_to: prefixo a ser removido das chaves de destino
     :return: a nova lista
     """
-
     # import the needed function
     from .dict_pomes import dict_transform
 
     # inicializa a variável de retorno
     result: list[any] = []
 
     # percorre a lista de origem
@@ -141,20 +144,21 @@
     return result
 
 
 def list_elem_starting_with(source: list[str | bytes],
                             prefix: str | bytes, keep_prefix: bool = True) -> str | bytes:
     """
     Localiza e retorna o primeiro elemento em *source* prefixado por *prefix*.
+
     Retorna *None* se esse elemento não for encontrado.
 
     :param source: a lista a ser inspecionada
     :param prefix: o dado prefixando o elemento a ser retornado
     :param keep_prefix: define se o elemento encontrado deve ou não ser retornado com o prefixo
-    :return: O elemento prefixado, com ou sem o prefixo
+    :return: o elemento prefixado, com ou sem o prefixo
     """
     # inicializa a variável de retorno
     result: str | bytes | None = None
 
     # percorre a lista de origem
     for elem in source:
         if elem.startswith(prefix):
```

### Comparing `pypomes_core-0.2.0/src/pypomes_core/logging_pomes.py` & `pypomes_core-0.2.1/src/pypomes_core/logging_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 LOGGING_ID: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_ID", f"{APP_PREFIX}")
 LOGGING_FORMAT: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_FORMAT",
                                          "{asctime} {levelname:1.1} {thread:5d} "
                                          "{module:20.20} {funcName:20.20} {lineno:3d} {message}")
 LOGGING_STYLE: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_STYLE", "{")
 
 LOGGING_FILE_PATH: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_FILE_PATH",
-                                            os.path.join(tempfile.gettempdir(), f"{APP_PREFIX}.log"))
+                                            os.path.join(tempfile.gettempdir(),
+                                                         f"{APP_PREFIX}.log"))
 LOGGING_FILE_MODE: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_FILE_MODE", "a")
 
 # define and configure the logger
 PYPOMES_LOGGER: Final[logging.Logger] = logging.getLogger(LOGGING_ID)
 
 # define the logging severity level
 # noinspection PyTypeChecker
@@ -64,16 +65,17 @@
 
 
 def logging_get_entries(errors: list[str],
                         log_level:  Literal["debug", "info", "warning", "error", "critical"] = None,
                         log_from: str = None, log_to: str = None,
                         file_path: str = LOGGING_FILE_PATH) -> BytesIO:
     """
-    Extract and return all entries in *PYPOMES_LOGGER*'s logging file,
-    meeting the criteria specified by *log_level* and by the inclusive interval *[log_from, log_to]*.
+    Extract and return all entries in *PYPOMES_LOGGER*'s logging file.
+
+    The extraction meets the criteria specified by *log_level* and by the inclusive interval *[log_from, log_to]*.
 
     :param errors: errors eventually generated during execution
     :param log_level: the logging level (defaults to all levels)
     :param log_from: the initial timestamp (defaults to unspecified)
     :param log_to: the finaL timestamp (defaults to unspecified)
     :param file_path: the path of the log file
     :return: the logging entries meeting the specified criteria
@@ -105,15 +107,15 @@
         # no, report the error
         errors.append(f"File '{file_path}' not found")
 
     # any error ?
     if len(errors) == 0:
         # no, proceed
         result = BytesIO()
-        with open(file_path, "r") as f:
+        with open(file_path) as f:
             line: str = f.readline()
             while line:
                 items: list[str] = line.split(maxsplit=3)
                 # noinspection PyTypeChecker
                 msg_level: int = __get_logging_level(items[2])
                 if msg_level >= logging_level:
                     timestamp: datetime = parser.parse(f"{items[0]} {items[1]}")
@@ -122,19 +124,21 @@
                         result.write(line.encode())
                 line = f.readline()
 
     return result
 
 
 def logging_log_msgs(msgs: list[str], output_dev: TextIO = None,
-                     log_level: Literal["debug", "info", "warning", "error", "critical"] = "error",
+                     log_level: Literal["debug", "info", "warning",
+                                        "error", "critical"] = "error",
                      logger: logging.Logger = PYPOMES_LOGGER):
     """
-    Write all messages in *msgs* to *PYPOMES_LOGGER*'s logging file, and to *output_dev*
-    (tipically, *sys.stdout* ou *sys.stderr*).
+    Write all messages in *msgs* to *PYPOMES_LOGGER*'s logging file, and to *output_dev*.
+
+    The output device is tipically *sys.stdout* ou *sys.stderr*.
 
     :param msgs: the messages list
     :param output_dev: output device where the message is to be printed (None for no device printing)
     :param log_level: the logging level, defaults to 'error' (None for no logging)
     :param logger: the logger to use
     """
     # define the log writer
```

### Comparing `pypomes_core-0.2.0/src/pypomes_core/str_pomes.py` & `pypomes_core-0.2.1/src/pypomes_core/str_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 def str_split_on_mark(source: str, mark: str) -> list[str]:
     """
     Extrai, de *source*, os segmentos de texto separados por *mark*, e os retorna em uma lista.
+
     Os segmentos retornados não contem o separador.
 
     :param source: o texto de referência
     :param mark: o separador
     :return: a lista de segmentos de texto obtidos
     """
     # inicializa a variável de retorno
@@ -23,16 +24,17 @@
         result.append("")
 
     return result
 
 
 def str_between(source: str, from_str: str, to_str: str) -> str:
     """
-    Extrai e retorna a *substring* em *source* localizada entre os delimitadores
-    *from_st* e *to_str*, ou *None* se essa extração não for possível.
+    Extrai e retorna a *substring* em *source* localizada entre os delimitadores *from_st* e *to_str*.
+
+    Retorna *None* se essa extração não for possível.
 
     :param source: a string a ser pesquisada
     :param from_str: o delimitador inicial
     :param to_str: o delimitador final
     :return: a substring procurada
     """
     # inicializa a variável de retorno
@@ -47,14 +49,15 @@
 
     return result
 
 
 def str_find_whitespace(source: str) -> int:
     """
     Localiza e retorna a posição da primeira ocorrência de *whitespace* em *source*.
+
     Retorna *-1* se nenhum *whitespace* for encontrado.
 
     :param source: a string a ser pesquisada
     :return: a posição do primeiro whitespace encontrado
     """
     # inicializa a variável de retorno
     result: int = -1
```

### Comparing `pypomes_core-0.2.0/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.2.1/src/pypomes_core/xml_pomes.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 XML_FILE_HEADER: Final[str] = '<?xml version="1.0" encoding="UTF-8" ?>'
 
 
 def xml_normalize_keys(source: dict) -> dict:
     """
     Clona o *source*, removenda os *namespaces* e os prefixos *'@'* e *'#'* nos nomes de suas chaves.
+
     A ordem das chaves é mantida.
 
     :param source: o dict de referência
     :return: um novo dict normalizado
     """
     # inicializa a variável de retorno
     result: dict = {}
@@ -45,16 +46,18 @@
                 result[curr_key[pos+1:]] = curr_value
 
     return result
 
 
 def xml_to_dict(file_data: bytes | str) -> dict:
     """
-    Converte XML em um dict sem namespaces e sem chaves com prefixos "@" e "#". O XML de entrada deve estar em
-    *file_data* (tipo *bytes*), ou em arquivo do sistema com o caminho especificado por *file_data* (tipo *str*).
+    Convert the XML into a *dict*, by removing namespaces, and keys prefixed with "@" e "#".
+
+    O XML de entrada deve estar em *file_data* (tipo *bytes*),
+    ou em arquivo do sistema com o caminho especificado por *file_data* (tipo *str*).
 
     :param file_data: XML a ser convertido
     :return: dict normalizado
     """
     # file_data é o próprio conteúdo XML ?
     if isinstance(file_data, bytes):
         # sim
```

### Comparing `pypomes_core-0.2.0/LICENSE` & `pypomes_core-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.0/pyproject.toml` & `pypomes_core-0.2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "Flask>=2.3.2",
-    "pip>=23.1.2",
+    "pip>=23.2.1",
     "python-dateutil>=2.8.2",
+    "requests>=2.31.0",
     "setuptools>=68.0.0",
-    "wheel>=0.40.0",
+    "wheel>=0.41.0",
     "xmltodict3>=0.0.4"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Core"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-Core/issues"
```

### Comparing `pypomes_core-0.2.0/PKG-INFO` & `pypomes_core-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pypomes_core
-Version: 0.2.0
+Version: 0.2.1
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: flask>=2.3.2
-Requires-Dist: pip>=23.1.2
+Requires-Dist: pip>=23.2.1
 Requires-Dist: python-dateutil>=2.8.2
+Requires-Dist: requests>=2.31.0
 Requires-Dist: setuptools>=68.0.0
-Requires-Dist: wheel>=0.40.0
+Requires-Dist: wheel>=0.41.0
 Requires-Dist: xmltodict3>=0.0.4
```

