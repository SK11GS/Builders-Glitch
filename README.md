# Builders-Glitch

# Architecture

As a non-profit organization, the Diversity Cyber Council (DCC) will face budgetary constraints until the ClearView project begins generating revenue. Therefore, the initial solution must be cost-effective and straightforward, with the flexibility to scale as demand grows or when DCC secures additional funding through profits or external investments.

Critical system components, particularly those supporting DCC's core operations, must maintain high availability—ideally around the clock but at least during peak business hours. The availability of business-critical components is crucial since DCC's revenue is directly tied to delivering value to partners, candidates, and hiring managers. Any downtime or inefficiency could negatively impact these relationships and revenue.

Given these considerations, we propose a solution that consists of two core services adopting a hybrid approach:

* **ClearView AI Engine** – to handle all automated tasks powered by AI models
* **ClearView Platform** – to handle other essential business functionalities.

## ClearView AI Engine:
The ClearView AI Engine must be designed for scalability. As the volume of candidate profiles and job postings increases, the system must seamlessly expand to accommodate the growing demand. Since AI model integration is resource-intensive, the infrastructure should efficiently support the increasing demand.

The AI landscape is evolving rapidly with frequent updates and advancements. To maintain a competitive edge and deliver an optimal user experience, the AI Engine should be adaptable, allowing DCC to integrate new AI technologies and improvements as they emerge. This focus is on evolvability, where the system evolves along with the advancements in the AI industry while maintaining its relevance and effectiveness in managing user needs.

### Architecture Characteristic Mapping 
Scalability, Evolvability and Availability

![Architecture Characteristic Mapping](architecture/images/ClearView%20AI%20Engine-Architectural-Characteristics.png "Architecture Characteristic Mapping")

### Chosen Architecture
Event Driven
![Architecture](architecture/images/ClearView%20AI%20Engine-Architecture-Styles.png "Architecture")

## ClearView Platform
ClearView Platform allows key users, including candidates, hiring managers, and ClearView administrators, to carry out their daily activities and interactions. Its primary function is to enable seamless user experiences by handling essential tasks such as onboarding, dashboard management, notifications, and other entity-oriented actions.

While these functions are standard across many software solutions and with AI Engine handling the most resource-intensive workload, we have focused on cost-effectiveness, simplicity, and a domain-driven architecture for the ClearView Platform.

Adopting a domain-driven design ensures the platform efficiently meets current needs while maintaining flexibility for future growth. As the platform expands and new requirements emerge, individual components can be scaled and deployed independently, providing the necessary adaptability.

### Architecture Characteristic Mapping
Cost-effective/Feasibility, Simplicity/Maintainable, Domain Driven according to the capabilities to suppor the extraction of these
into its own services.

![Architecture Characteristic Mapping](architecture/images/ClearView%20Platform-Architectural-Characteristics.png "Architecture Characteristic Mapping")

### Chosen Architecture
Modular Monolith
![Architecture](architecture/images/ClearView%20Platform-Achitecture-Styles.png "Architecture")