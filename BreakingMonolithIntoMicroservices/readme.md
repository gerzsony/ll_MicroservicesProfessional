### Which components does the monolith consist of?

 - The monolith is - as the name says - monolithic and does not have any structure to it.
 - It's a frontend and a backend.
 - > models, views and controllers as well as a persistence layer with databases
 - It's a MVVM system.



### Why should you consult with key stakeholders before starting your initiative?

 - > to understand their requirements and expectations and create measurable goals that provide business value
 - to start splitting up the teams into smaller service teams
 - to explain to everyone what you are about to do and what they should expect to happen
 - to explain to everyone how to move out the logic in their responsibility into microservices



### What is a valid reason to move to microservices?

 - doing the long due redesign of the website
 - moving the whole stack into the cloud
 - to switch to Kubernetes
 - > increasing the frequency of new releases and with that speeding up innovation



### Which service does Cheapr! provide?

 - > It's a price comparison page that shows very to get an item for the cheapest price.
 - It lets you find cheap journeys to destinations around the globe.
 - It's a comparison site for insurances and helps you find the cheapest supplier.
 - It's a webshop for cheap retail and bulk items.



### What is a good reason to refactor code instead of doing a rewrite?

 - If the team does not have time for a rewrite just now.
 - If a controller can be directly mapped to a service.
 - Refactoring is always the preferred approach. It's about splitting up code and not rewriting the whole application.
 - > If the code is complex and self contained and does not have dependencies to the rest of the application.



### What is NOT a common design mistake when moving to microservices?

 - designing services that provide exactly one function
 - > designing services that provide exactly one capability
 - sharing a database between services to provide a shared state
 - sharing code between microservices to avoid redundancies



### How can we create services that still rely on data owned by the monolith?

 - by running a job that copies data to a migration database to be used by the services that need it
 - > by creating a migration API on the monolith that provides endpoints that are similar to those later provided by dedicated services
 - You have to plan the migration so that this doesn't happen. A service must not call back into the monolith.
 - by exposing the monolith's database to the microservices



### What would be a reason to make the user interface part of the respective services?

 - > a service team that owns all tiers from persistence to presentation can innovate independently
 - creating and operating a composite frontend is easier compared to monolithic frontends
 - returning just the data is generally slower than sending the rendered HTML partial
 - an HTML page that is created from various services will render faster as the load is distributed



### What is the tool of choice to migrate to new functionality on-the-fly?

 - blue/green deployments
 - > feature toggles
 - a second monolith serving the new code
 - a migration API




### What is a main asset of cloud providers that might want you consider using them as you create your services?

 - They are more secure than running things locally.
 - > They provide managed utility services, like databases or serverless functions that can be used without much operational effort.
 - They are generally cheaper than running services on premise.
 - They are usually faster.



### What is a good capability to migrate first?

 - a central capability as many other services will later depend on it - so let's move it out first
 - a capability that isn't used frequently
 - a capability that does not connect to a database
 - > a rather small capability that does not have many dependencies - a so called "edge service"



### What changes need to be done on the monolith to accommodate a new service?

 - > You replace in-process calls with calls into the microservice whenever a capability is used.
 - You don't change the monolith but wait for the whole migration to complete and switch over to the new infrastructure.
 - You create a migration API that provides an interface to all the services.
 - You reduce the reserved memory and compute as the service now takes parts of the load.



### What should you do once all business logic has been moved into services?

 - > Replace the leftover monolith with a more lightweight middleware platform.
 - Do load tests and install monitoring to make sure everything runs smoothly.
 - Nothing. The migration is done and the monolith now acts as middleware.
 - Create service teams that operate the new services.



### Why do you need Continuous Integration (CI) when developing microservices?

 - > Locally, a developer can not test how the respective service works in conjunction with the rest of the application. Continuous Integration ensures that each change is tested with the application at large, providing immediate feedback to the developer.
 - CI ensures that services are continuously tested and can be rolled out into production.
 - CI ensures that services could be rolled out into production at any given time.
 - It's just modern and when moving to microservices, this is a logical next step.




### Why should you switch to monitoring before starting your microservice migration?

 - to optimize the monolith before attempting the migration
 - to make sure that the monolith is not broken
 - to learn how to use the monitoring service
 - > to create a baseline to verify that the microservice migration does not cause a performance degradation




### How should API documentation be created?

 - The documentation should be in the respective code.
 - > It should be auto-generated from the actual code in real-time.
 - The code should be self-explanatory and no documentation should be needed.
 - It should be maintained on a documentation page run by the docs team.



### What does Inner Source mean?

 - Everyone can change any code anytime.
 - The development is done on GitHub.
 - > Apply the same rules and processes that are known to work from open source development to proprietary software development inside a company.
 - The code by one team can be used by other teams.



### What can Conway's law tell us about software architecture?

 - > The architecture of an application mirrors the structure of the organization that built it.
 - You have to have small teams to build proper software.
 - It's important that teams have proper communication channels.
 - Documentation is important.


