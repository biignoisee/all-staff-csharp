## Microservices Architecture
A software architecure style where and app is built as a collection of small independt services, each handling a specific business function

### 4 Core Pillars
autonomous
operate efficiently
ownership
agile


1. Autonomy
Independent: self contained with separete resources
  no data sharing
Decoupled:  loosely connected throught REST o gRPC , APIs or Message
  changes made to one service do not force changes of others
Resilient:  Failure in one doesnt affect others
  Implements strategies like retries, circuit breakers or fallbacks
  Critical services have high availability


2. Operate efficiently
Deployable
  Deployed separetly from other services
    respond to business needs quiclky
    works well with CI/CD pipelines
    deployed into its own enviroments and released at different times

Scalable: Scales independetly based on demands
  Scaled up without impact other services


3. Ownership
Business Focus: hanldes one specific business function
  avoiding shared responsabilities
  easier to apply DDD priciples (domain driven design)

Team Owned: fully owned by one team
  flexibilities in choosing tech stack
  small teams get things done more faster

4. Agile
Adapatable: flexible to new buisness needs
  works well with agile methodologies ...
Composable: Easily assembled for a larger solutions
  efficient & expandable



### Benefits & Challenge
Functions independently
Loosely coupled with the other services
Easily deployable
Highly Scalable
Focused one specific business function
Flexible to new business needs
fully owned by one team
Faster development
Freedot to use the optimal tecnologies
easily assembled for large solutions
resilient to failures

the challenge??
data consistency and suncrhonization ...
sync using event-drive updates or schedules sync jobs

increased complexity in multi microservices scenarios
  review sevice
  payment service
  production services tak over for final processing
  article hub  kacknowledged the article satus change

testing , debuggins and monitoring
  testing involves setting up complex enviroments
  monitoring requires correlation techniques ...



## Modular Monolith
An application is signle deployable unit, internally divided into well encapsulated modules
modules each responsible for a specific part of the application

  single deployable unit
  modules have clear boundariies
  can be shared across microservies
  use the same database
  no network obehead
  modules can share or have thei own tech stack
  team nautrally split into sub teaks for modules
  modules align with specific business areas




### Modular Monolith vs Microservices

Independence:  multiple modules share the same enviroment
deployment:  deployed togetheer  with the other modules
scalability:  the entire application is scaled
communication: messages or method-call
data: isolated, different database or schema
technology: some flex in choosing the stack
ownership: ....


#### Real world Example -- File Storage
File Storage at monolith:
  Integrated with a microservices
  Lower operational complexity
  Better performance
  Scales Naturally
  Different security policy
  Fits better the service needs


File Storage at microservices
  Independent scaling needs
  Cross services storage operations
  Company decides on a common file strategy
    cost optimization
    unified security and data governance
    common retention policies
    simplifying development and maintenance




