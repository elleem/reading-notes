## Hash Tables

#### Things I Want to Know More About


### Hash Tables Cheat Sheet

Hashtable Cheat Sheet

Terminology:

Hash: The result of an algorithm that converts a string into a value used to determine the index of an array in a hashtable.
Buckets: Containers in each index of the hashtable array, capable of holding multiple key/value pairs if collisions occur.
Collisions: Occur when multiple keys hash to the same location in the hashtable.
Why use hashtables:

Hold unique values
Implement dictionaries or libraries
Structure of a Hashtable:

Hashtable is a data structure that uses key-value pairs.
Each node or bucket in the hashtable contains a key and a value.
Hashing:

Hashing is the process of converting a key into an integer using a hash function.
The hash code should be deterministic, producing the same output for the same input.
A hash code helps determine the index in the array where the key-value pair should be stored.
Creating a Hash:

Initialize an array of an appropriate size.
Convert the key into a numeric value using a hashing algorithm.
Use modulo to find the remainder of the hash code divided by the array size.
Store the key-value pair in the array at the calculated index.
Collisions:

Collisions occur when multiple keys hash to the same index in the array.
To handle collisions, each index in the array can hold a linked list of key-value pairs.
The entire key-value pair is stored in the bucket to differentiate between values for the same index.



Bucket Sizes:

The number of buckets in a hashtable can vary.
Fewer buckets result in denser storage and more collisions.
More buckets create sparser storage but may have empty space.
Load factor can be used to determine how full the hashtable is and when to resize it.





