# Code 401 Class 10 Reading notes:

## Stacks and Queues
### What is a Stack
A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.

Common terminology for a stack is

- Push - Nodes or items that are put into the stack are pushed
- Pop - Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised.
- Top - This is the top of the stack.
- Peek - When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.
- IsEmpty - returns true when stack is empty otherwise returns false.

### Stacks follow these concepts:

**FILO**
First In Last Out

This means that the first item added in the stack will be the last item popped out of the stack.

**LIFO**
Last In First Out

This means that the last item added to the stack will be the first item popped out of the stack.

**Stack Visualization**
Here’s an example of what a stack looks like. As you can see, the topmost item is denoted as the top. When you push something to the stack, it becomes the new top. When you pop something from the stack, you pop the current top and set the next top as top.next.

![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/stack1.PNG)

## Stack

### Push O(1)
Pushing a Node onto a stack will always be an O(1) operation. This is because it takes the same amount of time no matter how many Nodes (n) you have in the stack.

When adding a Node, you push it into the stack by assigning it as the new top, with its next property equal to the original top.

Let’s walk through the steps:

- First, you should have the Node that you want to add. Here is an example of a Node that we want to add to the stack. 

![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/pushStack1.PNG)

**Push to Stack 01**

- Next, you need to assign the next property of Node 5 to reference the same Node that top is referencing: Node 4. 

![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/pushStack2.PNG)

**Push to Stack 02**

- Technically at this point, your new Node is added to your stack, but there is no indication that it is the first Node in the stack. To make this happen, you have to re-assign our reference top to the newly added Node, Node 5. 

![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/pushStack3.PNG)

**Push to Stack 02**

- Congratulations! You completed a successful push of Node 5 onto the stack.

## What is a Queue

### Common terminology for a queue is

1. Enqueue - Nodes or items that are added to the queue.
2. Dequeue - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
3. Front - This is the front/first Node of the queue.
4. Rear - This is the rear/last Node of the queue.
5. Peek - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
6. IsEmpty - returns true when queue is empty otherwise returns false.


### Queues follow these concepts:

**FIFO**
First In First Out

This means that the first item in the queue will be the first item out of the queue.

**LILO**
Last In Last Out

This means that the last item in the queue will be the last item out of the queue.

**Queue Visualization**
Here is what a Queue looks like:

### Queue

### Enqueue O(1)
When you add an item to a queue, you use the enqueue action. This is done with an O(1) operation in time because it does not matter how many other items live in the queue (n); it takes the same amount of time to perform the operation.

Let’s walk through the process of adding a Node to a queue:

![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/Enqueue1.PNG)

**Enqueue 01**

- First, we should change the next property of Node 4 to point to the Node we are adding. In our case with the visual below, we will be re-assigning Node 4’s .next to Node 5. The only way we have access to Node 4 is through our reference rear. Following the rules of reference types, this means that we must change rear.next to Node 5. 

![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/Enqueue3.PNG)

**Enqueue 02**

- After we have set the next property, we can re-assign the rear reference to point to Node 5. By doing this, it allows us to keep a reference of where the rear is, and we can continue to enqueue Nodes into the queue as needed. 

![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/Enqueue3.PNG)

**Enqueue 03**


- Congratulations! You have just successfully added a Node to a queue by activating the enqueue action.


## General summaries of what I learned this week :

**RBAC**

Role-based access control (RBAC) is a policy-neutral access-control mechanism defined around roles and privileges. The components of RBAC such as role-permissions, user-role and role-role relationships make it simple to perform user assignments.


**User Roles**

User Roles are permission sets that control access to areas and features within the Professional Archive Platform. Each User account requires a Role assignment.


**JWT Token**

JSON Web Token is a proposed Internet standard for creating data with optional signature and/or optional encryption whose payload holds JSON that asserts some number of claims. The tokens are signed either using a private secret or a public/private key.

**encryption**

Cryptographically turns data into a secret code that cannot easily be deciphered

**token**

A token is a thing that represents an object

**bearer**

A type of token used for authentication - represents the user

**secret**

A secret ket or passcode used to login or create a login/token

**JSON Web Token**

JSON web tokens are used to securely transmit data between parties as 
JSON objects

**Client ID**

The client_id is a public identifier for apps, It must also be unique across all clients that the authorization server handles.

**Client Secret**

The client_secret is a secret known only to the application and the authorization server. It must be sufficiently random to not be guessable.

**Authentication Endpoint**

mechanism used to verify the identity of a network's connecting device .

**Access Token Endpoint**

used in token-based authentication to allow an application to access an API .


**API Endpoint**

is the point of communication when two systems are interacting. It refers to communication between an API and a server.

**Authorization Code**

is a temporary code that the client will exchange for an access token. The code itself is obtained from the authorization server

**Access Token**

used in token-based authentication to allow an application to access an API .

**Router Middleware**

The term is composed of 2 words router and middleware. Middleware. It is a piece of code that comes in the middle of request and response . It kind of hijacks your request so that you can do anything that you want with your request or response eg: Modify the data or call the next middleware.

**Dynamic Module Loading**

Dynamic loading is a mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory.

**Singleton Pattern**

Use the Singleton pattern when a class in your program should have just a single instance available to all clients; for example, a single database object shared by different parts of the program. The Singleton pattern disables all other means of creating objects of a class except for the special creation method.

**CRUD -> REST Method Matches**

Which GET HTTP method is equivalent to which the CRUD operation?
HTTP GET - SELECT/Request. HTTP PUT - UPDATE. HTTP POST - INSERT/Create. HTTP DELETE - DELETE.

**Mock Testing**

Mocking is done when you invoke methods of a class that has external communication like database calls or rest calls. Through mocking you can explicitly define the return value of methods without actually executing the steps of the method.



#### Want To Know More ? 
[Stacks and Queues](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html)