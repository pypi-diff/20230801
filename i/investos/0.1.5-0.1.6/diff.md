# Comparing `tmp/investos-0.1.5.tar.gz` & `tmp/investos-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investos-0.1.5.tar", max compression
+gzip compressed data, was "investos-0.1.6.tar", max compression
```

## Comparing `investos-0.1.5.tar` & `investos-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0    20869 2023-04-03 18:29:49.638655 investos-0.1.5/LICENSE
--rw-r--r--   0        0        0      803 2023-07-18 21:12:06.647068 investos-0.1.5/README.md
--rw-r--r--   0        0        0       49 2023-07-20 19:52:49.628775 investos-0.1.5/investos/__init__.py
--rw-r--r--   0        0        0      238 2023-07-19 05:16:44.131001 investos-0.1.5/investos/portfolio/__init__.py
--rw-r--r--   0        0        0      337 2023-07-19 05:16:44.131177 investos-0.1.5/investos/portfolio/constraint_model/__init__.py
--rw-r--r--   0        0        0      557 2023-07-19 05:16:44.131684 investos-0.1.5/investos/portfolio/constraint_model/base_constraint.py
--rw-r--r--   0        0        0     1372 2023-07-19 05:16:44.131849 investos-0.1.5/investos/portfolio/constraint_model/leverage_constraint.py
--rw-r--r--   0        0        0     2660 2023-07-19 05:16:44.132122 investos-0.1.5/investos/portfolio/constraint_model/long_constraint.py
--rw-r--r--   0        0        0     1411 2023-07-19 05:16:44.132321 investos-0.1.5/investos/portfolio/constraint_model/trade_constraint.py
--rw-r--r--   0        0        0     2402 2023-07-19 05:16:44.132629 investos-0.1.5/investos/portfolio/constraint_model/weight_constraint.py
--rw-r--r--   0        0        0    13341 2023-07-19 05:16:44.132867 investos-0.1.5/investos/portfolio/controller.py
--rw-r--r--   0        0        0      168 2023-07-19 05:16:44.133026 investos-0.1.5/investos/portfolio/cost_model/__init__.py
--rw-r--r--   0        0        0     1850 2023-07-19 05:16:44.133180 investos-0.1.5/investos/portfolio/cost_model/base_cost.py
--rw-r--r--   0        0        0     2120 2023-07-19 05:16:44.133467 investos-0.1.5/investos/portfolio/cost_model/holding_cost.py
--rw-r--r--   0        0        0     4075 2023-07-19 05:16:44.133639 investos-0.1.5/investos/portfolio/cost_model/trading_cost.py
--rw-r--r--   0        0        0      104 2023-07-19 05:16:44.133795 investos-0.1.5/investos/portfolio/result/__init__.py
--rw-r--r--   0        0        0    12614 2023-07-19 05:16:44.133970 investos-0.1.5/investos/portfolio/result/base_result.py
--rw-r--r--   0        0        0      300 2023-07-19 05:16:44.134415 investos-0.1.5/investos/portfolio/result/forecast_result.py
--rw-r--r--   0        0        0     4532 2023-07-19 05:16:44.134575 investos-0.1.5/investos/portfolio/result/save_result.py
--rw-r--r--   0        0        0      115 2023-07-19 05:16:44.134721 investos-0.1.5/investos/portfolio/risk_model/__init__.py
--rw-r--r--   0        0        0     1306 2023-07-19 05:16:44.135169 investos-0.1.5/investos/portfolio/risk_model/base_risk.py
--rw-r--r--   0        0        0     2599 2023-07-19 05:16:44.135446 investos-0.1.5/investos/portfolio/risk_model/stat_factor_risk.py
--rw-r--r--   0        0        0      160 2023-07-19 05:16:44.135700 investos-0.1.5/investos/portfolio/strategy/__init__.py
--rw-r--r--   0        0        0     1274 2023-07-19 05:16:44.136176 investos-0.1.5/investos/portfolio/strategy/base_strategy.py
--rw-r--r--   0        0        0     3990 2023-07-19 05:16:44.136619 investos-0.1.5/investos/portfolio/strategy/rank_long_short.py
--rw-r--r--   0        0        0     3887 2023-07-19 05:16:44.136789 investos-0.1.5/investos/portfolio/strategy/spo.py
--rw-r--r--   0        0        0     2249 2023-07-19 05:16:44.137255 investos-0.1.5/investos/util.py
--rw-r--r--   0        0        0     1908 2023-07-20 19:52:38.569220 investos-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2287 1970-01-01 00:00:00.000000 investos-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    20869 2023-04-03 18:29:49.638655 investos-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1904 2023-07-24 00:26:14.040338 investos-0.1.6/README.md
+-rw-r--r--   0        0        0       49 2023-08-01 18:00:06.636074 investos-0.1.6/investos/__init__.py
+-rw-r--r--   0        0        0      238 2023-07-21 18:30:51.315697 investos-0.1.6/investos/portfolio/__init__.py
+-rw-r--r--   0        0        0      337 2023-07-21 18:30:51.315827 investos-0.1.6/investos/portfolio/constraint_model/__init__.py
+-rw-r--r--   0        0        0      466 2023-07-21 18:30:51.315953 investos-0.1.6/investos/portfolio/constraint_model/base_constraint.py
+-rw-r--r--   0        0        0     1331 2023-07-21 18:30:51.316077 investos-0.1.6/investos/portfolio/constraint_model/leverage_constraint.py
+-rw-r--r--   0        0        0     2579 2023-07-21 18:30:51.316202 investos-0.1.6/investos/portfolio/constraint_model/long_constraint.py
+-rw-r--r--   0        0        0     1411 2023-07-21 18:30:51.316360 investos-0.1.6/investos/portfolio/constraint_model/trade_constraint.py
+-rw-r--r--   0        0        0     2361 2023-07-21 18:30:51.316520 investos-0.1.6/investos/portfolio/constraint_model/weight_constraint.py
+-rw-r--r--   0        0        0    13295 2023-07-21 18:30:51.316723 investos-0.1.6/investos/portfolio/controller.py
+-rw-r--r--   0        0        0      168 2023-07-21 18:30:51.316851 investos-0.1.6/investos/portfolio/cost_model/__init__.py
+-rw-r--r--   0        0        0     1851 2023-07-21 18:30:51.316976 investos-0.1.6/investos/portfolio/cost_model/base_cost.py
+-rw-r--r--   0        0        0     2121 2023-07-21 18:30:51.317101 investos-0.1.6/investos/portfolio/cost_model/holding_cost.py
+-rw-r--r--   0        0        0     4076 2023-07-21 18:30:51.317232 investos-0.1.6/investos/portfolio/cost_model/trading_cost.py
+-rw-r--r--   0        0        0      159 2023-07-25 18:27:16.735028 investos-0.1.6/investos/portfolio/result/__init__.py
+-rw-r--r--   0        0        0    12627 2023-07-26 06:37:12.033358 investos-0.1.6/investos/portfolio/result/base_result.py
+-rw-r--r--   0        0        0      260 2023-07-21 18:30:51.317663 investos-0.1.6/investos/portfolio/result/forecast_result.py
+-rw-r--r--   0        0        0     4551 2023-08-01 17:55:15.170620 investos-0.1.6/investos/portfolio/result/save_result.py
+-rw-r--r--   0        0        0     1300 2023-08-01 18:45:00.404371 investos-0.1.6/investos/portfolio/result/weights_result.py
+-rw-r--r--   0        0        0      115 2023-07-19 05:16:44.134721 investos-0.1.6/investos/portfolio/risk_model/__init__.py
+-rw-r--r--   0        0        0     1307 2023-07-21 18:30:51.317920 investos-0.1.6/investos/portfolio/risk_model/base_risk.py
+-rw-r--r--   0        0        0     2599 2023-07-21 18:30:51.318049 investos-0.1.6/investos/portfolio/risk_model/stat_factor_risk.py
+-rw-r--r--   0        0        0      160 2023-07-19 05:16:44.135700 investos-0.1.6/investos/portfolio/strategy/__init__.py
+-rw-r--r--   0        0        0     1275 2023-07-21 18:30:51.318176 investos-0.1.6/investos/portfolio/strategy/base_strategy.py
+-rw-r--r--   0        0        0     3991 2023-07-21 18:30:51.318305 investos-0.1.6/investos/portfolio/strategy/rank_long_short.py
+-rw-r--r--   0        0        0     4040 2023-07-21 18:30:51.318476 investos-0.1.6/investos/portfolio/strategy/spo.py
+-rw-r--r--   0        0        0     2215 2023-07-21 18:30:51.318602 investos-0.1.6/investos/util.py
+-rw-r--r--   0        0        0     2287 2023-08-01 17:59:36.224378 investos-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 investos-0.1.6/PKG-INFO
```

### Comparing `investos-0.1.5/LICENSE` & `investos-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `investos-0.1.5/investos/portfolio/constraint_model/leverage_constraint.py` & `investos-0.1.6/investos/portfolio/constraint_model/leverage_constraint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import cvxpy as cvx
 
-from investos.util import values_in_time
 from investos.portfolio.constraint_model.base_constraint import BaseConstraint
 
 
 class MaxLeverageConstraint(BaseConstraint):
     """
     A constraint that enforces a limit on the (absolute) leverage of the portfolio.
```

