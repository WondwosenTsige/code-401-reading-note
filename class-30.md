# [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## Read 30: Hashtable

### What is a Hashtable?

Terminology:

Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.

Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.

Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

### Why do we use them?

Hold unique values
Dictionary
Library

### What Are they

Hashtables are a data structure that utilize key value pairs. This means every Node or Bucket has both a key, and a value.

Read more on the link below

[Hashtables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)

### Basics of Hash Tables

Hashing is a technique that is used to uniquely identify a specific object from a group of similar objects. Some examples of how hashing is used in our lives include:

In universities, each student is assigned a unique roll number that can be used to retrieve information about them.
In libraries, each book is assigned a unique number that can be used to determine information about the book, such as its exact position in the library or the users it has been issued to etc.

Hashing is implemented in two steps:

    1. An element is converted into an integer by using a hash function. This element can be used as an index to store the original element, which falls into the hash table.

    2. The element is stored in the hash table where it can be quickly retrieved using hashed key.

    hash = hashfunc(key)
    index = hash % array_size

In this method, the hash is independent of the array size and it is then reduced to an index (a number between 0 and array_size − 1) by using the modulo operator (%).



...............................................................................

__Attributions for the following Reference materials and their authors__

[Hashtables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)

[Basic of Hash Tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)

[>> NEXT (Read: Class 31)](https://wondwosentsige.github.io/code-401-reading-note/class-31)