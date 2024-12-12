### Both cloud native development practices and microservices architectures put an emphasis on _____, while building into your application and system as a whole.


 - reliability
 - manageability
 - availability
 - > scalability




### If you need to provide modified payloads that meet the need of a third-party contract, which service type would you use?

 - data service
 - business service
 - > edge service
 - translation service




### What should be your first step when building a business process service?

 - defining the domains
 - defining the APIs
 - > defining the process



### When building services around data domains, what do you need to start with?

 - > the model
 - the datastore
 - the actions



### Which decomposition pattern allows you to deploy components of an application into separate functional components alongside the main service component?

 - > the sidecar pattern
 - the strangler pattern
 - the proxy pattern
 - the bulkhead pattern



### You are designing an atomic transaction, and your underlying data domains do not currently share a database. What should you do?

 - Keep the domains in separate databases.
 - Give each service implementation its own datastore.
 - > Merge the domains into a single shared database.



### What is the main purpose of the sidecar pattern?

 - to control tasks to prevent resource exhaustion
 - to shard services off your monolith piece by piece
 - to provide a substitute for another object
 - > to remove repetitive code across services



### What is the main purpose of the strangler pattern?

 - to provide a substitute for another object
 - > to shard services off your monolith piece by piece
 - to control tasks to prevent resource exhaustion
 - to remove repetitive code across services



### Why does the edge pattern have a more scalable component over the gateway pattern?

 - > It targets a single client.
 - It keeps clients in sync.
 - It has fewer moving parts.
 - It targets multiple clients.



### How does the process aggregator pattern help you if you have several business processes that must be called together and have a composite payload?

 - by producing a choke point in your system
 - by producing a blocking call for the API
 - > by providing clients with a single API to call



### What is your second step when designing a process aggregator pattern?

 - determining the business process
 - designing a consolidated model
 - designing an API for the actions on your model
 - > determining the processing rules



### What is your first step when building a gateway pattern?

 - > defining your contracts
 - exposing APIs in your gateway component
 - identifying the client
 - implementing the gateway




### In a single service database, as your service scales, what happens to your datastore?

 - > The datastore scales proportionally to the service.
 - The datastore scales up as the service scales down.
 - The datastore scales down as the service scales up.



### When should you use asynchronous eventing?

 - > when you have a complex workflow that cannot fit into a single, blocking API call
 - when you have a simple workflow that cannot fit into a single, blocking API call
 - when you have a complex workflow that will fit into a single, blocking API call
 - when you have a simple workflow that will fit into a single, blocking API call



### In which case is using CQRS common?

 - with event-based UI operations
 - with asynchronous UI operations
 - > with task-based UI operations



### To ensure that you have proper segmentation, what should each schema and each service that consumes data have?

 - scalability benefits
 - unique databases
 - > unique credentials
 - identical credentials




### How should secrets be externalized in most implementations?

 - through transparent communication
 - > through special constructs
 - through published documents



### Where should the trace ID be injected?

 - > into the entry point of your system
 - into a tag on the log message
 - into the median point of your system



### Why is metrics aggregation considered easier than log aggregation?

 - > There is less human interaction.
 - There is more human interaction.
 - The developer writes and structures the message.
 - You are only looking for a code output.



### While log aggregation takes on many forms, where do all the logs end up?

 - > in a single stream of data
 - in the same domain
 - in different domains
 - in separate streams of data