### Comparing `investos-0.1.5/investos/portfolio/constraint_model/long_constraint.py` & `investos-0.1.6/investos/portfolio/constraint_model/long_constraint.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-import numpy as np
-import cvxpy as cvx
-
-from investos.util import values_in_time
 from investos.portfolio.constraint_model.base_constraint import BaseConstraint
 
 
 class LongOnlyConstraint(BaseConstraint):
     """
     A constraint that enforces no short positions. Including no short cash position.
```

### Comparing `investos-0.1.5/investos/portfolio/constraint_model/trade_constraint.py` & `investos-0.1.6/investos/portfolio/constraint_model/trade_constraint.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import numpy as np
 import cvxpy as cvx
+import numpy as np
 
-from investos.util import values_in_time
 from investos.portfolio.constraint_model.base_constraint import BaseConstraint
+from investos.util import values_in_time
 
 
 class MaxTradeConstraint(BaseConstraint):
     """
     A constraint that enforces a limit on the (absolute) max trade size (as a weight, or fraction, of daily volume).
 
     Parameters
```

### Comparing `investos-0.1.5/investos/portfolio/constraint_model/weight_constraint.py` & `investos-0.1.6/investos/portfolio/constraint_model/weight_constraint.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from investos.util import values_in_time
 from investos.portfolio.constraint_model.base_constraint import BaseConstraint
 
 
 class MaxWeightConstraint(BaseConstraint):
     """
     A constraint that enforces a limit on the weight of each asset in a portfolio.
```

### Comparing `investos-0.1.5/investos/portfolio/controller.py` & `investos-0.1.6/investos/portfolio/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import pandas as pd
-import numpy as np
-import statistics
 import datetime as dt
+import statistics
 from typing import Callable
 
-import investos.portfolio.strategy as strategy
-from investos.portfolio.strategy import BaseStrategy, RankLongShort
+import numpy as np
+import pandas as pd
+
 import investos.portfolio.result as result
 import investos.util as util
+from investos.portfolio.strategy import BaseStrategy, RankLongShort
 
 
 class Controller:
     """Container class that runs backtests using passed-in portfolio optimization `strategy` (see :py:class:`~investos.portfolio.strategy.base_strategy.BaseStrategy`), then saves results into passed-in `result` (see :py:class:`~investos.backtest.result.Result`) class.
 
     Parameters
     ----------
