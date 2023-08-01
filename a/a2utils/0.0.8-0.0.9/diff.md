# Comparing `tmp/a2utils-0.0.8-py3-none-any.whl.zip` & `tmp/a2utils-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 17473 bytes, number of entries: 8
--rwxr-xr-x  2.0 unx    17230 b- defN 20-Dec-06 17:15 a2utils-0.0.8.data/scripts/a2certbot
--rwxr-xr-x  2.0 unx     5782 b- defN 20-Dec-06 17:15 a2utils-0.0.8.data/scripts/a2conf
--rwxr-xr-x  2.0 unx     3245 b- defN 20-Dec-06 17:15 a2utils-0.0.8.data/scripts/a2okerr
--rwxr-xr-x  2.0 unx    12191 b- defN 20-Dec-06 17:15 a2utils-0.0.8.data/scripts/a2vhost
--rw-r--r--  2.0 unx    14610 b- defN 20-Dec-06 17:15 a2utils-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 20-Dec-06 17:15 a2utils-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 20-Dec-06 17:15 a2utils-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      665 b- defN 20-Dec-06 17:15 a2utils-0.0.8.dist-info/RECORD
-8 files, 53816 bytes uncompressed, 16313 bytes compressed:  69.7%
+Zip file size: 17619 bytes, number of entries: 8
+-rwxr-xr-x  2.0 unx    17230 b- defN 20-Dec-06 17:15 a2utils-0.0.9.data/scripts/a2certbot
+-rwxr-xr-x  2.0 unx     5782 b- defN 20-Dec-06 17:15 a2utils-0.0.9.data/scripts/a2conf
+-rwxr-xr-x  2.0 unx     3245 b- defN 20-Dec-06 17:15 a2utils-0.0.9.data/scripts/a2okerr
+-rwxr-xr-x  2.0 unx    13251 b- defN 20-Dec-07 15:49 a2utils-0.0.9.data/scripts/a2vhost
+-rw-r--r--  2.0 unx    14610 b- defN 20-Dec-07 15:49 a2utils-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 20-Dec-07 15:49 a2utils-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 20-Dec-07 15:49 a2utils-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      665 b- defN 20-Dec-07 15:49 a2utils-0.0.9.dist-info/RECORD
+8 files, 54876 bytes uncompressed, 16459 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: a2utils-0.0.8.data/scripts/a2certbot
+Filename: a2utils-0.0.9.data/scripts/a2certbot
 Comment: 
 
-Filename: a2utils-0.0.8.data/scripts/a2conf
+Filename: a2utils-0.0.9.data/scripts/a2conf
 Comment: 
 
-Filename: a2utils-0.0.8.data/scripts/a2okerr
+Filename: a2utils-0.0.9.data/scripts/a2okerr
 Comment: 
 
-Filename: a2utils-0.0.8.data/scripts/a2vhost
+Filename: a2utils-0.0.9.data/scripts/a2vhost
 Comment: 
 
-Filename: a2utils-0.0.8.dist-info/METADATA
+Filename: a2utils-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: a2utils-0.0.8.dist-info/WHEEL
+Filename: a2utils-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: a2utils-0.0.8.dist-info/top_level.txt
+Filename: a2utils-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: a2utils-0.0.8.dist-info/RECORD
+Filename: a2utils-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `a2utils-0.0.8.data/scripts/a2certbot` & `a2utils-0.0.9.data/scripts/a2certbot`

 * *Files identical despite different names*

## Comparing `a2utils-0.0.8.data/scripts/a2conf` & `a2utils-0.0.9.data/scripts/a2conf`

 * *Files identical despite different names*

## Comparing `a2utils-0.0.8.data/scripts/a2okerr` & `a2utils-0.0.9.data/scripts/a2okerr`

 * *Files identical despite different names*

## Comparing `a2utils-0.0.8.data/scripts/a2vhost` & `a2utils-0.0.9.data/scripts/a2vhost`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 
 from a2conf import Node
 import argparse
 import sys
 import subprocess
 import os
 
-class VhostNotFound(Exception):
+class MyException(Exception):
+    pass
+
+class VhostNotFound(MyException):
+    pass
+
+class ArgumentError(MyException):
     pass
 
 #
 # subroutines
 #
 def get_all_hostnames(vhost):
     names = list()
