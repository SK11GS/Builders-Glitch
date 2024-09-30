# Title
Deployment Style for ClearView Solution

## Status
Proposed

## Context
The ClearView platform needs to handle increasing business demands as more companies and candidates join the system.
Scalability is a critical factor, given that the system may need to support significantly larger volumes of candidate profiles, resumes, and job listings over time. Additionally, operating within a cost-effective framework is important due to budget constraints.

**Decision**:
We decided to use kubernetes cluster to deploy and manahe the ClearView platform for the initial phase, which is both cost-effective and allows us to scale when needed. This approach will enable clear separation of responsibilities within the system while allowing it to scale over time. Using kubenetes cluster also allows us to scale different parts of the system in our hybrid-modular monolith architecture.


## Consequences
* **Pros**:
  * Easier independent scaling of different services when needed.
  * Helps application stay highly available by self healing and fault tolerance
  * Offers isolation between different services within the system

* **Cons**:
  * Steep learning curve and we need people with devops experience
  * May be unnecessary complexity in the initial stages
