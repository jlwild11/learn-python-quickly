## Dictionaries

Dictionaries store pairs of elements: keys and values. In this example we define a dictionary where the keys are element names and the values are their corresponding atomic numbers.

```
elements = {'hydrogen': 1, 'helium': 2, 'carbon': 6}
```

We can look up values in the dictionary using square brackets enclosing a key:

```
>>> print(element['carbon'])
6
```

We can also insert new values into the dictionary with square brackets:

```
>>> elements['lithium'] = 3
>>> print(elements['lithium'])
3
```

We can check whether a value is in a dictionary on the same way we check whether a value is in a list or set with the`in`keyword.

```
if 'mithril' in elements:
    print("That's a real element!")
else:
    print("There's no such element!')
```

We can use`in`to verify whether a key is in the dictionary before looking it up, if there's a possibility that the key isn't there.

Dicts have a related method that's also useful,`get`.`get`looks up values in a dictionary, but unlike square brackets,`get`returns`None`\(or a default value of your choice\) if the key isn't found. If you expect lookups to sometimes fail,`get`might be a better tool than normal square bracket lookups.

```
>>> elements.get('dilithium')
None
>>> elements['dilithium']
KeyError: 'dilithium'
>>> elements.get('kryptonite', 'There\'s no such element!')
"There's no such element!"
```

The syntax for iterating over dictionaries is very similar to sets.

```
Beatles_Discography = {"Please Please Me": 1963, "With the Beatles": 1963, 
    "A Hard Day's Night": 1964, "Beatles for Sale": 1964, "Twist and Shout": 1964,
    "Help": 1965, "Rubber Soul": 1965, "Revolver": 1966,
    "Sgt. Pepper's Lonely Hearts Club Band": 1967,
    "Magical Mystery Tour": 1967, "The Beatles": 1968,
    "Yellow Submarine": 1969 ,'Abbey Road': 1969,
    "Let It Be": 1970}

for album_title in Beatles_Discography:
    print("title: {}, year: {}".format(album_title, Beatles_Discography[album_title]))
```

But what if we wanted to store more information about each element, like their weight and symbol?

```
elements = {'hydrogen': {'number': 1, 'weight': 1.00794, 'symbol': 'H'},
            'helium': {'number': 2, 'weight': 4.002602, 'symbol': 'He'}}
```

```
>>> print(elements['helium'])
{'number': 2, 'symbol': 'He', 'weight': 4.002602}
>>> print(elements.get('unobtainium', 'There\'s no such element!'))
There's no such element!
```

```
>>> print(elements['helium']['weight'])
4.002602
```



