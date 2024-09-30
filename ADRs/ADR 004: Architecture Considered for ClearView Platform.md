# Service Based Architecture for ClearView AI Engine

## Status
Superseded by [ADR #001](ADR%20001%3A%20Architecture%20Decision%20for%20ClearView%20Platform.md)

## Context
The ClearView platform needs to handle increasing business demands as more companies and candidates join the diversity of inclusion programs. 
Initially, the platform is expected to manage moderate user traffic and CRUD operations, but it must be designed with the ability to scale in the future as the user base grows. Scalability is a critical factor, given that the system may need to support significantly larger volumes of candidate profiles, resumes, and job listings over time. Additionally, operating within a cost-effective framework is important due to budget constraints, and time-to-market is a priority to validate the platform in its initial phase.

**Decision**:  
We decided to structure the ClearView platform using **modular monolith** architecture for the initial phase, which is both cost-effective and allows for quick time-to-market. This approach will enable clear separation of responsibilities within the system while allowing it to scale over time. The modular monolith design also enables a smoother future transition to microservices, should the need arise to scale components independently.

## Consequences
* **Pros**:
  * By scaling and managing services independently, organizations can optimize their infrastructure and resource utilization, leading to cost savings.
  * Easier to integrate with third-party services or legacy systems.
  * Allows services to be developed, maintained, and deployed independently.

* **Cons**:
  * Increases complexity compared to monolithic architectures, as you have to manage multiple services instead of a single application.
  * Introduces communication overhead, including latency, potential failure points, and the need for robust error handling.
  * Need to manage separate pipelines for each service.