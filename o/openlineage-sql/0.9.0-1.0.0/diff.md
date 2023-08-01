# Comparing `tmp/openlineage_sql-0.9.0.tar.gz` & `tmp/openlineage_sql-1.0.0.tar.gz`

## Comparing `openlineage_sql-0.9.0.tar` & `openlineage_sql-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,42 @@
--rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 openlineage_sql-0.9.0/Cargo.toml
--rw-rw-r--   0     1001     1002       51 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/README.md
--rw-rw-r--   0     1001     1002       71 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/build.rs
--rw-rw-r--   0     1001     1002      324 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/pyproject.toml
--rw-rw-r--   0     1001     1002       13 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/requirements.txt
--rw-rw-r--   0     1001     1002     1147 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/script/build.sh
--rw-rw-r--   0     1001     1002      699 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/src/bigquery.rs
--rw-rw-r--   0     1001     1002    15937 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/src/lib.rs
--rw-rw-r--   0     1001     1002      180 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/tests/python/test_small.py
--rw-rw-r--   0     1001     1002     1130 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/tests/test_utils/mod.rs
--rw-rw-r--   0     1001     1002     1400 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/tests/tests_copy.rs
--rw-rw-r--   0     1001     1002     1417 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/tests/tests_create.rs
--rw-rw-r--   0     1001     1002     5160 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/tests/tests_cte.rs
--rw-rw-r--   0     1001     1002    16087 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/tests/tests_insert.rs
--rw-rw-r--   0     1001     1002     1994 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/tests/tests_merge.rs
--rw-rw-r--   0     1001     1002     2243 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/tests/tests_select.rs
--rw-rw-r--   0     1001     1002    34252 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/tests/tests_tpcds.rs
--rw-rw-r--   0     1001     1002     1264 2022-06-03 23:03:15.000000 openlineage_sql-0.9.0/tests/tests_update.rs
--rw-r--r--   0        0        0      615 1970-01-01 00:00:00.000000 openlineage_sql-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      580 1970-01-01 00:00:00.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/Cargo.toml
+-rw-rw-r--   0     1001     1002      704 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/src/bigquery.rs
+-rw-rw-r--   0     1001     1002     1006 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/src/context/alias_table.rs
+-rw-rw-r--   0     1001     1002    16376 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/src/context/mod.rs
+-rw-rw-r--   0     1001     1002     1700 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/src/dialect.rs
+-rw-rw-r--   0     1001     1002     2776 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/src/lib.rs
+-rw-rw-r--   0     1001     1002     4466 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/src/lineage.rs
+-rw-rw-r--   0     1001     1002    22418 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/src/visitor.rs
+-rw-rw-r--   0     1001     1002      189 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/column_lineage/mod.rs
+-rw-rw-r--   0     1001     1002     3999 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/column_lineage/tests_aliases.rs
+-rw-rw-r--   0     1001     1002     1119 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/column_lineage/tests_cte.rs
+-rw-rw-r--   0     1001     1002     2149 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/column_lineage/tests_select.rs
+-rw-rw-r--   0     1001     1002     8992 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/column_lineage/tests_simple.rs
+-rw-rw-r--   0     1001     1002      389 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/table_lineage/mod.rs
+-rw-rw-r--   0     1001     1002     1140 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/table_lineage/tests_alter.rs
+-rw-rw-r--   0     1001     1002     3925 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/table_lineage/tests_copy.rs
+-rw-rw-r--   0     1001     1002     5193 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/table_lineage/tests_create.rs
+-rw-rw-r--   0     1001     1002     5546 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/table_lineage/tests_cte.rs
+-rw-rw-r--   0     1001     1002      909 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/table_lineage/tests_delete.rs
+-rw-rw-r--   0     1001     1002      431 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/table_lineage/tests_drop.rs
+-rw-rw-r--   0     1001     1002     1608 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/table_lineage/tests_error_handling.rs
+-rw-rw-r--   0     1001     1002    17518 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/table_lineage/tests_insert.rs
+-rw-rw-r--   0     1001     1002     2199 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/table_lineage/tests_merge.rs
+-rw-rw-r--   0     1001     1002     3438 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/table_lineage/tests_select.rs
+-rw-rw-r--   0     1001     1002    34761 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/table_lineage/tests_tpcds.rs
+-rw-rw-r--   0     1001     1002      392 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/table_lineage/tests_truncate.rs
+-rw-rw-r--   0     1001     1002     1530 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/table_lineage/tests_update.rs
+-rw-rw-r--   0     1001     1002     1001 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/test_utils/mod.rs
+-rw-rw-r--   0     1001     1002      158 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/tests.rs
+-rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 openlineage_sql-1.0.0/Cargo.toml
+-rw-rw-r--   0     1001     1002      174 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/build.rs
+-rw-rw-r--   0     1001     1002     1660 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/openlineage_sql.pyi
+-rw-rw-r--   0     1001     1002      316 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/pyproject.toml
+-rw-rw-r--   0     1001     1002       13 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/requirements.txt
+-rwxrwxr-x   0     1001     1002     1438 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/script/build-macos.sh
+-rwxrwxr-x   0     1001     1002     1341 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/script/build.sh
+-rwxrwxr-x   0     1001     1002     1142 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/script/setup-macos.sh
+-rw-rw-r--   0     1001     1002    11136 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/src/lib.rs
+-rw-rw-r--   0     1001     1002     2381 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/tests/python/sql_tester.py
+-rw-rw-r--   0     1001     1002      281 2023-08-01 19:45:59.000000 openlineage_sql-1.0.0/tests/python/test_small.py
+-rw-r--r--   0        0        0    11943 2023-08-01 19:46:50.000000 openlineage_sql-1.0.0/Cargo.lock
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 openlineage_sql-1.0.0/PKG-INFO
```

### Comparing `openlineage_sql-0.9.0/script/build.sh` & `openlineage_sql-1.0.0/script/build.sh`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 #!/usr/bin/env bash
-# SPDX-License-Identifier: Apache-2.0.
-
-
+#
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
+#
 # Build script for OpenLineage SQL parser.
 # It's assumed that it will be run in manylinux image: see https://github.com/pypa/manylinux
 set -e
 
 # Manylinux image has multiple "pythons" - in /opt/python directory.
-# We use Python 3.7, since it's the lowest we want to use
+# We use Python 3.8, since it's the lowest we want to use
 # and create local virtualenv - it's easier to proceed in venv than use python behind long absolute path
-/opt/python/cp37-cp37m/bin/python -m venv .env
+/opt/python/cp38-cp38/bin/python -m venv .env
 source .env/bin/activate
 
 # Maturin is build tool that we're using. It can build python wheels based on standard Rust Cargo.toml.
 python -m pip install maturin
 
 # Install Rust
 curl https://sh.rustup.rs -sSf | sh -s -- -y
 source $HOME/.cargo/env
 
 # Disable incremental compilation, since it causes issues.
 export CARGO_INCREMENTAL=0
 
 # Run test if indicated to do so.
-if [[ -z ${RUN_TESTS} ]]; then
+if [[ $RUN_TESTS = true ]]; then
   cargo test --no-default-features
+  cargo clippy --all-targets --all-features -- -D warnings
+  cargo fmt -- --check
 fi
 
 # Build release wheels
-maturin build --out target/wheels
+cd iface-py
+maturin build --sdist --out target/wheels --release --strip
 
 # Verify that it imports properly
-pip install openlineage-sql --no-index --find-links target/wheels --force-reinstall
+python -m pip install openlineage-sql --no-index --find-links target/wheels --force-reinstall
 python -c "import openlineage_sql"
 echo "all good"
```

