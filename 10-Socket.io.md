## WebSocket
 is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket
 remains open all the time, so they allow real-time data transfer. When clients trigger the request to the server, it does not close the 
 connection on receiving the response; it rather persists and waits for the Client or server to terminate the request.
 
 We need WebSocket because It provides full-duplex communication, which helps in persisting the connection established between the Client and the Web Server.
 It also lives up to the standards and provides the accuracy and efficiency stream events to and from with negligible latency.WebSocket removes the overhead
 and reduce complexity.It makes real-time communication effortless and efficient.
 
 ## Socket.IO
 
 is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol 
 to provide the interface. Generally, it is divided into two parts; both WebSocket vs Socket.io are event-driven libraries.
 - Client-Side: it is the library that runs inside the browser
 - Server Side: It is the library for Node.js
 - 
 We need Socket.IO:
I handle all the degradation of your technical alternatives to get full-duplex communication in real-time.
It also handles the various support level and the inconsistencies from the browser.
It also gives the additional feature room support for basic publish infrastructure and thinks like automatic reconnect.
Currently, AFAIK is the most used one and easier to help with vanilla web sockets.

**Key features of Socket.IO**
It helps in broadcasting to multiple sockets at a time and handles the connection transparently.
It works on all platform, server or device, ensuring equality, reliability, and speed.
It automatically upgrades the requirement to WebSocket if needed.
It is a custom real-time transport protocol implementation on top of other protocols.
It requires both libraries to be used Client side as well as a server-side library.
IO works on work-based events. there are some reserved events that can be accessed using the Socket on the server side like Connect, message, Disconnect, Ping and Reconnect.
There are some Client based reserved events like Connect, connect- error, connect-timeout and Reconnect etc.


## Key Differences between WebSocket and socket.io
It provides the Connection over TCP, while Socket.io is a library to abstract the WebSocket connections. WebSocket doesn't have 
fallback options, while Socket.io supports fallback.WebSocket is the technology, while Socket.io is a library for WebSockets.

 
