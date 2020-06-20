
# class-readings-25-github.io

Is a HashTable useful for search or sorting operations? Why?

Hashtable is useful for serach as all we need to know is a little bit of data of what we are looking for.

What makes a good hash function?

The hash functions are deterministic ,their output is determined only by their input. 
Hash functions should never have randomness to them. The same key should always produce the same hash code/index.

Why should you try to reduce the number of collisions?

The worst possible hash function is one that hashes every single key to the same exact index of an array and that is the reason we
should avoid collision.Therefore more than one key hashes to the same index of an array.
A HashTable needs to be able to handle two keys resolving to the same index. Otherwise, data could be lost as two different keys begin to overwrite each other at their position on the array.

What is stored at each index of a HashTable? Why?

Data is stored
