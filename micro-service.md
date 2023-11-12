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



# Pros

# Cons

# Diagram

# Why we would use it instead of a monolith architecture

The typical example of where a micro-service architecture can be used, is to replae a monolith architecture.

In the monolith paradigm all code is deployed as a single "block", that is, all processes are run as a single service. This is a reasonable thing to do when only a single team is responsible for the monolith, but with more teams there may be conflict, and so development/innovation slows down.Additionally, if there is a sudden spike in a single application of the monolith, to meet demand the whole architecture has to scale.

# References
https://aws.amazon.com/microservices/ <br>
https://aws.amazon.com/what-is/api/
