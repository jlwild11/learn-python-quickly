## 

## Open a file

Open in read only.

```
f = open('/my_path/my_file.txt','r')
```

## Access and read a file

```
file_data = f.read()
```

## Close a file

```
f.close()
```

## Write to a file

```
f = open('/my_path/my_file.txt','w')
```

Caution: once you open a file in writing mode, anything that it had contained previously will be deleted. If you're interested in adding to an existing file \(without deleting its content\) you should use append instead of write and open in append mode \(using a instead of w\).

```
f.write("Hello World!")
f.close()
```

# `with` {#-with-}

Python allows you to open a file, do operations on it, and automatically close it afterwards using`with`.

```
>>> with open('/my_path/my_file.txt','r') as f:
>>>   file_data = f.read()
```