### Comparing `openlineage_sql-0.9.0/tests/tests_cte.rs` & `openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/table_lineage/tests_cte.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-extern crate core;
+// Copyright 2018-2023 contributors to the OpenLineage project
+// SPDX-License-Identifier: Apache-2.0
 
-use openlineage_sql::{parse_sql, SqlMeta};
+use crate::test_utils::*;
+use openlineage_sql::{parse_sql, ExtractionError, TableLineage};
 use sqlparser::dialect::PostgreSqlDialect;
-use std::sync::Arc;
-
-#[macro_use]
-mod test_utils;
-use test_utils::*;
 
 #[test]
 fn parse_simple_cte() {
     assert_eq!(
         test_sql(
             "
                 WITH sum_trans as (
@@ -20,43 +17,47 @@
                     GROUP BY user_id
                 )
                 INSERT INTO potential_fraud (user_id, cnt, balance)
                 SELECT user_id, cnt, balance
                     FROM sum_trans
                     WHERE count > 1000 OR balance > 100000;
                 ",
-        ),
-        SqlMeta {
-            in_tables: table("transactions"),
-            out_tables: table("potential_fraud")
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
+            in_tables: tables(vec!["transactions"]),
+            out_tables: tables(vec!["potential_fraud"])
         }
     );
 }
 
 #[test]
 fn parse_bugged_cte() {
-    assert_eq!(
-        parse_sql(
-            "
-                WITH sum_trans (
-                    SELECT user_id, COUNT(*) as cnt, SUM(amount) as balance
-                    FROM transactions
-                    WHERE created_date > '2020-01-01'
-                    GROUP BY user_id
-                )
-                INSERT INTO potential_fraud (user_id, cnt, balance)
-                SELECT user_id, cnt, balance
-                FROM sum_trans
-                WHERE count > 1000 OR balance > 100000;",
-            Arc::new(PostgreSqlDialect {}),
-            None
+    let sql = "
+        WITH sum_trans (
+            SELECT user_id, COUNT(*) as cnt, SUM(amount) as balance
+            FROM transactions
+            WHERE created_date > '2020-01-01'
+            GROUP BY user_id
         )
-        .unwrap_err(),
-        "sql parser error: Expected ), found: user_id"
-    )
+        INSERT INTO potential_fraud (user_id, cnt, balance)
+        SELECT user_id, cnt, balance
+        FROM sum_trans
+        WHERE count > 1000 OR balance > 100000;";
+    let meta = parse_sql(sql, &PostgreSqlDialect {}, None).unwrap();
+    assert_eq!(meta.errors.len(), 1);
+    assert_eq!(
+        meta.errors.get(0).unwrap(),
+        &ExtractionError {
+            index: 0,
+            message: "Expected ), found: user_id".to_string(),
+            origin_statement: sql.to_string(),
+        }
+    );
 }
 
 #[test]
 fn parse_recursive_cte() {
     assert_eq!(
         test_sql(
             "
@@ -70,37 +71,44 @@
                 e.manager_id,
                 e.full_name
             FROM employees e
             INNER JOIN subordinates s ON s.employee_id = e.manager_id)
             INSERT INTO sub_employees (employee_id, manager_id, full_name)
             SELECT employee_id, manager_id, full_name FROM subordinates;
         "
-        ),
-        SqlMeta {
-            in_tables: table("employees"),
-            out_tables: table("sub_employees")
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
+            in_tables: tables(vec!["employees"]),
+            out_tables: tables(vec!["sub_employees"])
         }
     )
 }
 
 #[test]
 fn multiple_ctes() {
     assert_eq!(
-        test_sql("
+        test_sql(
+            "
             WITH customers AS (
                 SELECT * FROM DEMO_DB.public.stg_customers
             ),
             orders AS (
                 SELECT * FROM DEMO_DB.public.stg_orders
             )
             SELECT *
             FROM customers c
             JOIN orders o
             ON c.id = o.customer_id
-        "), SqlMeta {
+        "
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: tables(vec![
                 "DEMO_DB.public.stg_customers",
                 "DEMO_DB.public.stg_orders"
             ]),
             out_tables: vec![]
         }
     )
@@ -174,14 +182,16 @@
               AND grps.started = tps.started
             GROUP BY
               grps.p_i,
               grps.u_i,
               grps.uk,
               grps.grp
         "
-        ),
-        SqlMeta {
-            in_tables: table("d_n.f_p_s"),
-            out_tables: table("dev_d_n.f_p_s_m")
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
+            in_tables: tables(vec!["d_n.f_p_s"]),
+            out_tables: tables(vec!["dev_d_n.f_p_s_m"])
         }
     )
 }
