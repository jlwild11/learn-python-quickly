# Importing Modules {#importing-modules}

```
>>> import math
```

```
>>> print(math.factorial(3))
6
```

### To import an individual function or class from a module use {#to-import-an-individual-function-or-class-from-a-module-use}

```
>>> from module_name import object_name
```

```
>>> from collections import defaultdict
```

This gives access only to defaultdict from the module collections. defaultdictwill be accessible with its own name \(without the module name before it\) and trying to access collections or even call collections.defaultdict\(\) will give a NameError.

