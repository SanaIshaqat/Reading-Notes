# Code 401 Class 24 Reading notes:
## Implementation: Hash Tables

## Document the Vocabulary Terms

**Rendering**

Rendering is a process used in web development that turns website code into the interactive pages users see when they visit a website. The term generally refers to the use of HTML, CSS, and JavaScript codes. The process is completed by a rendering engine, the software used by a web browser to render a web page.

**Templates**

A website template is a predesigned resource that shows the structure for the comprehensive layout and display features of any website. It is provided by various suppliers to help make Web design a lot easier for designers. A website template is also known as a Web page template or page template.

**State**

State is how something is; its configuration, attributes, condition or information content. We will use the term component to include software and hardware "things". Virtually all components have state, from applications to operating systems to network layers.


**Functional Components**

Functional components are basic JavaScript functions. These are typically arrow functions but can also be created with the regular function keyword. Sometimes referred to as “dumb” or “stateless” components as they simply accept data and display them in some form; that is they are mainly responsible for rendering UI.

**Children / Child Components**

Children allow you to pass components as data to other components, just like any other prop you use. The special thing about children is that React provides support through its ReactElement API and JSX. XML children translate perfectly to React children!

**State Hook**

State Hook The useState() is a Hook that allows you to have state variables in functional components , it takes the initial state as an argument and returns an array of two entries.

**Mounting and Un-Mounting**

Mounting and Un-Mounting The main job of React is to figure out how to modify the DOM to match what the components want to be rendered on the screen. React does so by mounting (adding nodes to the DOM), unmounting (removing them from the DOM), and updating (making changes to nodes already in the DOM).



## Intro to Hash Tables:

![](https://images.viblo.asia/01e58f10-41c7-4fc1-b235-67aa41263f1e.png)
### Hash

Is an algorithm takes a string and converts it into a value that could be used for security or some other purpose, in a hashtable, it is used to determine the index of the array.

### Buckets

Are contained in each index of the array of the hashtable
Each index is a bucket, index could potentially contain multiple key/value pairs if a collision occurs.

### Collisions
what happens when more than one key gets hashed to the same location of the hashtable.

### Hashing is implemented in two steps:

- An element is converted into an integer by using a hash function. This element can be used as an index to store the original element, which falls into the hash table.
- The element is stored in the hash table where it can be quickly retrieved using hashed key.
img


### What are Hash Tables

A data structure that utilizes key value pairs
every Node or Bucket has both a key, and a value
basic idea of a hashtable is the ability to store the key and quickly retrieve the value through a hash
hash is the ability to encode the key that will eventually map to a specific location
in the data structure, we can directly retrieve the value
O(1) time complexity for lookups.

### Internal Methods

**Add()**


send the key to the GetHash method
determine the index of where it should be placed
go to that index
Check if something exists at that index already
if it doesn’t, add it with the key/value pair.
else add the new key/value pair to the data structure within that bucket


**Find()**


takes in a key
gets the Hash
goes to the index location specified

**Contains()**


accept a key
return a boolean if that key exists inside the hashtable

**GetHash()**


GetHash will accept a key as a string
conduct the hash
return the index of the array where the key/value should be placed






#### Want To Know More ? 

[Read Intro to Hash Tables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html) 

[Watch what is a hash table?](https://www.youtube.com/watch?v=MfhjkfocRR0) 

[Read basics of hash tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/) 

[Skim hash table wiki](https://en.wikipedia.org/wiki/Hash_table) 