```

### Comparing `openlineage_sql-0.9.0/tests/tests_insert.rs` & `openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/table_lineage/tests_insert.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,48 @@
-use openlineage_sql::SqlMeta;
+// Copyright 2018-2023 contributors to the OpenLineage project
+// SPDX-License-Identifier: Apache-2.0
 
-#[macro_use]
-mod test_utils;
-use test_utils::*;
+use crate::test_utils::*;
+use openlineage_sql::TableLineage;
 
 #[test]
 fn insert_values() {
     assert_eq!(
-        test_sql("INSERT INTO TEST VALUES(1)",),
-        SqlMeta {
+        test_sql("INSERT INTO TEST VALUES(1)",)
+            .unwrap()
+            .table_lineage,
+        TableLineage {
             in_tables: vec![],
-            out_tables: table("TEST")
+            out_tables: tables(vec!["TEST"])
         }
     );
 }
 
 #[test]
 fn insert_cols_values() {
     assert_eq!(
-        test_sql("INSERT INTO tbl(col1, col2) VALUES (1, 2), (2, 3)",),
-        SqlMeta {
+        test_sql("INSERT INTO tbl(col1, col2) VALUES (1, 2), (2, 3)",)
+            .unwrap()
+            .table_lineage,
+        TableLineage {
             in_tables: vec![],
-            out_tables: table("tbl")
+            out_tables: tables(vec!["tbl"])
         }
     );
 }
 
 #[test]
 fn insert_select_table() {
     assert_eq!(
-        test_sql("INSERT INTO TEST SELECT * FROM TEMP",),
-        SqlMeta {
-            in_tables: table("TEMP"),
-            out_tables: table("TEST")
+        test_sql("INSERT INTO TEST SELECT * FROM TEMP",)
+            .unwrap()
+            .table_lineage,
+        TableLineage {
+            in_tables: tables(vec!["TEMP"]),
+            out_tables: tables(vec!["TEST"])
         }
     );
 }
 
 #[test]
 fn insert_select_table_2() {
     assert_eq!(
@@ -48,39 +54,52 @@
                    P,
                    count(*)
             from \"b1\".\"b2\" as s
                      left join \"m\".\"dim\" as dm on (dm.m_id = s.m_id)
             where PROCESSED_AT = '2022-04-14'
             group by to_date(C_AT), dm.C_NAME, P
             ;",
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: tables(vec!["b1.b2", "m.dim"]),
-            out_tables: table("a1.a2")
+            out_tables: tables(vec!["a1.a2"])
         }
     )
 }
 
 #[test]
 fn insert_nested_select() {
     assert_eq!(test_sql("
                 INSERT INTO popular_orders_day_of_week (order_day_of_week, order_placed_on,orders_placed)
                 SELECT EXTRACT(ISODOW FROM order_placed_on) AS order_day_of_week,
                     order_placed_on,
                     COUNT(*) AS orders_placed
                 FROM top_delivery_times
                 GROUP BY order_placed_on;
             ",
-    ), SqlMeta {
-        in_tables: table("top_delivery_times"),
-        out_tables: table("popular_orders_day_of_week")
+    ).unwrap().table_lineage, TableLineage {
+        in_tables: tables(vec!["top_delivery_times"]),
+        out_tables: tables(vec!["popular_orders_day_of_week"])
     })
 }
 
 #[test]
+fn insert_snowflake_table() {
+    assert_eq!(
+        test_sql_dialect("\n    INSERT INTO test_orders (ord, str, num) VALUES\n    (1, 'b', 15),\n    (2, 'a', 21),\n    (3, 'b', 7);\n   ", "snowflake").unwrap().table_lineage,
+        TableLineage {
+            in_tables: vec![],
+            out_tables: tables(vec!["test_orders"])
+        }
+    )
+}
+
+#[test]
 fn insert_overwrite_table() {
     assert_eq!(
         test_sql(
             "\
         INSERT OVERWRITE TABLE schema.dps
         PARTITION (ds = '2022-03-30')
         SELECT
@@ -97,18 +116,20 @@
         WHERE ds = '2022-03-30'
             AND UNIX_TIMESTAMP(stopped) - UNIX_TIMESTAMP(joined) BETWEEN 0 AND 28800
         GROUP BY
             pid,
             uid,
             pii_userid
     "
-        ),
-        SqlMeta {
-            in_tables: table("schema.fpsm"),
-            out_tables: table("schema.dps")
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
+            in_tables: tables(vec!["schema.fpsm"]),
+            out_tables: tables(vec!["schema.dps"])
         }
     )
 }
 
 #[test]
 fn insert_overwrite_subqueries() {
     assert_eq!(
@@ -116,18 +137,20 @@
             "
         INSERT OVERWRITE TABLE mytable
         PARTITION (ds = '2022-03-31')
         SELECT
             *
         FROM
         (SELECT * FROM table2) a"
-        ),
-        SqlMeta {
-            in_tables: table("table2"),
-            out_tables: table("mytable")
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
+            in_tables: tables(vec!["table2"]),
+            out_tables: tables(vec!["mytable"])
         }
     )
 }
 
 #[test]
 fn insert_overwrite_multiple_subqueries() {
     assert_eq!(
@@ -140,18 +163,20 @@
         FROM
         (SELECT * FROM table2
          UNION
          SELECT * FROM table3
          UNION ALL
          SELECT * FROM table4) a
          "
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: tables(vec!["table2", "table3", "table4"]),
-            out_tables: table("mytable")
+            out_tables: tables(vec!["mytable"])
         }
     )
 }
 
 #[test]
 fn insert_overwrite_partition() {
     assert_eq!(
@@ -166,35 +191,39 @@
                 (SELECT * FROM d_d_n.u_t_250 WHERE ds = '2022-02-24') u
             JOIN
                 (SELECT * FROM d_n_p.g_d_r WHERE ds = '2022-02-24') g
             ON
                 u.u_i = g.u_i
         ",
             "hive"
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: tables(vec!["d_d_n.u_t_250", "d_n_p.g_d_r"]),
-            out_tables: table("d_d_n.g_d_t_r")
+            out_tables: tables(vec!["d_d_n.g_d_t_r"])
         }
     )
 }
 
 #[test]
 fn set_before_insert() {
     assert_eq!(
         test_sql_dialect(
             "
                 SET hive.something=false;
                 INSERT INTO TABLE a.b.c VALUES (1, 2, 3);
             ",
             "hive"
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: vec![],
-            out_tables: table("a.b.c")
+            out_tables: tables(vec!["a.b.c"])
         }
     )
 }
 
 #[test]
 fn insert_overwrite_hive_sets_large() {
     assert_eq!(
@@ -217,18 +246,20 @@
                            WHERE fpsm.ds = '2022-05-01'
                            GROUP BY
                                fpsm.p_id
                         ) AS T2
                         ON T1.p_id = T2.p_id
         ",
             "hive"
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: tables(vec!["d_p.f_p_s", "d_p.f_p_s_merged"]),
-            out_tables: table("d_d_p.d_f_s")
+            out_tables: tables(vec!["d_d_p.d_f_s"])
         }
     )
 }
 
 #[test]
 fn insert_group_by() {
     assert_eq!(
@@ -252,18 +283,20 @@
               C_DT,
               C_NAME,
               U_C,
               U_M,
               U_SOURCE,
               P,
               U_SOURCE;"
-        ),
-        SqlMeta {
-            in_tables: table("b1.b2"),
-            out_tables: table("a1.a2")
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
+            in_tables: tables(vec!["b1.b2"]),
+            out_tables: tables(vec!["a1.a2"])
         }
     )
 }
 
 #[test]
 fn insert_nested_with_select() {
     assert_eq!(
@@ -366,48 +399,54 @@
           count(distinct user_id)
         from
           a_b_c
         group by
           created_dt,
           region,
           x;"
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: tables(vec!["b1.b2", "c1.c2", "d1.d2", "e1.e2", "f1.f2"]),
-            out_tables: table("a1.a2")
+            out_tables: tables(vec!["a1.a2"])
         }
     )
 }
 
 #[test]
 fn test_multiple_statements_delete_insert() {
     assert_eq!(
         test_sql(
             "
             DELETE FROM public.\"Employees\";
             INSERT INTO public.\"Employees\" VALUES (1, 'TALES OF SHIVA', 'Mark', 'mark', 0);
         "
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: vec![],
-            out_tables: table("public.\"Employees\""),
+            out_tables: tables(vec!["public.\"Employees\""]),
         }
     )
 }
 
 #[test]
 fn test_multiple_statements_insert_insert() {
     assert_eq!(
         test_sql(
             "
             INSERT INTO a.a VALUES(1,2);
             INSERT INTO b.b VALUES(1,2);
         "
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: vec![],
             out_tables: tables(vec!["a.a", "b.b"]),
         }
     )
 }
 
 #[test]
