# Code 401 Class 11 Reading notes:

## Review, Research, and Discussion

### Why is access control important?
Limits the risk of information being accessed without the appropriate authorisation .
### Describe an application that would need access control, What is a role used for?
Social media websites, data managment systems like university students grade-book system.

Role is used to regulate who or what can view or use any given resource. based on his bussiness authery in real life.

### Why is role based access control more scalable than discretionary or mandatory access control?
Unlike Mandatory Access Control (MAC) where access to system resources is controlled by the operating system (under the control of a system administrator), Discretionary Access Control (DAC) allows each user to control access to their own data. User A can, however, set access permissions on a file that she owns.
## Document the following Vocabulary Terms

**Authorization**
Authorization is the process of giving someone the ability to access a resource.

**Role Based Access Control**
Approach to restricting system access to authorized users.

**Capabilities**
The process the user is allowed to have access on based on his role.


## Preview


### Which 3 things had you heard about previously and now have better clarity on?
- Authentication 
- Authorization
- Jest
### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- Cookies
- Securing JWT
- EDA
- AWS
### What are you most excited about trying to implement or see how it works?
Authorising user to access certain data only after signing in, allowing user to change/password.

## Preparation Materials

### Event-Driven Programming
The idea in event-driven programming is that the program is designed to react.

It reacts to specific kinds of input from users, whether it's a click on a command button, a choice from a drop-down list, an entry into a text box, or other kinds of user events.

### Event-Driven Programming makes use of the following concepts?
An Event Handler is a callback function that will be called when an event is triggered. A Main Loop listens for event triggers and calls the associated event handler for that event.

### EventEmitter

Node.js natively provides a useful module called EventEmitter that allows us to get started incorporating Event-Driven Programming .

The **EventEmitter** instance will emit its own 'newListener' event before a listener is added to its internal array of listeners.

Listeners registered for the 'newListener' event are passed the event name and a reference to the listener being added.

The fact that the event is triggered before adding the listener has a subtle but important side effect: any additional listeners registered to the same name within the 'newListener' callback are inserted before the listener that is in the process of being added.

#### Want To Know More ? 
[Event Driven Programming](https://www.digitalocean.com/community/tutorials/nodejs-event-driven-programming)
[Node docs: events](https://nodejs.org/api/events.html#class-eventemitter)