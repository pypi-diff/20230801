# Comparing `tmp/pypomes_soap-0.1.2.tar.gz` & `tmp/pypomes_soap-0.1.3.tar.gz`

## Comparing `pypomes_soap-0.1.2.tar` & `pypomes_soap-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 pypomes_soap-0.1.2/src/pypomes_soap/__init__.py
--rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 pypomes_soap-0.1.2/src/pypomes_soap/soap_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_soap-0.1.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_soap-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_soap-0.1.2/README.md
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pypomes_soap-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 pypomes_soap-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 pypomes_soap-0.1.3/src/pypomes_soap/__init__.py
+-rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 pypomes_soap-0.1.3/src/pypomes_soap/soap_pomes.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pypomes_soap-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_soap-0.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_soap-0.1.3/README.md
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pypomes_soap-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 pypomes_soap-0.1.3/PKG-INFO
```

### Comparing `pypomes_soap-0.1.2/src/pypomes_soap/soap_pomes.py` & `pypomes_soap-0.1.3/src/pypomes_soap/soap_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import ast
 import json
 import requests
 from lxml import etree
-from pypomes_core.json_pomes import jsonify_dict
-from pypomes_core.xml_pomes import xml_to_dict
+from pypomes_core import json_normalize_dict, xml_to_dict
 from zeep import Client
 
 
 def soap_build_envelope(zeep_client: Client, service: str, payload: dict, file_path: str = None) -> bytes:
     """
     Constrói e retorna o envelope SOAP para um dado serviço. Esse envelope não contem os *headers*.
 
@@ -76,28 +75,29 @@
     """
     # invoca o servico
     # ('response' é uma subclasse de dict - definida como retorno do 'zeep_service' no wsdl)
     response: any = zeep_service(**payload)
 
     # converte o conteúdo retornado em dict e o prepara para descarga em JSON
     result: dict = ast.literal_eval(str(response))
-    jsonify_dict(result)
+    json_normalize_dict(result)
 
     # salva o retorno em arquivo ?
     if file_path is not None:
         # sim
         with open(file_path, "w") as f:
             f.write(json.dumps(result, ensure_ascii=False))
 
     return result
 
 
 def soap_get_dict(soap_response: bytes, xml_path: str = None, json_path: str = None) -> dict:
     """
     Recupera o objeto *dict* contendo os dados retornados pela solicitação SOAP.
+
     Esse objeto é retornado em condições de ser descarregado em formato JSON.
 
     :param soap_response: o conteúdo retornado pela solicitação SOAP
     :param xml_path: Path to store the XML correspondinge to the returned response.
     :param json_path: Path to store the JSON correspondinge to the returned response.
     :return: o objeto com os dados de resposta à solicitação
     """
@@ -110,15 +110,15 @@
     if xml_path is not None:
         # sim
         with open(xml_path, "wb") as f:
             f.write(content)
 
     # converte o conteúdo XML em dict e o prepara para descarga em JSON
     result: dict = xml_to_dict(content)
-    jsonify_dict(result)
+    json_normalize_dict(result)
 
     # salva o retorno em arquivo ?
     if json_path is not None:
         # sim
         with open(json_path, "w") as f:
             f.write(json.dumps(result, ensure_ascii=False))
 
@@ -155,16 +155,17 @@
         pos_1 = soap_response.find(prefix, pos_1)
 
     return result
 
 
 def soap_get_attachment(soap_response: bytes, cid: bytes, file_path: str = None) -> bytes:
     """
-    Obtem e retorna o anexo contido no *response* da solicitação *SOAP*, no padrão *MTOM*
-    (*Message Transmission Optimization Mechanism*), e identificado pelo *cid* (Content-ID).
+    Obtem e retorna o anexo contido no *response* da solicitação *SOAP*, no padrão *MTOM*.
+
+    Nesse padrão (*Message Transmission Optimization Mechanism*), o anexo é identificado pelo *cid* (Content-ID).
 
     :param soap_response: o conteúdo retornado pela solicitação SOAP
     :param cid: a identificação do anexo
     :param file_path: Path to store the JSON corresponding to the returned attachment.
     :return: o anexo em referência, ou None se não for encontrado
     """
     # inicializa a variável de retorno
```

### Comparing `pypomes_soap-0.1.2/LICENSE` & `pypomes_soap-0.1.3/LICENSE`

 * *Files identical despite different names*

