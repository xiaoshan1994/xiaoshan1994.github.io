---
title: 4 data structures in Python
date: 2021-08-31T12:08:51+02:00
description:
images:
- https://i.morioh.com/2019/11/09/c99230a9da36.jpg
thumbnailImagePosition: left
thumbnailImage: //i.morioh.com/2019/11/09/c99230a9da36.jpg
tags:
- Python
- code
Categories:
- Skill
- Coding
---
# Tuple
Tuples are used to store multiple items in a single variable.
A tuple is a collection which is ordered and unchangeable.
Tuples are written with round brackets.
```
thistuple = ("apple", "banana", "cherry")
```
* Tuple items are **ordered, unchangeable, and allow duplicate values**.
  - When we say that tuples are ordered, it means that the items have a defined order, and that order will not change.
  - Tuples are unchangeable, meaning that ***we cannot change, add or remove items after the tuple has been created***.
  - Since tuples are indexed, they can have items with the same value
* Tuple items are indexed, the first item has index [0], the second item has index [1] etc.

Tuple items can be String, int and boolean data types
```
tuple1 = ("apple", "banana", "cherry")
tuple2 = (1, 5, 7, 9, 3)
tuple3 = (True, False, False)
```
# List
Lists are used to store multiple items in a single variable.
Lists are created using square brackets:
```
thislist = ["apple", "banana", "cherry"]
```
* List items are **ordered, changeable, and allow duplicate values**.
  - List items have a defined order
  - The list is changeable, meaning that we can change, add, and remove items in a list after it has been created
  - Since lists are indexed, lists can have items with the same value
* List items are indexed, the first item has index [0], the second item has index [1] etc.
* List items can be String, int and boolean data types.

# Dictionary
Dictionaries are used to store data values in key: value pairs.
A dictionary is a collection which is ordered*, changeable and does not allow duplicates.
- Dictionaries cannot have two items with the same key (duplicate values will overwrite existing values)
```
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964,
  "year": 2020
}
```
Dictionaries are written with **curly brackets**, and have keys and values:
```
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict)
```
# Set
Sets are used to store multiple items in a single variable.
Set items are unordered, unchangeable, and do not allow duplicate values.
Sets are written with curly brackets.
```
thisset = {"apple", "banana", "cherry"}
```