@@ -415,17 +454,19 @@
     assert_eq!(
         test_sql(
             "
             INSERT INTO a.a VALUES(1,2);
             INSERT INTO b.b SELECT * FROM a.a;
             INSERT INTO c.c VALUES(1,2);
         "
-        ),
-        SqlMeta {
-            in_tables: table("a.a"),
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
+            in_tables: tables(vec!["a.a"]),
             out_tables: tables(vec!["a.a", "b.b", "c.c"]),
         }
     )
 }
 
 #[test]
 fn insert_overwrite_multiple_unions() {
@@ -479,18 +520,20 @@
                     ds = '2022-04-03'
                     AND l_a_d >= DATE_ADD('2022-05-01', -56)
                 ) sub
             GROUP BY
                 sub.p_i,
                 sub.u_i
         "
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: tables(vec!["d_d_n.a_p_s_v", "d_d_n.d_p_s_v"]),
-            out_tables: table("d_d_n.a_p_s_v")
+            out_tables: tables(vec!["d_d_n.a_p_s_v"])
         }
     )
 }
 
 #[test]
 fn insert_overwrite_partition_dates() {
     assert_eq!(
@@ -609,14 +652,16 @@
                 AND lad >= DATE_ADD('2022-05-01', -56)
             ) sub
         GROUP BY
             sub.pid,
             sub.uid,
             sub.userkey
         "
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: tables(vec!["ddw.aps2", "ddw.dps"]),
-            out_tables: table("ddw.aps2")
+            out_tables: tables(vec!["ddw.aps2"])
         }
     )
 }
