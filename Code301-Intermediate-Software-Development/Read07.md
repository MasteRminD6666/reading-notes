# What is REST

REST is acronym for REpresentational State Transfer. It is architectural style for distributed hypermedia systems and was first presented by Roy Fielding in 2000 in his famous dissertation.

Like any other architectural style, REST also does have it’s own 6 guiding constraints which must be satisfied if an interface needs to be referred as RESTful. These principles are listed below.



## Guiding Principles of REST
- Client–server – By separating the user interface concerns from the data storage concerns, we improve the portability of the user interface across multiple platforms and improve scalability by simplifying the server components.
- Stateless – Each request from client to server must contain all of the information necessary to understand the request, and cannot take advantage of any stored context on the server. Session state is therefore kept entirely on the client.
- Cacheable – Cache constraints require that the data within a response to a request be implicitly or explicitly labeled as cacheable or non-cacheable. If a response is cacheable, then a client cache is given the right to reuse that response data for later, equivalent requests.
- Uniform interface – By applying the software engineering principle of generality to the component interface, the overall system architecture is simplified and the visibility of interactions is improved. In order to obtain a uniform interface, multiple architectural constraints are needed to guide the behavior of components. REST is defined by four interface constraints: identification of resources; manipulation of resources through representations; self-descriptive messages; and, hypermedia as the engine of application state.
- Layered system – The layered system style allows an architecture to be composed of hierarchical layers by constraining component behavior such that each component cannot “see” beyond the immediate layer with which they are interacting.
Code on demand (optional) 
– REST allows client functionality to be extended by downloading and executing code in the form of applets or scripts. This simplifies clients by reducing the number of features required to be pre-implemented.


## Who is Roy Fielding?
the pearson who crated the HTTP (Hypertext Transfer Protocol

## Why don’t the techniques that we use today work well when we need to be able to talk to all of the machines in the world?
because each machine has a different language

## What is the HTTP protocol that Fielding and his friends created?
its an application-layer protocol for transmitting hypermedia documents, such as HTML. It was designed for communication between web browsers and web servers, 


## What does a GET do?
GET is used to request data from a specified resource.

## What does a POST do?
POST is used to send data to a server to create/update a resource.

## What does PUT do?
PUT method is used to update resource available on the server

## What does PATCH do?
he HTTP PATCH request method applies partial modifications to a resource. PATCH is somewhat analogous to the "update" concept found in CRUD
