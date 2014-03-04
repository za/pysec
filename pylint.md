
```
# pip install pylint
```

```
➜  pysec git:(master) pylint sample.py
No config file found, using default configuration
************* Module sample
C:  9, 0: Invalid constant name "module_variable" (invalid-name)
W: 11,23: Redefining built-in 'int' (redefined-builtin)
W: 13, 4: Redefining name 'module_variable' from outer scope (line 9) (redefined-outer-name)
C: 11, 0: Invalid function name "functionName" (invalid-name)
C: 11, 0: Missing function docstring (missing-docstring)
W: 11,23: Unused argument 'int' (unused-argument)
W: 11,17: Unused argument 'self' (unused-argument)
W: 12, 4: Unused variable 'local' (unused-variable)
C: 16, 0: Invalid class name "my_class" (invalid-name)
C: 23, 8: Invalid attribute name "s" (invalid-name)
C: 16, 0: Missing class docstring (missing-docstring)
W: 18,29: Redefining name 'string' from outer scope (line 7) (redefined-outer-name)
W: 18,23: Unused argument 'arg1' (unused-argument)
W: 18,29: Unused argument 'string' (unused-argument)
W: 22,22: Redefining built-in 'str' (redefined-builtin)
C: 22, 4: Missing method docstring (missing-docstring)
C: 26, 4: Missing method docstring (missing-docstring)
W: 28, 8: Unreachable code (unreachable)
R: 26, 4: Method could be a function (no-self-use)
E: 30, 4: method already defined line 22 (function-redefined)
C: 30, 4: Missing method docstring (missing-docstring)
W: 23, 8: Attribute 's' defined outside __init__ (attribute-defined-outside-init)
C: 34, 0: Invalid class name "my_subclass" (invalid-name)
C: 34, 0: Missing class docstring (missing-docstring)
W: 36,29: Redefining name 'string' from outer scope (line 7) (redefined-outer-name)
W: 36, 4: __init__ method from base class 'my_class' is not called (super-init-not-called)
W:  7, 0: Unused import string (unused-import)
```

Report
======
24 statements analysed.

Messages by category
--------------------

+-----------+-------+---------+-----------+
|type       |number |previous |difference |
+===========+=======+=========+===========+
|convention |11     |NC       |NC         |
+-----------+-------+---------+-----------+
|refactor   |1      |NC       |NC         |
+-----------+-------+---------+-----------+
|warning    |14     |NC       |NC         |
+-----------+-------+---------+-----------+
|error      |1      |NC       |NC         |
+-----------+-------+---------+-----------+



Messages
--------

+-------------------------------+------------+
|message id                     |occurrences |
+===============================+============+
|missing-docstring              |6           |
+-------------------------------+------------+
|invalid-name                   |5           |
+-------------------------------+------------+
|unused-argument                |4           |
+-------------------------------+------------+
|redefined-outer-name           |3           |
+-------------------------------+------------+
|redefined-builtin              |2           |
+-------------------------------+------------+
|unused-variable                |1           |
+-------------------------------+------------+
|unused-import                  |1           |
+-------------------------------+------------+
|unreachable                    |1           |
+-------------------------------+------------+
|super-init-not-called          |1           |
+-------------------------------+------------+
|no-self-use                    |1           |
+-------------------------------+------------+
|function-redefined             |1           |
+-------------------------------+------------+
|attribute-defined-outside-init |1           |
+-------------------------------+------------+



Global evaluation
-----------------
Your code has been rated at -2.92/10

Raw metrics
-----------

+----------+-------+------+---------+-----------+
|type      |number |%     |previous |difference |
+==========+=======+======+=========+===========+
|code      |21     |65.62 |NC       |NC         |
+----------+-------+------+---------+-----------+
|docstring |4      |12.50 |NC       |NC         |
+----------+-------+------+---------+-----------+
|comment   |2      |6.25  |NC       |NC         |
+----------+-------+------+---------+-----------+
|empty     |5      |15.62 |NC       |NC         |
+----------+-------+------+---------+-----------+



Statistics by type
------------------

+---------+-------+-----------+-----------+------------+---------+
|type     |number |old number |difference |%documented |%badname |
+=========+=======+===========+===========+============+=========+
|module   |1      |NC         |NC         |100.00      |0.00     |
+---------+-------+-----------+-----------+------------+---------+
|class    |2      |NC         |NC         |0.00        |100.00   |
+---------+-------+-----------+-----------+------------+---------+
|method   |5      |NC         |NC         |40.00       |0.00     |
+---------+-------+-----------+-----------+------------+---------+
|function |1      |NC         |NC         |0.00        |100.00   |
+---------+-------+-----------+-----------+------------+---------+



Duplication
-----------

+-------------------------+------+---------+-----------+
|                         |now   |previous |difference |
+=========================+======+=========+===========+
|nb duplicated lines      |0     |NC       |NC         |
+-------------------------+------+---------+-----------+
|percent duplicated lines |0.000 |NC       |NC         |
+-------------------------+------+---------+-----------+
```
