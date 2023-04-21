# Data-Structures-Complexity-and-Algorithms

Matrices & List Comprehension:
A matrix is a representation of numbers, symbols, or expression in a 2D array. In CS, we can start to create a data structure that has values in rows and columns, much like a table, by utilizing a list within a list. In python 3, there is no data structure called a "Matrix". Therefore, we are programming a list within a list and following the rules of a regular matrix: all rows and colums must have the same number values, all items in the 2D list must have the same data types, and since indexing always starts at 0... row 1 is technically located at matrix_A[0].
List comprehension is a concise method to create a list in python used when: the list is a reuslt of some operations applied to all its items, it is a made from another sequence/iterable data, and when the list is member of another list/sequence/iterable data that satisfies a certain condition.
List comprehension conists of a square bracket containing an expression that describes the list, one or more For clause to explain its members, and thena  zero or more if clauses dependind on the complexity of the list.


Map & Filter:
The idea of a map function is to apply a function to an iterable data. One thing to note about the map function is that it does not return a specific data type, rather a python iterable data. Therefore, after we apply the map function, we just execture a list function on it.
Formatting:


map(function_name, sequence)

-- function_name: any function (built-in or selfmade) that returns a desired value of choice

-- sequence: any iterable data type


The idea of the filter function is to filter out items from a data set that meets a certain condition.
Formatting:

filter(bool_returning_function, sequence)

-- function: The function name we provide for filter() must be return a boolean value ... should also be able handle the items inside the sequence as its arguments

-- sequence: any iterable data type


Tuples:
Strings and Lists are basic iterable data types that are very similar with key differences: strings only allow alphanumeric characters and special symbols to represent text while lists allow all data types as its items/members. Additionally strings are immutable whereas lists are mutable. These significant differences cause issues when you require the following data structure: must be immutabke, must allow differnt data types as item, must be iterable or must be nestable.
Tuples can solve these issues. They are declared with parenthesis ( () is an empty tuple), (50,) is singleton tuple; the comma is required. Tuples are sliceable; therefore, indexable using square brackets.


Sets:
A set is an unordered collection with no duplicate elements as it is a mathematical way to describe collection of differnt unique obkects. By following the operations and characteristics of the mathematical set, we can utilize such data structure in our python code. 
Membership is one of the key operations with set because a set has no duplicates, a set's membership operation is one of the fastest operations compared to strings, lists, or tuples, and finally by using membership operator, we can be certain a target exists or does not exist in our data.
When accessing values in a set it is different because it is unordered. There is no concept of indexing or slicing with a set however it is iterable.
Sets are mutable; therefore, we can add and remove values, there are also methods much lists that can affect the original sets as well.
Sets in python 3 can utilize its vast operators to help us do complex calculations. Most of these operators will have a method counterpart because sets are mutable.


Our operators - union, intersection, difference, symmetric difference, proper subset, subset, proper superset, superset
union: The joining/combining of two sets.
Intersection: Members/Items that only exists in both sets.
Difference: Members/items that only exists in the first set and not the second set.
Symmetric Difference: Members/items that exists one or the other set, but not both sets.
Boolean Operators:
Proper Subset: A is proper subset of B if all members of A is found in B, but A cannot be exactly the same as B.
Subset: A is a Proper Subset of B if A < B is True, but A can equal to B unlike a proper subset.
Proper Superset: A is a proper superset of B if A has all the values of B and more, but they are not equal to each other.
Superset: A is a superset of B if A > B or A == B.

Two set are consided disjointed when two sets share no common value. Let A and B both represent a set. If A & B is empty, then set A and B are considered disjointed. To check this in python there is a method called: isdisjoint().

Recap of sets - They are NOT sliceable or indexable, CANNOT have sets inside them, DO NOT have order, CANNOT guarantee that their values will be in order, DO NOT record a value's position


Dictionary:
Dictionary (Associative Array, map, symbol table) is a data type that stores a collection of (key, value) pairs, such that each possible key appears at most once in the collection.
Common operations include adding or removing a pair, modifying an existing pair and lookup of a value associated with a particular key. Dictionaries also use {} like sets; however, their individual item format is very different. Each item in a dictionary be a pair of key: value.

Each item in a dictionary is a key, value pair as keys are unique address for a dictionary value's location. Must be immutable (strings, numbers, tuples, frozenset) and unique as two same key values cannot exist in a single dictionary.
Values of a dictionary with a key can be any data type. We can also update a dictionary by modifying existing values by referncing the key. We can add new values to a dictionary by creating a new key. We can also overwrite a value at an existing key by referencing and recreating the value for it 

We can delete a key hance deleing the value connected to the key. We can empty out the entire dictionary or delete the dictionary.
We can use the in and not in operators to check if a key exists in a dictionary.


Dictionary methods -
A.keys() –> Returns a sequence of keys/addresses in A.
A.values() –> Returns a sequence of item values in A.
A.items() –> Returns a sequence of key,item pairs in A.
A.get(address) –> Returns the item value at address.
A.update(B) –> Extends A with the dictionary of key,value pairs of B.

We can turn other data types to dictionaries as similar to lists, tuples and set, dictionaries also support comprehension.
