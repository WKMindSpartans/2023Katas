# Architectural Decision Record
## Date
9/13/23 

## Title
Road Warrior will use a microservices architecture

## Status
Accepted

## Context

The Road Warrior App requires several different components including frontend, services, and data storage techniques. To kickoff things we must decide on a high-level architectural style that will be used to enable these requirements.


## Decision

We will use a microservces architecture style.


## Consequences

#### Positive
* Microservices enables extensibility: new functions can be implemented by creating new capabiltiy services
* Scalability: there are many methods to orchestrate services based on changing load
* Usuability: By making the architecture extensible, we can make it easier to add new functionality

#### Negative
* Costs are quite high due to unused compute time, etc.
* Additional complexity: troubleshooting is harder


#### Risks
* Data consistency: Without additional considerations we have very few guarentees that data will be consistent across services. This likely isn't a huge concern given the use-cases we must support, but should be recognized.
* Regressions: Without more complex end-to-end test frameworks it is much harder to verify that changes in one service don't break others.