```

### Comparing `openlineage_sql-0.9.0/tests/tests_select.rs` & `openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/table_lineage/tests_select.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,48 @@
-use openlineage_sql::{parse_sql, BigQueryDialect, SqlMeta};
-use std::sync::Arc;
+// Copyright 2018-2023 contributors to the OpenLineage project
+// SPDX-License-Identifier: Apache-2.0
 
-#[macro_use]
-mod test_utils;
-use test_utils::*;
+use crate::test_utils::*;
+use openlineage_sql::{parse_sql, BigQueryDialect, TableLineage};
 
 #[test]
 fn select_simple() {
     assert_eq!(
-        test_sql("SELECT * FROM table0;",),
-        SqlMeta {
-            in_tables: table("table0"),
+        test_sql("SELECT * FROM table0;",).unwrap().table_lineage,
+        TableLineage {
+            in_tables: tables(vec!["table0"]),
             out_tables: vec![]
         }
     )
 }
 #[test]
 fn select_from_schema_table() {
     assert_eq!(
-        test_sql("SELECT * FROM schema0.table0;",),
-        SqlMeta {
-            in_tables: table("schema0.table0"),
+        test_sql("SELECT * FROM schema0.table0;",)
+            .unwrap()
+            .table_lineage,
+        TableLineage {
+            in_tables: tables(vec!["schema0.table0"]),
             out_tables: vec![]
         }
     )
 }
 #[test]
 fn select_join() {
     assert_eq!(
         test_sql(
             "
                 SELECT col0, col1, col2
                 FROM table0
                 JOIN table1
                 ON t1.col0 = t2.col0",
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: tables(vec!["table0", "table1"]),
             out_tables: vec![]
         }
     )
 }
 
 #[test]
@@ -47,16 +50,18 @@
     assert_eq!(
         test_sql(
             "
                 SELECT col0, col1, col2
                 FROM table0
                 INNER JOIN table1
                 ON t1.col0 = t2.col0",
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: tables(vec!["table0", "table1"]),
             out_tables: vec![]
         }
     )
 }
 
 #[test]
@@ -64,16 +69,18 @@
     assert_eq!(
         test_sql(
             "
             SELECT col0, col1, col2
             FROM table0
             LEFT JOIN table1
             ON t1.col0 = t2.col0",
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: tables(vec!["table0", "table1"]),
             out_tables: vec![]
         }
     )
 }
 
 #[test]