```

### Comparing `investos-0.1.5/investos/portfolio/cost_model/base_cost.py` & `investos-0.1.6/investos/portfolio/cost_model/base_cost.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import pandas as pd
-import datetime as dt
 import copy
+import datetime as dt
+
+import pandas as pd
 
 
 class BaseCost:
     """Base cost model for InvestOS.
     Other cost models should subclass BaseCost.
     The only requirement of custom cost models is that they (re)implement :py:meth:`~investos.portfolio.cost_model.base_cost.BaseCost.value_expr`.
     """
```

### Comparing `investos-0.1.5/investos/portfolio/cost_model/holding_cost.py` & `investos-0.1.6/investos/portfolio/cost_model/holding_cost.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import pandas as pd
-import numpy as np
 import datetime as dt
+
 import cvxpy as cvx
+import numpy as np
+import pandas as pd
 
 from investos.portfolio.cost_model import BaseCost
 from investos.util import values_in_time
 
 
 class HoldingCost(BaseCost):
     """Calculates cost for holding short positions, given customizable short_rate."""
```

### Comparing `investos-0.1.5/investos/portfolio/cost_model/trading_cost.py` & `investos-0.1.6/investos/portfolio/cost_model/trading_cost.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import pandas as pd
-import numpy as np
 import datetime as dt