@@ -33,14 +39,17 @@
     raise VhostNotFound('Vhost args: {} host: {} not found'.format(arg, host))
     
 def get_vhconfig(apacheconfig, vhspec, domainlist):
     """
         return path to virtualhost apache config
     """
 
+    if not domainlist:
+        raise ArgumentError("Domain (-d) is required")
+
     root = Node(apacheconfig)
     root = Node(get_vhost_by_host(root, domainlist[0], vhspec).path)
     return root.path
 
 def guess_webroot(basename):
     prefixes = ['/var/www/virtual', '/var/www', '/usr/local/apache/htdocs', '/home/www/htdocs']
     for prefix in prefixes:
@@ -215,16 +224,15 @@
 
     vhost.args = vhost.args.replace(':80',':443')    
     root.write_file(root.path)
 
 def make_redirect(apacheconfig, domainlist):
     # sanity check 
     if not domainlist:
-        print("Specify at least one domain name: -d example.com")
-        sys.exit(1)
+        raise ArgumentError("Specify at least one domain name: -d example.com")
 
     # check maybe SSL host already exists
     root = Node(apacheconfig)
     for vhost in root.children('<VirtualHost>'):
         if not ':80' in vhost.args:
             continue
         vhnames = get_all_hostnames(vhost)
@@ -252,84 +260,95 @@
     new_vhost.insert('RewriteRule (.*) https://%{SERVER_NAME}$1 [R=301,L]')
 
     root.insert(['', '# auto-generated plain HTTP site for redirect', new_vhost], after=vhost)
     root.write_file(root.path)
 
 def add_directive(apacheconfig, vhconfig, domain, vhspec, directive):
     
-    if not domain:
-        print("Domain (-d) is required")
-        return
+    vhconfig = vhconfig or get_vhconfig(apacheconfig, vhspec, domain)
+    
+    root = Node(vhconfig)
+    vhost = get_vhost_by_host(root, domain[0],arg=vhspec)        
+    vhost.insert(directive)
+    root.write_file(root.path)
 
-    if not vhconfig:
-        try:
-            vhconfig = get_vhconfig(apacheconfig, vhspec, domain)
-        except VhostNotFound as e:
-            print("Error:", e)
-            return
+def rm_directive(apacheconfig, vhconfig, domain, vhspec, directive):
+    
+    try:
+        cmd, args = directive.split(' ', maxsplit=1)
+    except ValueError:
+        cmd = directive
+        args = None
 
+    vhconfig = vhconfig or get_vhconfig(apacheconfig, vhspec, domain)
+    
     root = Node(vhconfig)
-    for vhost in root.children('<VirtualHost>'):
-        if vhspec and vhspec not in vhost.args:
-            continue
-        
-        vhnames = get_all_hostnames(vhost)
-        
-        # filter by domain
-        if domain:
-            for d in domain:
-                if d not in vhnames:
-                    print("SKIP", vhost, vhnames, d)
-                    return
-        
-        vhost.insert(directive)
-        root.write_file(root.path)
-        return
-        
-def delete_vhost(apacheconfig, vhconfig, domain, vhspec):
-    if not domain:
-        print("Domain (-d) is required")
-        return
+    vhost = get_vhost_by_host(root, domain[0],arg=vhspec)        
+    
+    deleted = list()
+    for n in vhost.children(cmd):
+        if args:
+            if args==n.args:
+                deleted.append(n)
+        else:
+            deleted.append(n)
+    
+    for n in deleted:
+        print("removed:", n, n.args)
+        n.delete()
 
-    if not vhconfig:
-        try:
-            vhconfig = get_vhconfig(apacheconfig, vhspec, domain)
-        except VhostNotFound as e:
-            print("Error:", e)
-            return
+    root.write_file(root.path)
+
+def delete_vhost(apacheconfig, vhconfig, domain, vhspec):
 
+    vhconfig = vhconfig or get_vhconfig(apacheconfig, vhspec, domain)
     root = Node(vhconfig)
     vhost = get_vhost_by_host(root, domain[0],arg=vhspec)
     vhost.delete()
     root.write_file(root.path)
 
+def dump_vhost(apacheconfig, vhconfig, domain, vhspec):
+
+    vhconfig = vhconfig or get_vhconfig(apacheconfig, vhspec, domain)
+    
+    root = Node(vhconfig)
+    vhost = get_vhost_by_host(root, domain[0], arg=vhspec)
+    vhost.dump()
 
 def main():
 
     def_apacheconf = '/etc/apache2/apache2.conf'
 
     parser = argparse.ArgumentParser(description='Apache2 CLI vhost manager')
 
