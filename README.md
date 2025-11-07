# myfaqsdump
This is intended for Interview preparation all FAQs and Topics to refer all resources at One Place for self ref 

[HashMap](#hasmap) - [SynchronizedHashMap](#synchronizedhashmap) - <a href="#CunccurentHashMap"> CunccurentHashMap </a>

String - StringBuffer - StringBuilder - StringTokenizer

java-8 features,java-17 features,

Streams, and its functions working type (some cross questions this topic)

JVM architecture , Working style of Memory blocks (Heap, ...etc.)

SOLID Principals

Design Patterns ( 3 Categories around 24 Patterns )

Microservice FAQs, Microservice Design Patterns ( Brush-up As many as you can )

## HashMap  
* Key-Value Storage: HashMap stores elements as (Key, Value) pairs. Keys must be unique, while values can be duplicated.  
* Hashing for Efficiency: It utilizes hashing internally for efficient storage and retrieval of elements.  
  This allows for average O(1) time complexity for put, get, and remove operations.
* Unordered: HashMap does not guarantee any specific order of elements. The order of insertion is not preserved, and elements are not sorted. For ordered maps, LinkedHashMap (insertion order) or TreeMap (sorted order) are alternatives.
* Not Thread-Safe: HashMap is not synchronized, meaning it's not thread-safe. In a multi-threaded environment, external synchronization or alternatives like ConcurrentHashMap should be used.
* Nulls Allowed: It allows for one null key and multiple null values.
* Wrapper Classes for Primitives: Keys and values must be objects (reference types). Primitive types like int or double cannot be used directly; their corresponding wrapper classes (Integer, Double, etc.) must be used instead.
### Basic Operations

Basic Operations:
The HashMap class provides various methods for interacting with the stored data:  

* put(K key, V value): Associates the specified value with the specified key in this map.
* get(Object key): Returns the value to which the specified key is mapped, or null if this map contains no mapping for the key.
* remove(Object key): Removes the mapping for the specified key from this map if present.
* containsKey(Object key): Returns true if this map contains a mapping for the specified key.
* containsValue(Object value): Returns true if this map maps one or more keys to the specified value.
* size(): Returns the number of key-value mappings in this map.
* clear(): Removes all of the mappings from this map.

### Internal Mechanism
    A HashMap uses an array of buckets internally.  
The location in the array (bucket) for an entry is determined by the key's hashCode() method.  
Collisions, where different keys hash to the same bucket, are handled using a linked list or,  
in Java 8 and later, a balanced tree within that bucket.

## SynchronizedHashMap

## CunccurentHashMap  
some content

