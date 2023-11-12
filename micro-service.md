# What is a micro-service architecture pattern

It is an approach to software development where the project is composed of small independent services (managed by (typically small) independent teams) that communicate via APIs. This leads to software that develops, adapts, and scales quickly.

<details>
  <summary>What is an API?</summary>
  
  ### Application programming interface <br>
  
  A a mechanism that enables two software components to communicate via a well defined set of definitions and protocols. <br>

  **Application** stands for any software with a distinct function <br>
  
  **Interface** is the set of definitions and protocols, i.e., how two components are contracted to communicate with eachother using requests and responses <br>

  They are useful as a means of abstraction, as they allow a developer to use features/data from a service, application, or platform without any knowledge of the system.
  And since programs communicate via an API, when the programs are further developed the changes should not impact the API, this makes maintenance easier.
</details>

## What is a service

A microservice is a self-contained unit with its own "model" (cf. MVC model), that is, its own business logic and data storage. That is, each service has an entirely seperate codebase and are responsible for persisting their own data/external state: typically this means they have their own databases, note that this adds in the danger of service interactions accidentally changing state, this should not be an issue with proper APIs.

Services communicate via APIs with lightweight protocols, e.g. HTTP (for performance and maintenance reasons).

## Pros

- The modularity they provide allows for individual components to be scaled independently to match demand/resource needs.
- Since different teams maintain different components they are free to implement them however they see fit, this leads to more diversity, innovation, and agility.
- Each component has a smaller codebase, and so it is easier to add new features without unforseen consequences.
- It is possible to handle faults in services, i.e. isolate them so that the entire application is not impacted.

## Cons

# Diagram

# Why we would use it instead of a monolith architecture

The typical example of where a micro-service architecture can be used, is to replace a monolith architecture.

In the monolith paradigm all code is deployed as a single "block", that is, all processes are run as a single service. This is a reasonable thing to do when only a single team is responsible for the monolith, but with more teams there may be conflict, and so development/innovation slows down.Additionally, if there is a sudden spike in a single application of the monolith, to meet demand the whole architecture has to scale.

One solution would be to break the monolith into different components, each of which run a singular application process as a service. Thus solving the main issue of a monolith, scaling.

This seems to be the direction cloud hosted services are trying to push software development, and it seems to be pretty popular with [this article](https://www.meritdata-tech.com/resources/whitepaper/digital-engineering-solutions/microservices-architecture-docker-kubernetes/) claiming that Docker (a service that is used to develop software in "containers") has "Top-notch community support".

# References
https://aws.amazon.com/microservices/ <br>
https://aws.amazon.com/what-is/api/ <br>
https://learn.microsoft.com/en-us/azure/architecture/guide/architecture-styles/microservices
