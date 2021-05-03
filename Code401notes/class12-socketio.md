# Class 12 Reading: Socket.io

## Review, Research, and Discussion

### What is the benefit of transforming data into packets

- Packet switching is used to optimize the use of the channel capacity available in digital telecommunication networks, such as computer networks, and minimize the transmission latency (the time it takes for data to pass across the network), and to increase robustness of communication. *[source](https://en.wikipedia.org/wiki/Packet_switching#Packet_switching_in_networks)*

### UDP is often referred to as a connectionless protocol..Why is that?

- UDP uses a simple connectionless communication model with a minimum of protocol mechanisms *[source](https://en.wikipedia.org/wiki/User_Datagram_Protocol)*

### Can a socket server application have multiple socket connections?

- A server socket listens on a single port. All established client connections on that server are associated with that same listening port on the server side of the connection. An established connection is uniquely identified by the combination of client-side and server-side IP/Port pairs. Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to. *[source](https://stackoverflow.com/questions/11129212/tcp-can-two-different-sockets-share-a-port#:~:text=5%20Answers&text=A%20server%20socket%20listens%20on%20a%20single%20port.&text=Multiple%20connections%20on%20the%20same,system%20resources%20allow%20it%20to.)*

### Can a socket connection application be connected to multiple socket servers?

- On the client-side, it is common practice for new outbound connections to use a random client-side port, in which case it is possible to run out of available ports if you make a lot of connections in a short amount of time. *[source](https://stackoverflow.com/questions/11129212/tcp-can-two-different-sockets-share-a-port#:~:text=5%20Answers&text=A%20server%20socket%20listens%20on%20a%20single%20port.&text=Multiple%20connections%20on%20the%20same,system%20resources%20allow%20it%20to.)*

### Can an application be both a socket server and a socket connection?

- You can use a client socket and a server socket within a single application... You can do that if you're willing to use two different ports. You can also use threads. If you are using TCP, you might have to add a delay in connecting a client after a server thread is spawned, reason being the server socket need to be ready and listening when a client is trying to connect. *[source](https://www.quora.com/Can-you-make-a-client-socket-and-a-server-socket-in-one)*

## Document the following vocab words

- **Observer pattern:** a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods. *[source](https://en.wikipedia.org/wiki/Observer_pattern)*
- **Listener:** It can be a JavaScript function which respond to the event occur. *[source](https://www.geeksforgeeks.org/javascript-addeventlistener-with-examples/)*
- **Event Handler:** code that can be made to run when an event is triggered by assigning it to the target element's corresponding onevent property, or by registering the handler as a listener for the element using the addEventListener() method.*[source](https://developer.mozilla.org/en-US/docs/Web/Events/Event_handlers)*
- **Event Driven Progamming:** programming paradigm in which the flow of the program is determined by events such as user actions (mouse clicks, key presses), sensor outputs, or message passing from other programs or threads. *[source](https://en.wikipedia.org/wiki/Event-driven_programming)*
- **Event Loop:**  programming construct or design pattern that waits for and dispatches events or messages in a program. The event loop works by making a request to some internal or external "event provider" (that generally blocks the request until an event has arrived), then calls the relevant event handler ("dispatches the event"). The event loop is also sometimes referred to as the message dispatcher, message loop, message pump, or run loop. *[source](https://en.wikipedia.org/wiki/Event_loop)*
- **Event Queue:** a repository where events from an application are held prior to being processed by a receiving program or system. Event queues are often used in the context of an enterprise messaging system. *[source](https://www.techopedia.com/definition/24963/event-queue)*
- **Call Stack:** a stack data structure that stores information about the active subroutines of a computer program. *[source](https://en.wikipedia.org/wiki/Call_stack)*
- **Emit/Raise/Trigger:** functions that call the specified event
- **Subscribe:** unction is similar to the Promise.then(), .catch() and .finally() methods in jQuery, but instead of dealing with promises it deals with Observables. That means it will subscribe itself to the observable of interest (which is getTasks() in your case) and wait until it is successful and then execute the first passed callback function *[source](https://stackoverflow.com/questions/42000883/what-does-the-subscribe-function-do)*
- **database:** stores organized information

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

### What are you most excited about trying to implement or see how it works?
