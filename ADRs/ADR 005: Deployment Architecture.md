# Deployment Style for ClearView Solution

## Status
Proposed

## Context
The ClearView platform needs to handle increasing business demands as more companies and candidates join the system.
Scalability is a critical factor, given that the system may need to support significantly larger volumes of candidate profiles, resumes, and job listings over time. Additionally, operating within a cost-effective framework is important due to budget constraints.

**Decision**:
We have chosen to deploy and manage the ClearView platform using a Kubernetes cluster for the initial phase, as it offers a cost-effective solution with the flexibility to scale as needed. This strategy ensures a clear separation of responsibilities within the system while allowing for seamless scalability over time. Additionally, Kubernetes enables us to independently scale different components of our hybrid-modular monolithic architecture, providing both efficiency and adaptability as the platform evolves.


## Consequences
* **Pros**:
  * Easier independent scaling of different services when needed.
  * Helps application stay highly available by self healing and fault tolerance
  * Offers isolation between different services within the system

* **Cons**:
  * Steep learning curve and we need people with devops experience
  * May be unnecessary complexity in the initial stages
