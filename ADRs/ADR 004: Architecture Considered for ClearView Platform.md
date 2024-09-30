# Service Based Architecture for ClearView AI Engine

## Status
Superseded by [ADR #001](ADR%20001%3A%20Architecture%20Decision%20for%20ClearView%20Platform.md)

## Context

**Decision**:  


## Consequences
* **Pros**:
  * By scaling and managing services independently, organizations can optimize their infrastructure and resource utilization, leading to cost savings.
  * Easier to integrate with third-party services or legacy systems.
  * Allows services to be developed, maintained, and deployed independently.

* **Cons**:
  * Increases complexity compared to monolithic architectures, as you have to manage multiple services instead of a single application.
  * Introduces communication overhead, including latency, potential failure points, and the need for robust error handling.
  * Need to manage separate pipelines for each service.