+
 import cvxpy as cvx
+import numpy as np
+import pandas as pd
 
 from investos.portfolio.cost_model import BaseCost
 from investos.util import values_in_time
 
 
 class TradingCost(BaseCost):
     """Calculates per period cost for trades `u`, based on spread, standard deviation, volume, and price.
```

### Comparing `investos-0.1.5/investos/portfolio/result/base_result.py` & `investos-0.1.6/investos/portfolio/result/base_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-import pandas as pd
+import collections
+import datetime as dt
+
 import numpy as np
+import pandas as pd
 
-import datetime as dt
-import collections
+from investos.portfolio.result.save_result import SaveResult
 from investos.util import clip_for_dates
-from investos.portfolio.result import SaveResult
 
 
 class BaseResult(SaveResult):
     """The `Result` class captures portfolio data and performance for each asset and period over time.
 
     Instances of this object are called by the :py:meth:`investos.portfolio.controller.Controller.generate_positions` method.
     """
```

### Comparing `investos-0.1.5/investos/portfolio/result/save_result.py` & `investos-0.1.6/investos/portfolio/result/save_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import requests
-import json
 
 
 class SaveResult:
     def save(
         self,
         description,
-        tags,
         api_key,
         api_endpoint="https://app.forecastos.com/api/v1",
+        tags=[],
+        team_ids=[],
     ):
         self.api_key = api_key
         self.api_endpoint = api_endpoint
         self.request_headers = {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
         }
         self.tags = tags
+        self.team_ids = team_ids
 
         self.save_backtest(description)
         self.save_backtest_charts()
 
     def save_backtest(self, description):
         json_body = {
             "backtest": {
@@ -30,17 +31,16 @@
                     "annualized_return": self.annualized_return,
                     "annualized_excess_return": self.annualized_excess_return,
                     "sharpe_ratio": self.sharpe_ratio,
                     "max_drawdown": self.max_drawdown,
                     "annual_turnover": self.annual_turnover,
                 },
                 "portfolio_id": None,
-                "team_id": None,
-                "project_id": None,
                 "tags": self.tags,
+                "team_ids": self.team_ids,
             }
         }
 
         response = requests.post(
             f"{self.api_endpoint}/backtests",
             headers=self.request_headers,
             json=json_body,
```

### Comparing `investos-0.1.5/investos/portfolio/risk_model/base_risk.py` & `investos-0.1.6/investos/portfolio/risk_model/base_risk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import pandas as pd
 import datetime as dt
 
+import pandas as pd
+
 from investos.portfolio.cost_model import BaseCost
 
 
 class BaseRisk(BaseCost):
     """Base risk model for InvestOS.
 
     The only requirement of custom risk models is that they implement a `_estimated_cost_for_optimization` method.
```

### Comparing `investos-0.1.5/investos/portfolio/risk_model/stat_factor_risk.py` & `investos-0.1.6/investos/portfolio/risk_model/stat_factor_risk.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import pandas as pd
-import numpy as np
 import cvxpy as cvx
+import numpy as np
+import pandas as pd
 
 from investos.portfolio.risk_model import BaseRisk
 
 
 class StatFactorRisk(BaseRisk):
     """PCA-factor based risk model.
```

### Comparing `investos-0.1.5/investos/portfolio/strategy/base_strategy.py` & `investos-0.1.6/investos/portfolio/strategy/base_strategy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import pandas as pd
 import datetime as dt
 
+import pandas as pd
+
 
 class BaseStrategy:
     """Base class for an optimization strategy.
 
     Must implement :py:meth:`~investos.portfolio.strategy.base_strategy.BaseStrategy.generate_trade_list` as per below.
 
     Attributes
```

### Comparing `investos-0.1.5/investos/portfolio/strategy/rank_long_short.py` & `investos-0.1.6/investos/portfolio/strategy/rank_long_short.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import pandas as pd
 import datetime as dt
 
+import pandas as pd
+
+from investos.portfolio.cost_model import BaseCost, HoldingCost, TradingCost
 from investos.portfolio.strategy import BaseStrategy
