# HashTables :

### What is a Hashtable?

  * "A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array".

  * "Hashing is a technique or process of mapping keys, values into the hash table by using a hash function. It is done for faster access to elements. The efficiency of mapping depends on the efficiency of the hash function used".

### What is a Buckets?

  * "A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs".

### What is a Collisions ?

  * "A collision is what happens when more than one key gets hashed to the same location of the hashtable".

### Hashtable Used for :
   1. Hold unique values
   2. Dictionary
   3. Library

### Creating a Hash :

  * "A hashtable traditionally is created from an array. I always like the size 1024. this is important for index placement. After you have created your array of the appropriate size, do some sort of logic to turn that “key” into a numeric number value". 

  * "A collision occurs when more than one key hashes to the same index in an array. As mentioned earlier, a “perfect hash” will never have any collisions. To put this into perspective, the worst possible hash is one that hashes every single key to the same exact index of an array. The more keys you have hashed to a specific index, the more key/value pair combos you can potentially have".

  * "Hashing is implemented in two steps:
    1. An element is converted into an integer by using a hash function. This element can be used as an index to store the original element, which falls into the hash table.
   2. The element is stored in the hash table where it can be quickly retrieved using hashed key.
      hash = hashfunc(key)
      index = hash % array_size.

### To achieve a good hashing mechanism, It is important to have a good hash function with the following basic requirements:
  1. Easy to compute.
  2. Uniform distribution.
  3. Less collisions

![image1](https://he-s3.s3.amazonaws.com/media/uploads/dda3e36.jpg)

### Internal Methods :
  * Add() : When adding a new key/value pair to a hashtable.
  * Find() : "The Find takes in a key, gets the Hash, and goes to the index location specified. Once at the index location is found in the array, it is then the responsibility of the algorithm the iterate through the bucket and see if the key exists and return the value".
  * Contains() : "The Contains method will accept a key, and return a bool on if that key exists inside the hashtable. The best way to do this is to have the contains call the GetHash and check the hashtable if the key exists in the table given the index returned".
  * GetHash() : "The GetHash will accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed".

### Linear probing (open addressing or closed hashing)
  * "In open addressing, instead of in linked lists, all entry records are stored in the array itself. When a new entry has to be inserted, the hash index of the hashed value is computed and then the array is examined (starting with the hashed index). If the slot at the hashed index is unoccupied, then the entry record is inserted in slot at the hashed index else it proceeds in some probe sequence until it finds an unoccupied slot".

### Quadratic Probing
  * "Quadratic probing is similar to linear probing and the only difference is the interval between successive probes or entry slots. Here, when the slot at a hashed index for an entry record is already occupied, you must start traversing until you find an unoccupied slot. The interval between slots is computed by adding the successive value of an arbitrary polynomial in the original hashed index".

### Double hashing
  * "Double hashing is similar to linear probing and the only difference is the interval between successive probes. Here, the interval between probes is computed by using two hash functions".




#### Sources:
[source1](https://www.geeksforgeeks.org/hashing-data-structure/)

[source2](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)

[source3](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)

