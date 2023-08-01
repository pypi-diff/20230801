# Comparing `tmp/engineering_notation-0.8.0-py3-none-any.whl.zip` & `tmp/engineering_notation-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,9 @@
-Zip file size: 6612 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      181 b- defN 23-Jan-13 20:20 engineering_notation/__init__.py
--rw-rw-rw-  2.0 fat    15856 b- defN 23-Jan-13 20:46 engineering_notation/engineering_notation.py
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jan-13 20:47 engineering_notation/version.py
--rw-rw-rw-  2.0 fat     3924 b- defN 23-Jan-13 20:54 engineering_notation-0.8.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jan-13 20:54 engineering_notation-0.8.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1068 b- defN 23-Jan-13 20:54 engineering_notation-0.8.0.dist-info/license.txt
--rw-rw-rw-  2.0 fat       21 b- defN 23-Jan-13 20:54 engineering_notation-0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      731 b- defN 23-Jan-13 20:54 engineering_notation-0.8.0.dist-info/RECORD
-8 files, 21896 bytes uncompressed, 5312 bytes compressed:  75.7%
+Zip file size: 5793 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx      177 b- defN 23-Aug-01 01:30 engineering_notation/__init__.py
+-rw-rw-r--  2.0 unx    15569 b- defN 23-Aug-01 01:39 engineering_notation/engineering_notation.py
+-rw-rw-r--  2.0 unx       22 b- defN 23-Aug-01 01:39 engineering_notation/version.py
+-rw-rw-r--  2.0 unx     3878 b- defN 23-Aug-01 01:42 engineering_notation-0.9.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Aug-01 01:42 engineering_notation-0.9.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       21 b- defN 23-Aug-01 01:42 engineering_notation-0.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      626 b- defN 23-Aug-01 01:42 engineering_notation-0.9.0.dist-info/RECORD
+7 files, 20385 bytes uncompressed, 4665 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -3,23 +3,20 @@
 
 Filename: engineering_notation/engineering_notation.py
 Comment: 
 
 Filename: engineering_notation/version.py
 Comment: 
 