-from investos.portfolio.cost_model import TradingCost, HoldingCost, BaseCost
 from investos.util import values_in_time
 
 
 class RankLongShort(BaseStrategy):
     """Optimization strategy that builds trade list by going long assets with best return forecasts and short stocks with worst return forecasts.
```

### Comparing `investos-0.1.5/investos/portfolio/strategy/spo.py` & `investos-0.1.6/investos/portfolio/strategy/spo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,24 @@
-import pandas as pd
 import datetime as dt
+
 import cvxpy as cvx
+import pandas as pd
 
-from investos.portfolio.constraint_model import *
-from investos.portfolio.risk_model import *
+import investos.util as util
+from investos.portfolio.constraint_model import (
+    BaseConstraint,
+    EqualLongShortConstraint,
+    MaxLeverageConstraint,
+    MaxWeightConstraint,
+    MinWeightConstraint,
+)
+from investos.portfolio.cost_model import BaseCost, HoldingCost, TradingCost
+from investos.portfolio.risk_model import BaseRisk, StatFactorRisk
 from investos.portfolio.strategy import BaseStrategy
-from investos.portfolio.cost_model import TradingCost, HoldingCost, BaseCost
 from investos.util import values_in_time
-import investos.util as util
 
 
 class SPO(BaseStrategy):
     """Optimization strategy that builds trade list using single period optimization."""
 
     BASE_SOLVER_OPTS = {
         "max_iter": 50_000,
```

### Comparing `investos-0.1.5/investos/util.py` & `investos-0.1.6/investos/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import copy
 from functools import wraps
 
-import numpy as np
 import pandas as pd
 
 
 def deep_dict_merge(default_d, update_d):
     "Deep copies update_d onto default_d recursively"
 
     default_d = copy.deepcopy(default_d)
     update_d = copy.deepcopy(update_d)
 
     def deep_dict_merge_inner(default_d, update_d):
-        for k, v in update_d.items():
+        for k in update_d.keys():
             if (
                 k in default_d
                 and isinstance(default_d[k], dict)
                 and isinstance(update_d[k], dict)
             ):
                 deep_dict_merge_inner(default_d[k], update_d[k])
             else:
@@ -52,15 +51,15 @@
     tau: np.Timestamp (or similar), or None. Time tau >= t
         of the prediction,  e.g., tau could be tomorrow, t
         today, and we ask for prediction of market volume tomorrow,
         made today. If None, then it is assumed tau = t.
 
     """
 
-    if hasattr(obj, "__call__"):
+    if callable(obj):
         return obj(t, tau)
 
     if isinstance(obj, pd.Series) or isinstance(obj, pd.DataFrame):
         try:
             if isinstance(obj.index, pd.MultiIndex):
                 return obj.loc[(t, tau)]
             else:
```

### Comparing `investos-0.1.5/pyproject.toml` & `investos-0.1.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "investos"
-version = "0.1.5"
+version = "0.1.6"
 description = "For investors who want to focus on generating alpha"
 authors = ["Charlie Reese"]
 license = "Creative Commons Attribution-NonCommercial-ShareAlike (CC-BY-NC-SA)"
 readme = "README.md"
 packages = [{include = "investos"}]
 homepage = "https://investos.io/"
 repository = "https://github.com/charliereese/investos"
@@ -38,14 +38,20 @@
 [tool.poetry.group.dev.dependencies]
 black = {version = "^23.7.0", extras = ["jupyter"]}
 jupyter = "^1.0.0"
 pandas-market-calendars = "^4.1.4"
 pytest = "^7.3.1"
 ruff = "^0.0.278"
 sphinx = "^7.0.0"
+ipywidgets = "^8.0.7"
+jupyterlab = "^3"
+plotly = "^5.15.0"
+pyarrow = "^12.0.1"
+xgboost = "^1.7.6"
+scikit-learn = "^1.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 python_files = [
@@ -67,13 +73,28 @@
 
 [tool.ruff]
 exclude = [
     "__pycache__",
     ".git/",
     ".pytest_cache/",
 ]
+select = [
+    "B",
+    "E",
+    "F",
+    "I",
+    "Q",
+    "UP",
+    "W",
+]
+ignore = [
+    "B006",  # Mutable argument default
+    "B008",  # Function call in default argument
+    "E501",  # Line too long 
+]
 target-version = "py39"
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = [
-    'F401',
+    'F401',  # Unused import
+    'F403',  # Wildcard import
 ]
```

