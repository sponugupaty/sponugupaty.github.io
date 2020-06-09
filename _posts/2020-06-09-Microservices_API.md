# Microservices And API's

Here's the table of contents:

1. TOC
{:toc}

## Microservices Overview
- Microservices is an architectural style where an application is structured as a group of individual loosely coupled services 
- The services are fine graind and interact with each other using light weight protocols 
- Can use HTTP or RPC 
- Example - E-commerce search , product list , payment , shipping 
- All the services are deployed separately 
- A service can be a single or multiple API's


## Why Microservices ?

- First need to udnerstand monoliths 
- Monolith - Single Unit , SOA - Coarse Grained , Microservices - Fine Grained 
- Advantages of monolith 
	- Simple to develop , deploy and scale 
- Disadvantages of monolithich architecture 
	- Technology dependency - Locked in to use the same technology 
	- Engineering focus - people need to be on the same team to interact with others using the codebase 
	- Scaling the data layer 
	- Overloaded VM's / Containers 
	- CI / CD / Build time - becomes an issue since we need to run all the tests across the board . Code conflicts 
	- Understanding of code 

## Functional Democomposition 
 - smaller modular services 
 - Need to understand the individual components rather than the whole thing
 - each service can be horizontally scaled 
 - Every service should have its own database 
- Enables a polygot architecture 
- Advantages of microservices 
	- scaling is easier 
	- deployment is easier 
	- technology usage 
	- faster to develop and understand 
	- loosely coupled 

- Disadvantages of microservices 
	- Interprocess communication 
	- distributed transactions 
	- more resources 
	- Debugging harder
 
## How to scale microservices 

-  Use the concept of a scale cube on 3 dimensions 
	- Functional decomposition 
	- Horizontal scaling 
	- Data Partioning 

