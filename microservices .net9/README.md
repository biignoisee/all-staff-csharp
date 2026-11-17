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