@@ -81,28 +88,63 @@
     assert_eq!(
         parse_sql(
             "
             SELECT *
             FROM `random-project`.`dbt_test1`.`source_table`
             WHERE id = 1
             ",
-            Arc::new(BigQueryDialect),
+            &BigQueryDialect,
             None
         )
-        .unwrap(),
-        SqlMeta {
-            in_tables: table("random-project.dbt_test1.source_table"),
+        .unwrap()
+        .table_lineage,
+        TableLineage {
+            in_tables: tables(vec!["random-project.dbt_test1.source_table"]),
             out_tables: vec![]
         }
     )
 }
 
 #[test]
 fn select_into() {
     assert_eq!(
-        test_sql("SELECT * INTO table0 FROM table1;",),
-        SqlMeta {
-            in_tables: table("table1"),
-            out_tables: table("table0")
+        test_sql("SELECT * INTO table0 FROM table1;",)
+            .unwrap()
+            .table_lineage,
+        TableLineage {
+            in_tables: tables(vec!["table1"]),
+            out_tables: tables(vec!["table0"])
+        }
+    )
+}
+
+#[test]
+fn select_redshift() {
+    assert_eq!(
+        test_sql_dialect("SELECT [col1] FROM [test_schema].[test_table]", "redshift")
+            .unwrap()
+            .table_lineage,
+        TableLineage {
+            in_tables: tables(vec!["test_schema.test_table"]),
+            out_tables: vec![]
+        }
+    )
+}
+
+#[test]
+fn select_with_table_generator() {
+    assert_eq!(
+        test_sql(
+            "
+            SELECT row_number() OVER (ORDER BY col) row_num, d
+            FROM TABLE(GENERATOR(ROWCOUNT => (12 * 6)))
+            JOIN test_schema.test_table ON test_table.d = row_number()
+            "
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
+            in_tables: tables(vec!["test_schema.test_table"]),
+            out_tables: vec![]
         }
     )
 }
```

### Comparing `openlineage_sql-0.9.0/tests/tests_tpcds.rs` & `openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/table_lineage/tests_tpcds.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-use openlineage_sql::SqlMeta;
+// Copyright 2018-2023 contributors to the OpenLineage project
+// SPDX-License-Identifier: Apache-2.0
 
-#[macro_use]
-mod test_utils;
-use test_utils::*;
+use crate::test_utils::*;
+use openlineage_sql::TableLineage;
 
 #[test]
 fn test_tpcds_cte_query() {
     assert_eq!(test_sql("
             WITH year_total AS
                 (SELECT c_customer_id customer_id,
                         c_first_name customer_first_name,
@@ -77,15 +77,15 @@
                     END
                 ORDER  BY t_s_secyear.customer_id,
                         t_s_secyear.customer_first_name,
                         t_s_secyear.customer_last_name,
                         t_s_secyear.customer_preferred_cust_flag
             LIMIT 100;
             ",
-    ), SqlMeta {
+    ).unwrap().table_lineage, TableLineage {
         in_tables: tables(vec![
             "date_dim",
             "store_sales",
             "src.customer",
         ]),
         out_tables: vec![],
     })
@@ -114,16 +114,18 @@
                                         FROM   customer_total_return ctr2
                                         WHERE  ctr1.ctr_store_sk = ctr2.ctr_store_sk)
                AND s_store_sk = ctr1.ctr_store_sk
                AND s_state = 'TN'
                AND ctr1.ctr_customer_sk = c_customer_sk
         ORDER  BY c_customer_id
         LIMIT 100;",
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: tables(vec!["customer", "date_dim", "store", "store_returns",]),
             out_tables: vec![]
         }
     )
 }
 
 #[test]
