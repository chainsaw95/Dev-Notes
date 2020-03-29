@@ -0,0 +1,83 @@
## What is a Web Service

The term "web service" is often used to describe a service that a client (a computer) can call remotely over the internet, via web protocols like HTTP. Like calling a method, procedure or function which is running on a different machine than the client.

## Ways to connect distributed systems

**RPC**

Remote Procedure Call (RPC) is a protocol that one program can use to request a service from a program located in another computer on a network without having to understand the network's details. A procedure call is also sometimes known as a function call or a subroutine call

The essential goal of this approach is to make remote invocation as similar as possible to regular procedure calls and to hide the details of the physical connection.


**Messaging**

Messaging as a communication concept is very much different from RPC in that it does not attempt to hide the physical aspects of communication. It is still trying to hide the implementation details, but not to the point of dismissing the notions related to run-time costs of exchanging data.


**Queuing**

A message queue provides an asynchronous communications protocol, which is a system that puts a message onto a message queue and does not require an immediate response to continuing processing.

**Object Oriented / Distributed Object Model**

A distributed object-based system is a collection of objects that isolates the requesters of services (clients) from the providers of services (servers) by a well-defined encapsulating interface.

In the distributed object-based model, a client sends a message to an object, which in turn interprets the message to decide what service to perform. This service, or method, selection could be performed by either the object or a broker. The Java Remote Method Invocation (RMI) and the Common Object Request Broker Architecture (CORBA) are examples of this model.


**AJAX / XML-HTTP**

Web services developed from the combination of HTTP servers, JavaScript clients and Plain Old XML.

**SOAP**

Simple Object Access Protocol SOAP relies exclusively on XML to provide messaging services.Microsoft originally developed SOAP to take the place of older technologies that don’t work well on the internet such as the Distributed Component Object Model (DCOM) and Common Object Request Broker Architecture (CORBA). These technologies fail because they rely on binary messaging. The XML messaging that SOAP employs works better over the internet.


**GraphQL**

GraphQL is a syntax that describes how to ask for data, and is generally used to load data from a server to a client. GraphQL has three main characteristics:

- It lets the client specify exactly what data it needs.
- It makes it easier to aggregate data from multiple sources.
- It uses a type system to describe data.

**GRPC**

gRPC (general-purpose Remote Procedure Calls) is an open source remote procedure call (RPC) system initially developed at Google in 2015.It uses HTTP/2 for transport, Protocol Buffers as the interface description language, and provides features such as authentication, bidirectional streaming and flow control, blocking or nonblocking bindings, and cancellation and timeouts. It generates cross-platform client and server bindings for many languages. Most common usage scenarios include connecting services in microservices style architecture and connect mobile devices, browser clients to backend services.

**REST**

REST is acronym for REpresentational State Transfer. It is architectural style for distributed hypermedia systems and was first presented by Roy Fielding in 2000.

Guiding Principles of REST

- **Client–server** – By separating the user interface concerns from the data storage concerns, we improve the portability of the user interface across multiple platforms and improve scalability by simplifying the server components.

- **Stateless** – Each request from client to server must contain all of the information necessary to understand the request, and cannot take advantage of any stored context on the server. Session state is therefore kept entirely on the client.

- **Cacheable** – Cache constraints require that the data within a response to a request be implicitly or explicitly labeled as cacheable or non-cacheable. If a response is cacheable, then a client cache is given the right to reuse that response data for later, equivalent requests.

- **Uniform interface** – By applying the software engineering principle of generality to the component interface, the overall system architecture is simplified and the visibility of interactions is improved. In order to obtain a uniform interface, multiple architectural constraints are needed to guide the behavior of components. REST is defined by four interface constraints: identification of resources; manipulation of resources through representations; self-descriptive messages; and, hypermedia as the engine of application state.

- **Layered system** – The layered system style allows an architecture to be composed of hierarchical layers by constraining component behavior such that each component cannot “see” beyond the immediate layer with which they are interacting.

- **Code on demand (optional)** – REST allows client functionality to be extended by downloading and executing code in the form of applets or scripts. This simplifies clients by reducing the number of features required to be pre-implemented.

Further reading and references

- [graphql](https://www.freecodecamp.org/news/so-whats-this-graphql-thing-i-keep-hearing-about-baf4d36c20cf/)

- [rest](https://restfulapi.net/)

- [soap/rest](https://smartbear.com/blog/test-and-monitor/soap-vs-rest-whats-the-difference/)

- [RPC/Messaging](http://www.inspirel.com/articles/RPC_vs_Messaging.html)

- [RPC/Messaging](https://sbdevel.wordpress.com/2009/12/17/the-case-rpc-vs-messaging/)

- [Queuing](https://www.cloudamqp.com/blog/2014-12-03-what-is-message-queuing.html)

- [OO/DOM](https://www.oracle.com/technical-resources/articles/javase/rmi-corba.html)