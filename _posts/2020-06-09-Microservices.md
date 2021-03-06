# Technology : Microservices

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
	
## API Gateway 

- One of the key uses of API GW is "ÄPI Composition"
- BFF pattern - Essentially a gateway for each of the channels like Web , mobile , 3rd party
- Also possible to have different gateways for different devices - Android , ioS
- Used to track usage and rate limit the API's
- Advantages of API GW 
	- Authentication 
	- SSL termination 
	- acts as a load balancer 
	- Insulation - no direct contact to the API's
	- Caching 
	- managing access quotas 
	- API versioning
- Disadvantages of API GW
	- Increases the number of hops 
	- Adds layer of complexity 

## Service Registry 

- Helps keep track of all the instances / port numbers of containers running the services 
- 2 ways this is maintained 
	- Self registry ( each container self registers )
	- third party registry ( Service register polls the microservices )
- Service Discovery 
	- useful when the client wants to talk to the services directly (without the GW )
	- Useful for the GW to poll the service registry as well 

## Interservice Communication 

- Synchronous calls can happen in realtime in a simple way 
- Disadvantage  - service availability and response times 
- Asynchronous calls between API's using queues 
- Advantages of asychronous -
	- Faster API's
	- Decoupled services 
	- no need for service discovery 
- disadvantages of asynchronous calls 
	- complex design 
	- process latency 
	- monitoring costs
## Misc

- Circuit breaking pattern is useful when the microservices interact among each other 
- if there is a dependency between services and one of the services fails to respond 
- In order to provide an opportunity for the failed service to recover
	- Circuit breaking allows sending cached responses back to client
	- Calling a third party service with similar functionalty ( fallback )
- Some issues with the inter communication between microservices 
	- Load balancing 
	- service discovery 
	- Collecting metrics 
	- Retries 
	- circuit breaking 
	- timeouts
- Service Mesh is deployed with each microservice to take care of the issues above 
	- This is called a sidecar pattern
	- Acts as a proxy between microservices 
	- 2 key things control plane and data plane 
- Deployment Patterns 
	- Considerations for deployment  
		- scalability and throughput 
		- reliability and availability
		- Isolation 
		- resource limit 
		- monitoring 
		- cost effective 
	- A few patterns 
		- Multiple services per host 
		- Advantages 
			- fast deployment 
			- cost effective
		- disadvantages 
			- poor isolation 
			- no resource limit 
			- dependency conflict 
		- service per container / VM
		- Advantages 
			- Isloation and secure 
			- manageable
			- fast ( containers only )
			- autoscaling 
		- disadvantages 
			- slow ( VM only )
			- not efficient ( VM only )
			- not so secure 
		- Serverless 
		- advantages 
		- focus on code 
		- no worries about scaling 
		- pay as you go 
		- disadvantages 
		- debugging pain 
		- vendor lock 
		- run time environments
		- expensive 