@@ -205,16 +207,18 @@
                    sat_sales         sat_sales2
             FROM   wswscs,
                    date_dim
             WHERE  date_dim.d_week_seq = wswscs.d_week_seq
                    AND d_year = 1998 + 1) z
     WHERE  d_week_seq1 = d_week_seq2 - 53
     ORDER  BY d_week_seq1;",
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: tables(vec!["catalog_sales", "date_dim", "web_sales",]),
             out_tables: vec![]
         }
     )
 }
 
 #[test]
@@ -237,16 +241,18 @@
                   item.i_brand,
                   item.i_brand_id
         ORDER  BY dt.d_year,
                   sum_agg DESC,
                   brand_id
         LIMIT 100;
         ",
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: tables(vec!["date_dim", "item", "store_sales",]),
             out_tables: vec![]
         }
     )
 }
 
 #[test]
@@ -402,16 +408,18 @@
                          END
         ORDER  BY t_s_secyear.customer_id,
                   t_s_secyear.customer_first_name,
                   t_s_secyear.customer_last_name,
                   t_s_secyear.customer_preferred_cust_flag
         LIMIT 100;
         ",
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: tables(vec![
                 "catalog_sales",
                 "customer",
                 "date_dim",
                 "store_sales",
                 "web_sales"
             ]),
@@ -545,15 +553,15 @@
                                    returns1 ,
                                    (profit - profit_loss) AS profit
                             FROM   wsr ) x
             GROUP BY rollup (channel, id)
             ORDER BY channel ,
                      id
             LIMIT 100; ",
