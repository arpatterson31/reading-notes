# Class 13 Reading: Message Queues

## Review, Research, and Discussion

### What does it mean that web sockets are bidirectional? Why is this useful?

- It enables the server to send real-time updates asynchronously, without requiring the client to submit a request each time. In the context of networked AV and control systems, this allows devices to send and receive continuous streams of data to and from any point on the network. *[source](https://www.amx.com/en-US/site_elements/benefits-and-applications-of-websockets)*

### Does socket.io use HTTP? Why?

- Socket.IO is NOT a WebSocket implementation. Although Socket.IO indeed uses WebSocket as a transport when possible, it adds additional metadata to each packet. That is why a WebSocket client will not be able to successfully connect to a Socket.IO server, and a Socket.IO client will not be able to connect to a plain WebSocket server either. *[source](https://socket.io/docs/v4/index.html)*

### What happens when a client emits an event?

- Client emits the event and it is handled by the server *[source](https://www.tutorialspoint.com/socket.io/socket.io_event_handling.htm)*

### What happens when a server emits an event?

- Server emits the event and it is handled by the client side

### What happens if a client “misses” an event?

- Unhandled messages are just ignored. It's just like when an event occurs and there are no event listeners for that event. The socket receives the msg and doesn't find a handler for it so nothing happens with it. *[source](https://stackoverflow.com/questions/32816290/what-happens-with-unhandled-socket-io-events)*

### How can we mitigate this?

- You could avoid missing messages by always having the handlers installed and then deciding in the handlers (based on other state) whether to do anything with the message or not. *[source](https://stackoverflow.com/questions/32816290/what-happens-with-unhandled-socket-io-events)*

## Document the following vocab words

- **socket:** software structure within a network node of a computer network that serves as an endpoint for sending and receiving data across the network. *[source](https://en.wikipedia.org/wiki/Network_socket)*
- **web socket:** a computer communications protocol, providing full-duplex communication channels over a single TCP connection. *[source](https://en.wikipedia.org/wiki/WebSocket)*
- **socket.io:** a library that enables real-time, bidirectional and event-based communication between the browser and the server. *[source](https://socket.io/docs/v4/index.html#What-Socket-IO-is)*
- **client:** a piece of computer hardware or software that accesses a service made available by a server as part of the client–server model of computer networks. *[source](https://en.wikipedia.org/wiki/Client_(computing))*
- **server:** a piece of computer hardware or software (computer program) that provides functionality for other programs or devices, called "clients". *[source](https://en.wikipedia.org/wiki/Server_(computing))*
- **OSI model (Open Systems Interconnection model):** a conceptual model that characterises and standardises the communication functions of a telecommunication or computing system without regard to its underlying internal structure and technology. Its goal is the interoperability of diverse communication systems with standard communication protocols. *[source](https://en.wikipedia.org/wiki/OSI_model)*
- **TCP Model:** specifications for translating the network addressing methods used in the Internet Protocol to link-layer addresses, such as media access control (MAC) addresses. *[source](https://en.wikipedia.org/wiki/Internet_protocol_suite)*
- **TCP:** Transmission control protocol. TCP provides reliable, ordered, and error-checked delivery of a stream of octets (bytes) between applications running on hosts communicating via an IP network. *[source](https://en.wikipedia.org/wiki/Transmission_Control_Protocol)*
- **UDP:** User Datagram Protocol - With UDP, computer applications can send messages, in this case referred to as datagrams, to other hosts on an Internet Protocol (IP) network. *[source](https://en.wikipedia.org/wiki/User_Datagram_Protocol)*
- **Packets:** a formatted unit of data carried by a packet-switched network. A packet consists of control information and user data;[1] the latter is also known as the payload. *[source](https://en.wikipedia.org/wiki/Network_packet)*

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

- socket.io from previous readings. I'm getting more and more understanding after reading the different articles provided.

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- a little bit more information on these protocols that have been in these last readings

### What are you most excited about trying to implement or see how it works?

- again, i'm excited to se how the rooms and chat features for socket.io work!
