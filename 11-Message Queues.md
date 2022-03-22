# Message Queues

A message queue is a form of asynchronous service-to-service communication used in serverless and microservices architectures. 
Messages are stored on the queue until they are processed and deleted. Each message is processed only once, by a single consumer.
Message queues can be used to decouple heavyweight processing, to buffer or batch work, and to smooth spiky workloads.

## Message Queue Basics

In modern cloud architecture, applications are decoupled into smaller, independent building blocks that are easier to develop, deploy and maintain.
Message queues provide communication and coordination for these distributed applications. Message queues can significantly simplify coding of decoupled 
applications, while improving performance, reliability and scalability.Message queues allow different parts of a system to communicate and process operations
asynchronously. A message queue provides a lightweight buffer which temporarily stores messages, and endpoints that allow software components to connect to
the queue in order to send and receive messages. The messages are usually small, and can be things like requests, replies, error messages, or just plain
information. To send a message, a component called a producer adds a message to the queue. The message is stored on the queue until another component
called a consumer retrieves the message and does something with it.



## Namespaces

Socket.IO allows you to Namespace your sockets, which essentially means assigning different endpoints or paths.This is a useful feature to minimize 
the number of resources (TCP connections) and at the same time separate concerns within your application by introducing separation between
communication channels. Multiple namespaces actually share the same WebSockets connection thus saving us socket ports on the server.
Namespaces are created on the server side. But they are joined by clients by sending a request to the server.

## Rooms

Rooms are subchannels of the namespaces. Rooms are purely a server-side construct and the client knows nothing about them.You can’t join a room with 
socket io from the client side, it should happens in the server side. To tackle this you need to emit a socket with the room you want to join as data , 
and in the server you listen to this socket and call socket.join() with the name or the id of the room that has been sent.