-Filename: engineering_notation-0.8.0.dist-info/METADATA
+Filename: engineering_notation-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: engineering_notation-0.8.0.dist-info/WHEEL
+Filename: engineering_notation-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: engineering_notation-0.8.0.dist-info/license.txt
+Filename: engineering_notation-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: engineering_notation-0.8.0.dist-info/top_level.txt
-Comment: 
-
-Filename: engineering_notation-0.8.0.dist-info/RECORD
+Filename: engineering_notation-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## engineering_notation/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-from engineering_notation.engineering_notation import EngNumber, EngUnit
-from engineering_notation.version import __version__
-
-__all__ = ['EngNumber', 'EngUnit', '__version__']
+from engineering_notation.engineering_notation import EngNumber, EngUnit
+from engineering_notation.version import __version__
+
+__all__ = ['EngNumber', 'EngUnit', '__version__']
```

## engineering_notation/engineering_notation.py

```diff
@@ -1,535 +1,544 @@
-from decimal import Decimal
-from string import digits
-
-_suffix_lookup = {
-    'y': 'e-24',
-    'z': 'e-21',
-    'a': 'e-18',
-    'f': 'e-15',
-    'p': 'e-12',
-    'n': 'e-9',
-    'u': 'e-6',
-    'm': 'e-3',
-    '': 'e0',
-    'k': 'e3',
-    'M': 'e6',
-    'G': 'e9',
-    'T': 'e12'
-}
-
-_exponent_lookup_scaled = {
-    '-48': 'y',
-    '-45': 'z',
-    '-42': 'a',
-    '-39': 'f',
-    '-36': 'p',
-    '-33': 'n',
-    '-30': 'u',
-    '-27': 'm',
-    '-24': '',
-    '-21': 'k',
-    '-18': 'M',
-    '-15': 'G',
-    '-12': 'T'
-}
-
-
-class EngUnit:
-    """
-    Represents an engineering number, complete with units
-    """
-    def __init__(self, value,
-                 precision=2, significant=0, unit: str = None):
-        """
-        Initialize engineering with units
-        :param value: the desired value in the form of a string, int, or float
-        :param precision: the number of decimal places
-        :param significant: the number of significant digits
-        if given, significant takes precendence over precision
-        """
-        suffix_keys = [key for key in _suffix_lookup.keys() if key != '']
-        self.unit = unit
-
-        if isinstance(value, str):
-            # parse the string into unit and engineering number
-            new_value = ''
-            v_index = 0
-            for c in value:
-                if (c in digits) or (c in ['.', '-']) or (c in suffix_keys):
-                    new_value += c
-                    v_index += 1
-                else:
-                    break
-
-            if self.unit is None and len(value) >= v_index:
-                self.unit = value[v_index:]
-
-            self.eng_num = EngNumber(new_value, precision, significant)
-
-        else:
-            self.eng_num = EngNumber(value, precision, significant)
-
-    def __repr__(self):
-        """
-        Returns the object representation
-        :return: a string representing the engineering number
-        """
-        unit = self.unit if self.unit else ''
-        return str(self.eng_num) + unit
-
-    def __str__(self):
-        """
-        Returns the string representation
-        :return: a string representing the engineering number
-        """
-        return self.__repr__()
-
-    def __int__(self):
-        """
-        Implements the 'int()' method
-        :return:
-        """
-        return int(self.eng_num)
-
-    def __float__(self):
-        """
-        Implements the 'float()' method
-        :return:
-        """
-        return float(self.eng_num)
-
-    def __add__(self, other):
-        """
-        Add two engineering numbers, with units
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, EngNumber):
-            other = EngUnit(str(other))
-
-        if self.unit != other.unit:
-            raise AttributeError('units do not match')
-
-        return EngUnit(str(self.eng_num + other.eng_num) + self.unit)
-
-    def __radd__(self, other):
-        """
-        Add two engineering numbers, with units
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        return self.__add__(other)
-
-    def __sub__(self, other):
-        """
-        Subtract two engineering numbers, with units
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, EngNumber):
-            other = EngUnit(str(other))
-
-        if self.unit != other.unit:
-            raise AttributeError('units do not match')
-
-        return EngUnit(str(self.eng_num - other.eng_num) + self.unit)
-
-    def __rsub__(self, other):
-        """
-        Subtract two engineering numbers, with units
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, EngNumber):
-            other = EngUnit(str(other))
-
-        if self.unit != other.unit:
-            raise AttributeError('units do not match')
-
-        return EngUnit(str(other.eng_num - self.eng_num) + self.unit)
-
-    def __mul__(self, other):
-        """
-        Multiply two engineering numbers, with units
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, EngNumber):
-            other = EngUnit(str(other))
-
-        return EngUnit(str(self.eng_num * other.eng_num)
-                       + self.unit + other.unit)
-
-    def __rmul__(self, other):
-        """
-        Multiply two engineering numbers, with units
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        return self.__mul__(other)
-
-    def __truediv__(self, other):
-        """
-        Divide two engineering numbers, with units
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, EngNumber):
-            other = EngUnit(str(other))
-
-        new_unit = ''
-        if self.unit:
-            new_unit += self.unit
-        if other.unit:
-            new_unit += '/' + other.unit
-
-        return EngUnit(str(self.eng_num / other.eng_num) + new_unit)
-
-    def __rtruediv__(self, other):
-        """
-        Divide two engineering numbers, with units
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, EngNumber):
-            other = EngUnit(str(other))
-
-        return EngUnit(str(other.eng_num / self.eng_num)
-                       + (other.unit + '/' + self.unit))
-
-    def __lt__(self, other):
-        """
-        Compare two engineering numbers, with units
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, EngNumber):
-            other = EngUnit(str(other))
-
-        if self.unit != other.unit:
-            raise AttributeError('units do not match')
-
-        return self.eng_num < other.eng_num
-
-    def __gt__(self, other):
-        """
-        Compare two engineering numbers, with units
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, EngNumber):
-            other = EngUnit(str(other))
-
-        if self.unit != other.unit:
-            raise AttributeError('units do not match')
-
-        return self.eng_num > other.eng_num
-
-    def __le__(self, other):
-        """
-        Compare two engineering numbers, with units
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, EngNumber):
-            other = EngUnit(str(other))
-
-        if self.unit != other.unit:
-            raise AttributeError('units do not match')
-
-        return self.eng_num <= other.eng_num
-
-    def __ge__(self, other):
-        """
-        Compare two engineering numbers, with units
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, EngNumber):
-            other = EngUnit(str(other))
-
-        if self.unit != other.unit:
-            raise AttributeError('units do not match')
-
-        return self.eng_num >= other.eng_num
-
-    def __eq__(self, other):
-        """
-        Compare two engineering numbers, with units
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, (EngNumber, EngUnit, str, int, float)):
-            return NotImplemented
-        if not isinstance(other, EngNumber):
-            other = EngUnit(str(other))
-
-        if self.unit != other.unit:
-            raise AttributeError('units do not match')
-
-        return self.eng_num == other.eng_num
-
-
-class EngNumber:
-    """
-    Used for easy manipulation of numbers which use engineering notation
-    """
-
-    def __init__(self, value,
-                 precision=2, significant=0):
-        """
-        Initialize the class
-
-        :param value: string, integer, or float representing
-        the numeric value of the number
-        :param precision: the precision past the decimal - default to 2
-        :param significant: the number of significant digits
-        if given, significant takes precendence over precision
-        """
-        self.precision = precision
-        self.significant = significant
-
-        if isinstance(value, str):
-            suffix_keys = [key for key in _suffix_lookup.keys() if key != '']
-
-            for suffix in suffix_keys:
-                if suffix in value:
-                    value = value[:-1] + _suffix_lookup[suffix]
-                    break
-
-            self.number = Decimal(value)
-
-        elif (isinstance(value, int)
-              or isinstance(value, float)
-              or isinstance(value, EngNumber)):
-            self.number = Decimal(str(value))
-
-    def to_pn(self, sub_letter=None):
-        """
-        Returns the part number equivalent.  For instance,
-        a '1k' would still be '1k', but a
-        '1.2k' would, instead, be a '1k2'
-        :return:
-        """
-        string = str(self)
-        if '.' not in string:
-            return string
-
-        # take care of the case of when there is no scaling unit
-        if not string[-1].isalpha():
-            if sub_letter is not None:
-                return string.replace('.', sub_letter)
-
-            return string
-
-        letter = string[-1]
-        return string.replace('.', letter)[:-1]
-
-    def __repr__(self):
-        """
-        Returns the string representation
-        :return: a string representing the engineering number
-        """
-        # since Decimal class only really converts number that are very small
-        # into engineering notation, then we will simply make all number a
-        # small number and take advantage of Decimal class
-        num_str = self.number * Decimal('10e-25')
-        num_str = num_str.to_eng_string().lower()
-
-        base, exponent = num_str.split('e')
-
-        if self.significant > 0:
-            if abs(Decimal(base)) >= 100.0:
-                base = str(round(Decimal(base), self.significant - 3))
-            elif abs(Decimal(base)) >= 10.0:
-                base = str(round(Decimal(base), self.significant - 2))
-            else:
-                base = str(round(Decimal(base), self.significant - 1))
-        else:
-            base = str(round(Decimal(base), self.precision))
-
-        if 'e' in base.lower():
-            base = str(int(Decimal(base)))
-
-        # remove trailing decimals:
-        # print(base)
-        # https://stackoverflow.com/questions/3410976/how-to-round-a-number-to-significant-figures-in-python
-        # https://stackoverflow.com/questions/11227620/drop-trailing-zeros-from-decimal
-        # base = '%s' % float("%#.2G"%Decimal(base))
-        # print(base)
-        # remove trailing decimal
-        if '.' in base:
-            base = base.rstrip('.')
-
-        # remove trailing .00 in precision 2
-        if self.precision == 2 and self.significant == 0:
-            if '.00' in base:
-                base = base[:-3]
-
-        return base + _exponent_lookup_scaled[exponent]
-
-    def __str__(self, eng=True, context=None):
-        """
-        Returns the string representation
-        :return: a string representing the engineering number
-        """
-        return self.__repr__()
-
-    def __int__(self):
-        """
-        Implements the 'int()' method
-        :return:
-        """
-        return int(self.number)
-
-    def __float__(self):
-        """
-        Implements the 'float()' method
-        :return:
-        """
-        return float(self.number)
-
-    def __add__(self, other):
-        """
-        Add two engineering numbers
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, EngNumber):
-            other = EngNumber(other)
-
-        num = self.number + other.number
-        return EngNumber(str(num))
-
-    def __radd__(self, other):
-        """
-        Add two engineering numbers
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        return self.__add__(other)
-
-    def __sub__(self, other):
-        """
-        Subtract two engineering numbers
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, EngNumber):
-            other = EngNumber(other)
-
-        num = self.number - other.number
-        return EngNumber(str(num))
-
-    def __rsub__(self, other):
-        """
-        Subtract two engineering numbers
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, EngNumber):
-            other = EngNumber(other)
-
-        num = other.number - self.number
-        return EngNumber(str(num))
-
-    def __mul__(self, other):
-        """
-        Multiply two engineering numbers
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, EngNumber):
-            other = EngNumber(other)
-
-        num = self.number * other.number
-        return EngNumber(str(num))
-
-    def __rmul__(self, other):
-        """
-        Multiply two engineering numbers
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        return self.__mul__(other)
-
-    def __truediv__(self, other):
-        """
-        Divide two engineering numbers
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, EngNumber):
-            other = EngNumber(other)
-
-        num = self.number / other.number
-        return EngNumber(str(num))
-
-    def __rtruediv__(self, other):
-        """
-        Divide two engineering numbers
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, EngNumber):
-            other = EngNumber(other)
-
-        num = other.number / self.number
-        return EngNumber(str(num))
-
-    def __lt__(self, other):
-        """
-        Compare two engineering numbers
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, EngNumber):
-            other = EngNumber(other)
-
-        return self.number < other.number
-
-    def __gt__(self, other):
-        """
-        Compare two engineering numbers
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, EngNumber):
-            other = EngNumber(other)
-
-        return self.number > other.number
-
-    def __le__(self, other):
-        """
-        Compare two engineering numbers
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, EngNumber):
-            other = EngNumber(other)
-
-        return self.number <= other.number
-
-    def __ge__(self, other):
-        """
-        Compare two engineering numbers
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, EngNumber):
-            other = EngNumber(other)
-
-        return self.number >= other.number
-
-    def __eq__(self, other):
-        """
-        Compare two engineering numbers
-        :param other: EngNum, str, float, or int
-        :return: result
-        """
-        if not isinstance(other, (EngNumber, str, int, float)):
-            return NotImplemented
-        if not isinstance(other, EngNumber):
-            other = EngNumber(other)
-
-        return self.number == other.number
+from decimal import Decimal
+from string import digits
+import sys
+
+try:
+    import numpy
+except ImportError:
+    pass
+
+_suffix_lookup = {
+    'y': 'e-24',
+    'z': 'e-21',
+    'a': 'e-18',
+    'f': 'e-15',
+    'p': 'e-12',
+    'n': 'e-9',
+    'u': 'e-6',
+    'm': 'e-3',
+    '': 'e0',
+    'k': 'e3',
+    'M': 'e6',
+    'G': 'e9',
+    'T': 'e12'
+}
+
+_exponent_lookup_scaled = {
+    '-48': 'y',
+    '-45': 'z',
+    '-42': 'a',
+    '-39': 'f',
+    '-36': 'p',
+    '-33': 'n',
+    '-30': 'u',
+    '-27': 'm',
+    '-24': '',
+    '-21': 'k',
+    '-18': 'M',
+    '-15': 'G',
+    '-12': 'T'
+}
+
+
+class EngUnit:
+    """
+    Represents an engineering number, complete with units
+    """
+    def __init__(self, value,
+                 precision=2, significant=0, unit: str = None):
+        """
+        Initialize engineering with units
+        :param value: the desired value in the form of a string, int, or float
+        :param precision: the number of decimal places
+        :param significant: the number of significant digits
+        if given, significant takes precendence over precision
+        """
+        suffix_keys = [key for key in _suffix_lookup.keys() if key != '']
+        self.unit = unit
+
+        if isinstance(value, str):
+            # parse the string into unit and engineering number
+            new_value = ''
+            v_index = 0
+            for c in value:
+                if (c in digits) or (c in ['.', '-']) or (c in suffix_keys):
+                    new_value += c
+                    v_index += 1
+                else:
+                    break
+
+            if self.unit is None and len(value) >= v_index:
+                self.unit = value[v_index:]
+
+            self.eng_num = EngNumber(new_value, precision, significant)
+
+        else:
+            self.eng_num = EngNumber(value, precision, significant)
+
+    def __repr__(self):
+        """
+        Returns the object representation
+        :return: a string representing the engineering number
+        """
+        unit = self.unit if self.unit else ''
+        return str(self.eng_num) + unit
+
+    def __str__(self):
+        """
+        Returns the string representation
+        :return: a string representing the engineering number
+        """
+        return self.__repr__()
+
+    def __int__(self):
+        """
+        Implements the 'int()' method
+        :return:
+        """
+        return int(self.eng_num)
+
+    def __float__(self):
+        """
+        Implements the 'float()' method
+        :return:
+        """
+        return float(self.eng_num)
+
+    def __add__(self, other):
+        """
+        Add two engineering numbers, with units
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, EngNumber):
+            other = EngUnit(str(other))
+
+        if self.unit != other.unit:
+            raise AttributeError('units do not match')
+
+        return EngUnit(str(self.eng_num + other.eng_num) + self.unit)
+
+    def __radd__(self, other):
+        """
+        Add two engineering numbers, with units
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        return self.__add__(other)
+
+    def __sub__(self, other):
+        """
+        Subtract two engineering numbers, with units
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, EngNumber):
+            other = EngUnit(str(other))
+
+        if self.unit != other.unit:
+            raise AttributeError('units do not match')
+
+        return EngUnit(str(self.eng_num - other.eng_num) + self.unit)
+
+    def __rsub__(self, other):
+        """
+        Subtract two engineering numbers, with units
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, EngNumber):
+            other = EngUnit(str(other))
+
+        if self.unit != other.unit:
+            raise AttributeError('units do not match')
+
+        return EngUnit(str(other.eng_num - self.eng_num) + self.unit)
+
+    def __mul__(self, other):
+        """
+        Multiply two engineering numbers, with units
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, EngNumber):
+            other = EngUnit(str(other))
+
+        return EngUnit(str(self.eng_num * other.eng_num)
+                       + self.unit + other.unit)
+
+    def __rmul__(self, other):
+        """
+        Multiply two engineering numbers, with units
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        return self.__mul__(other)
+
+    def __truediv__(self, other):
+        """
+        Divide two engineering numbers, with units
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, EngNumber):
+            other = EngUnit(str(other))
+
+        new_unit = ''
+        if self.unit:
+            new_unit += self.unit
+        if other.unit:
+            new_unit += '/' + other.unit
+
+        return EngUnit(str(self.eng_num / other.eng_num) + new_unit)
+
+    def __rtruediv__(self, other):
+        """
+        Divide two engineering numbers, with units
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, EngNumber):
+            other = EngUnit(str(other))
+
+        return EngUnit(str(other.eng_num / self.eng_num)
+                       + (other.unit + '/' + self.unit))
+
+    def __lt__(self, other):
+        """
+        Compare two engineering numbers, with units
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, EngNumber):
+            other = EngUnit(str(other))
+
+        if self.unit != other.unit:
+            raise AttributeError('units do not match')
+
+        return self.eng_num < other.eng_num
+
+    def __gt__(self, other):
+        """
+        Compare two engineering numbers, with units
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, EngNumber):
+            other = EngUnit(str(other))
+
+        if self.unit != other.unit:
+            raise AttributeError('units do not match')
+
+        return self.eng_num > other.eng_num
+
+    def __le__(self, other):
+        """
+        Compare two engineering numbers, with units
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, EngNumber):
+            other = EngUnit(str(other))
+
+        if self.unit != other.unit:
+            raise AttributeError('units do not match')
+
+        return self.eng_num <= other.eng_num
+
+    def __ge__(self, other):
+        """
+        Compare two engineering numbers, with units
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, EngNumber):
+            other = EngUnit(str(other))
+
+        if self.unit != other.unit:
+            raise AttributeError('units do not match')
+
+        return self.eng_num >= other.eng_num
+
+    def __eq__(self, other):
+        """
+        Compare two engineering numbers, with units
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, (EngNumber, EngUnit, str, int, float)):
+            return NotImplemented
+        if not isinstance(other, EngNumber):
+            other = EngUnit(str(other))
+
+        if self.unit != other.unit:
+            raise AttributeError('units do not match')
+
+        return self.eng_num == other.eng_num
+
+
+class EngNumber:
+    """
+    Used for easy manipulation of numbers which use engineering notation
+    """
+
+    def __init__(self, value,
+                 precision=2, significant=0):
+        """
+        Initialize the class
+
+        :param value: string, integer, or float representing
+        the numeric value of the number
+        :param precision: the precision past the decimal - default to 2
+        :param significant: the number of significant digits
+        if given, significant takes precendence over precision
+        """
+        self.precision = precision
+        self.significant = significant
+
+        if isinstance(value, str):
+            suffix_keys = [key for key in _suffix_lookup.keys() if key != '']
+
+            for suffix in suffix_keys:
+                if suffix in value:
+                    value = value[:-1] + _suffix_lookup[suffix]
+                    break
+
+            self.number = Decimal(value)
+
+        elif (isinstance(value, int)
+              or isinstance(value, float)
+              or isinstance(value, EngNumber)):
+            self.number = Decimal(str(value))
+        else:
+            # finally, check for numpy import
+            if 'numpy' in sys.modules and isinstance(value, numpy.integer):
+                self.number = Decimal(str(value))
+    def to_pn(self, sub_letter=None):
+        """
+        Returns the part number equivalent.  For instance,
+        a '1k' would still be '1k', but a
+        '1.2k' would, instead, be a '1k2'
+        :return:
+        """
+        string = str(self)
+        if '.' not in string:
+            return string
+
+        # take care of the case of when there is no scaling unit
+        if not string[-1].isalpha():
+            if sub_letter is not None:
+                return string.replace('.', sub_letter)
+
+            return string
+
+        letter = string[-1]
+        return string.replace('.', letter)[:-1]
+
+    def __repr__(self):
+        """
+        Returns the string representation
+        :return: a string representing the engineering number
+        """
+        # since Decimal class only really converts number that are very small
+        # into engineering notation, then we will simply make all number a
+        # small number and take advantage of Decimal class
+        num_str = self.number * Decimal('10e-25')
+        num_str = num_str.to_eng_string().lower()
+
+        base, exponent = num_str.split('e')
+
+        if self.significant > 0:
+            if abs(Decimal(base)) >= 100.0:
+                base = str(round(Decimal(base), self.significant - 3))
+            elif abs(Decimal(base)) >= 10.0:
+                base = str(round(Decimal(base), self.significant - 2))
+            else:
+                base = str(round(Decimal(base), self.significant - 1))
+        else:
+            base = str(round(Decimal(base), self.precision))
+
+        if 'e' in base.lower():
+            base = str(int(Decimal(base)))
+
+        # remove trailing decimals:
+        # print(base)
+        # https://stackoverflow.com/questions/3410976/how-to-round-a-number-to-significant-figures-in-python
+        # https://stackoverflow.com/questions/11227620/drop-trailing-zeros-from-decimal
+        # base = '%s' % float("%#.2G"%Decimal(base))
+        # print(base)
+        # remove trailing decimal
+        if '.' in base:
+            base = base.rstrip('.')
+
+        # remove trailing .00 in precision 2
+        if self.precision == 2 and self.significant == 0:
+            if '.00' in base:
+                base = base[:-3]
+
+        return base + _exponent_lookup_scaled[exponent]
+
+    def __str__(self, eng=True, context=None):
+        """
+        Returns the string representation
+        :return: a string representing the engineering number
+        """
+        return self.__repr__()
+
+    def __int__(self):
+        """
+        Implements the 'int()' method
+        :return:
+        """
+        return int(self.number)
+
+    def __float__(self):
+        """
+        Implements the 'float()' method
+        :return:
+        """
+        return float(self.number)
+
+    def __add__(self, other):
+        """
+        Add two engineering numbers
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, EngNumber):
+            other = EngNumber(other)
+
+        num = self.number + other.number
+        return EngNumber(str(num))
+
+    def __radd__(self, other):
+        """
+        Add two engineering numbers
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        return self.__add__(other)
+
+    def __sub__(self, other):
+        """
+        Subtract two engineering numbers
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, EngNumber):
+            other = EngNumber(other)
+
+        num = self.number - other.number
+        return EngNumber(str(num))
+
+    def __rsub__(self, other):
+        """
+        Subtract two engineering numbers
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, EngNumber):
+            other = EngNumber(other)
+
+        num = other.number - self.number
+        return EngNumber(str(num))
+
+    def __mul__(self, other):
+        """
+        Multiply two engineering numbers
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, EngNumber):
+            other = EngNumber(other)
+
+        num = self.number * other.number
+        return EngNumber(str(num))
+
+    def __rmul__(self, other):
+        """
+        Multiply two engineering numbers
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        return self.__mul__(other)
+
+    def __truediv__(self, other):
+        """
+        Divide two engineering numbers
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, EngNumber):
+            other = EngNumber(other)
+
+        num = self.number / other.number
+        return EngNumber(str(num))
+
+    def __rtruediv__(self, other):
+        """
+        Divide two engineering numbers
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, EngNumber):
+            other = EngNumber(other)
+
+        num = other.number / self.number
+        return EngNumber(str(num))
+
+    def __lt__(self, other):
+        """
+        Compare two engineering numbers
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, EngNumber):
+            other = EngNumber(other)
+
+        return self.number < other.number
+
+    def __gt__(self, other):
+        """
+        Compare two engineering numbers
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, EngNumber):
+            other = EngNumber(other)
+
+        return self.number > other.number
+
+    def __le__(self, other):
+        """
+        Compare two engineering numbers
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, EngNumber):
+            other = EngNumber(other)
+
+        return self.number <= other.number
+
+    def __ge__(self, other):
+        """
+        Compare two engineering numbers
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, EngNumber):
+            other = EngNumber(other)
+
+        return self.number >= other.number
+
+    def __eq__(self, other):
+        """
+        Compare two engineering numbers
+        :param other: EngNum, str, float, or int
+        :return: result
+        """
+        if not isinstance(other, (EngNumber, str, int, float)):
+            return NotImplemented
+        if not isinstance(other, EngNumber):
+            other = EngNumber(other)
+
+        return self.number == other.number
```

## engineering_notation/version.py

```diff
@@ -1 +1 @@
-__version__ = '0.8.0'
+__version__ = '0.9.0'
```

## Comparing `engineering_notation-0.8.0.dist-info/METADATA` & `engineering_notation-0.9.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: engineering-notation
-Version: 0.8.0
+Version: 0.9.0
 Summary: Easy engineering notation
 Home-page: https://github.com/slightlynybbled/engineering_notation
 Author: Jason R. Jones
 Author-email: slightlynybbled@gmail.com
 License: MIT
 Keywords: engineering notation decimal
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
-License-File: license.txt
 
 [![Unit Tests](https://github.com/slightlynybbled/engineering_notation/actions/workflows/unittest.yml/badge.svg)](https://github.com/slightlynybbled/engineering_notation/actions/workflows/unittest.yml)
 
 # Purpose
 
 To easily work with human-readable engineering notation.  I wrote this as a quick tool for my own use.
 I found that I was writing the same functionality into multiple packages and would like a quick pip-installable
@@ -114,9 +112,7 @@
 2meter     # <<< this value is equivalent to "0.002eter", the "m" was used to scale the unit!
 >>> EngUnit('2', unit='meter')   # <<< this will work better
 ```
 
 # Contributions
 
 Contributions are welcome.  Feel free to make feature requests in the issues.
-
-
```

## Comparing `engineering_notation-0.8.0.dist-info/RECORD` & `engineering_notation-0.9.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-engineering_notation/__init__.py,sha256=qJ2G7LIXk6DYMySOsRr3shKxCKWC_xGNJPdUuLs7qQo,181
-engineering_notation/engineering_notation.py,sha256=pZ9bxyKKhPCjLM92Bmrx7Ovct-c_mVpKK1puehm23i0,15856
-engineering_notation/version.py,sha256=yBu3sQ3KPk-uCQnyW1fOWVzUpb1PjIWdLs0gZmj2SQM,23
-engineering_notation-0.8.0.dist-info/METADATA,sha256=OczDGLJNTL7NnfknrIRj2-EYPqonTgYL7fEhEOpb0B4,3924
-engineering_notation-0.8.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-engineering_notation-0.8.0.dist-info/license.txt,sha256=vv8S6mGeYm7bjQrC1mZomHAPJf6r1Z3E_Cwk6v3htpA,1068
-engineering_notation-0.8.0.dist-info/top_level.txt,sha256=NM2x7gn9KDPltnckz38oGWiw0yVry_A-vwZi6L9IuCI,21
-engineering_notation-0.8.0.dist-info/RECORD,,
+engineering_notation/__init__.py,sha256=WtvM8za4jsyi_KADY-MFsGJ-2LTXbDg5hx05xNkv1O4,177
+engineering_notation/engineering_notation.py,sha256=0vYWVvO0lrVGyAf1XHfElKsfFfXNgY3__UIv7gEmjP4,15569
+engineering_notation/version.py,sha256=_DlwPNmTZTKflLiAF8YIqSr2ao66CTjj4bQtA6hz0jM,22
+engineering_notation-0.9.0.dist-info/METADATA,sha256=XoWLz9jmgsQM0Nge8E2NRkUskRv_EOfgXDgcjLnONSI,3878
+engineering_notation-0.9.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+engineering_notation-0.9.0.dist-info/top_level.txt,sha256=NM2x7gn9KDPltnckz38oGWiw0yVry_A-vwZi6L9IuCI,21
+engineering_notation-0.9.0.dist-info/RECORD,,
```

