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

##### Import multiple individual objects.

```
>>> from collections import defaultdict, namedtuple
```

##### To import a module and give it a different \(usually shorter\) name

To rename a module, you can use as:

`>>> import module_name as different_name`

for example

```
>>> import multiprocessing as mp
```

```
>>> mp.cpu_count()
4
```

### Import an individual item from a module and give it a different name {#import-an-individual-item-from-a-module-and-give-it-a-different-name}

You can combine the previous two pieces of syntax to import an item from a module and change its name:

```
from module_name import object_name as different_name
```

```
from csv import reader as csvreader
```