-    g = parser.add_argument_group('Commands')
+    g = parser.add_argument_group('Show vhost')
     g.add_argument('--list', default=False, action='store_true',
                    help='List VirtualHosts')
+    g.add_argument('--dump', default=False, action='store_true',
+                   help='Dump vhost content')
+
+    g = parser.add_argument_group('Manage vhosts')
+
     g.add_argument('--basic', default=False, action='store_true',
                    help='Create basic HTTP site (use: -c and --domain, --webroot)')
     g.add_argument('--convert', default=False, action='store_true',
                    help='Convert HTTP --domain site to HTTPS')
     g.add_argument('--redirect', default=False, action='store_true',
                    help='Create HTTP --domain redirect vhost to HTTPS')
     g.add_argument('--both', default=False, action='store_true',
                    help='Create both http/https sites and request certificate')
-
-    g.add_argument('--add', metavar='DIRECTIVE',
-                   help='Add custom apache configuration directive to vhost')
     g.add_argument('--delete', default=False, action='store_true',
                    help='Delete vhost (use -d, --vhost and (optionally) -c/-a')
 
+    g = parser.add_argument_group('Manage vhost configuration')
+    g.add_argument('--add', metavar='DIRECTIVE', 
+                   help='Add custom apache configuration directive to vhost')
+    g.add_argument('--rm', metavar='DIRECTIVE', 
+                   help='Remove custom apache configuration directive to vhost')
+
     g = parser.add_argument_group('Options')
     g.add_argument('-a', '--apacheconfig', default=def_apacheconf, metavar='CONF',
                    help='Main apache config file. def: {}'.format(None))
     g.add_argument('-c', '--config', default=None, metavar='VHOST_CONF',
                    help='VirtualHost config file.')
     g.add_argument('-w', '--webroot', default=None, metavar='PATH',
                    help='Webroot (DocumentRoot) for new site')
@@ -337,23 +356,34 @@
     g.add_argument('--vhost', metavar='VHOST', help='Process only this vhost (e.g. *:80)')
     g.add_argument('--auto', default=False, action='store_true', help='Autogenerate/guess missing params " \
         "(config file name, create missing directories)')
 
 
     args = parser.parse_args()
 
-    if args.list:
-        list_vhosts(args.apacheconfig)
-    elif args.both:
-        make_both(args.apacheconfig, args.config,  args.domain, args.webroot, args.auto)
-    elif args.basic:
-        make_basic(args.apacheconfig, args.config,  args.domain, args.webroot, args.auto)
-    elif args.convert:
-        make_convert(args.apacheconfig, args.domain)
-    elif args.redirect:
-        make_redirect(args.apacheconfig, args.domain)
-    elif args.add:
-        add_directive(args.apacheconfig, args.config, args.domain, args.vhost, args.add)
-    elif args.delete:
-        delete_vhost(args.apacheconfig, args.config, args.domain, args.vhost)
+    try:
+        if args.list:
+            list_vhosts(args.apacheconfig)
+        elif args.dump:
+            dump_vhost(args.apacheconfig, args.config, args.domain, args.vhost)
+
+        elif args.basic:
+            make_basic(args.apacheconfig, args.config,  args.domain, args.webroot, args.auto)
+        elif args.both:
+            make_both(args.apacheconfig, args.config,  args.domain, args.webroot, args.auto)
+        elif args.convert:
+            make_convert(args.apacheconfig, args.domain)
+        elif args.redirect:
+            make_redirect(args.apacheconfig, args.domain)
+        elif args.delete:
+            delete_vhost(args.apacheconfig, args.config, args.domain, args.vhost)
+
+        elif args.add:
+            add_directive(args.apacheconfig, args.config, args.domain, args.vhost, args.add)
+        elif args.rm:
+            rm_directive(args.apacheconfig, args.config, args.domain, args.vhost, args.rm)
+
+    except (MyException) as e:
+        print("Error:", e)
+        return
 
 main()
```

## Comparing `a2utils-0.0.8.dist-info/METADATA` & `a2utils-0.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a2utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: apache2 config file utilities
 Home-page: https://github.com/yaroslaff/a2utils
 Author: Yaroslav Polyakov
 Author-email: yaroslaff@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

