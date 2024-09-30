# Service Based Architecture for ClearView Platform

## Status
Superseded by [ADR #001](ADR%20001%3A%20Architecture%20Decision%20for%20ClearView%20Platform.md)

## Context
In the initial design of the ClearView Platform, there was a need to support scalability and performance, especially under high demand from candidates, hiring managers, and administrators. These demands include handling large volumes of user interactions and the ability to generate reports efficiently.

**Decision**:  
The ClearView Platform was initially built using a service-based architecture that divided the system into separate services, each owning its own data:

* Candidate Service: Managed candidate profiles, resumes, and job applications.
* Hiring Manager Service: Managed job postings, candidate matching, and interview scheduling.
* ClearView Administrator Service: Handled administrative functions and reporting.

The services were designed to be independent, each owning its database, but they were allowed to interact through APIs to share data when necessary. However, this frequent cross-service communication increased the overall system complexity, as services needed constant data access from each other.

## Consequences
* **Pros**:
  * Clear separation of concerns by domain, ensuring each service handled its specific tasks.
  * Independent data ownership per service.

* **Cons**:
  * High communication overhead due to frequent API calls between services, leading to performance bottlenecks.
  * Tight coupling at the data level because services needed to frequently share data, undermining the autonomy of each service.
  * Limited re-usability between services, as each service was highly specialized