-    ), SqlMeta {
+    ).unwrap().table_lineage, TableLineage {
         in_tables: tables(vec![
             "catalog_page",
             "catalog_returns",
             "catalog_sales",
             "date_dim",
             "store",
             "store_returns",
@@ -590,16 +598,18 @@
                                               FROM   item j
                                               WHERE  j.i_category = i.i_category)
         GROUP  BY a.ca_state
         HAVING Count(*) >= 10
         ORDER  BY cnt
         LIMIT 100;
     ",
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: tables(vec![
                 "customer",
                 "customer_address",
                 "date_dim",
                 "item",
                 "store_sales",
             ]),
@@ -633,16 +643,18 @@
                AND ( p_channel_email = 'N'
                       OR p_channel_event = 'N' )
                AND d_year = 1998
         GROUP  BY i_item_id
         ORDER  BY i_item_id
         LIMIT 100;
     ",
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: tables(vec![
                 "customer_demographics",
                 "date_dim",
                 "item",
                 "promotion",
                 "store_sales",
             ]),
@@ -695,16 +707,18 @@
                AND d_qoy = 2
                AND d_year = 2000
                AND ( Substr(s_zip, 1, 2) = Substr(V1.ca_zip, 1, 2) )
         GROUP  BY s_store_name
         ORDER  BY s_store_name
         LIMIT 100;
     ",
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: tables(vec![
                 "customer",
                 "customer_address",
                 "date_dim",
                 "store",
                 "store_sales",
             ]),
@@ -777,14 +791,16 @@
                  ELSE (SELECT Avg(ss_net_profit)
                        FROM   store_sales
                        WHERE  ss_quantity BETWEEN 81 AND 100)
                END bucket5
         FROM   reason
         WHERE  r_reason_sk = 1;
     ",
-        ),
-        SqlMeta {
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
             in_tables: tables(vec!["reason", "store_sales"]),
             out_tables: vec![]
         }
     )
 }
```

### Comparing `openlineage_sql-0.9.0/tests/tests_update.rs` & `openlineage_sql-1.0.0/local_dependencies/openlineage_sql/tests/table_lineage/tests_update.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,57 @@
-use openlineage_sql::SqlMeta;
+// Copyright 2018-2023 contributors to the OpenLineage project
+// SPDX-License-Identifier: Apache-2.0
 
-#[macro_use]
-mod test_utils;
-use test_utils::*;
+use crate::test_utils::*;
+use openlineage_sql::TableLineage;
 
 #[test]
 fn update_table() {
     assert_eq!(
-        test_sql("UPDATE table0 SET col0 = val0 WHERE col1 = val1"),
-        SqlMeta {
+        test_sql("UPDATE table0 SET col0 = val0 WHERE col1 = val1")
+            .unwrap()
+            .table_lineage,
+        TableLineage {
             in_tables: vec![],
-            out_tables: table("table0")
+            out_tables: tables(vec!["table0"])
         }
     );
 }
 
 #[test]
 fn update_table_from() {
     assert_eq!(
         test_sql(
             "UPDATE dataset.Inventory i
             SET quantity = i.quantity + n.quantity,
                 supply_constrained = false
             FROM dataset.NewArrivals n
             WHERE i.product = n.product"
-        ),
-        SqlMeta {
-            in_tables: table("dataset.NewArrivals"),
-            out_tables: table("dataset.Inventory")
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
+            in_tables: tables(vec!["dataset.NewArrivals"]),
+            out_tables: tables(vec!["dataset.Inventory"])
         }
     )
 }
 
 #[test]
 fn update_table_from_subquery() {
     assert_eq!(
         test_sql(
             "UPDATE dataset.Inventory
             SET quantity = quantity +
             (SELECT quantity FROM dataset.NewArrivals
             WHERE Inventory.product = NewArrivals.product),
             supply_constrained = false
             WHERE product IN (SELECT product FROM dataset.NewArrivals)"
-        ),
-        SqlMeta {
-            in_tables: table("dataset.NewArrivals"),
-            out_tables: table("dataset.Inventory")
+        )
+        .unwrap()
+        .table_lineage,
+        TableLineage {
+            in_tables: tables(vec!["dataset.NewArrivals"]),
+            out_tables: tables(vec!["dataset.Inventory"])
         }
     )
 }
```

