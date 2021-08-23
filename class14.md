What does it mean that web sockets are bidirectional? Why is this useful?
Whereas HTTP relies on a client request to receive a response from the server for every exchange, WebSockets allow for full-duplex bidirectional communication. This enables the server to send real-time updates asynchronously, without requiring the client to submit a request each time


Does socket.io use HTTP? Why?

Even when websockets can be used, the initial connection setup it done over HTTP. Also, a socket.io server will attach to an HTTP server so it can serve its own client code through /socket.io/socket.io.js .


What happens when a client emits an event?

socket.emit allows you to emit custom events on the server and client. socket.send sends messages which are received with the 'message' event.


What happens when a server emits an event?
sends a an event in to all the other clients that are connected on the same socket connection and gives it the ability to listen to the event in order to act upon it.


What happens if a client “misses” an event?

Unhandled messages are just ignored. It's just like when an event occurs and there are no event listeners for that event. The socket receives the msg and doesn't find a handler for it so nothing happens with it.



How can we mitigate this?

You could avoid missing messages by always having the handlers installed and then deciding in the handlers (based on other state) whether to do anything with the message or not.




Socket

A socket is one endpoint of a two-way communication link between two programs running on the network. A socket is bound to a port number so that the TCP layer can identify the application that data is destined to be sent to. ... Every TCP connection can be uniquely identified by its two endpoints.


Web Socket

WebSocket is a communications protocol for a persistent, bi-directional, full duplex TCP connection from a user's web browser to a server. A WebSocket connection is initiated by sending a WebSocket handshake request from a browser's HTTP connection to a server to upgrade the connection.


Socket.io

Socket.IO is a JavaScript library for realtime web applications. It enables realtime, bi-directional communication between web clients and servers. It has two parts: a client-side library that runs in the browser, and a server-side library for Node. js. Both components have a nearly identical API.


Client

n computing, a client is a piece of computer hardware or software that accesses a service made available by a server as part of the client–server model of computer networks. The server is often (but not always) on another computer system, in which case the client accesses the service by way of a network.


Server

A server is a computer connected to a network of other workstations called 'clients'. Client computers request information from the server over the network. Servers tend to have more storage, memory and processing power than a normal workstation


OSI Model

The OSI Model (Open Systems Interconnection Model) is a conceptual framework used to describe the functions of a networking system. The OSI model characterizes computing functions into a universal set of rules and requirements in order to support interoperability between different products and software.


TCP Model

TCP stands for Transmission Control Protocol a communications standard that enables application programs and computing devices to exchange messages over a network. It is designed to send packets across the internet and ensure the successful delivery of data and messages over networks.

TCP

TCP stands for Transmission Control Protocol a communications standard that enables application programs and computing devices to exchange messages over a network. It is designed to send packets across the internet and ensure the successful delivery of data and messages over networks.

UDP

User datagram protocol (UDP) operates on top of the Internet Protocol (IP) to transmit datagrams over a network. UDP does not require the source and destination to establish a three-way handshake before transmission takes place.

Packets

In networking, a packet is a small segment of a larger message. Data sent over computer networks*, such as the Internet, is divided into packets. These packets are then recombined by the computer or device that receives them. ... This is similar to how packets work on the Internet.

