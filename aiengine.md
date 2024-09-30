### Overview of ClearView AI Engine
ClearView's solution heavily relies on AI to drive its core business function, particularly in generating revenue, fostering trust between candidates and hiring companies, and ensuring effective candidate matching. 

### System Components
The components below constitute the ClearView AI Engine, which handles core business functionalities.

* **Resume Enhancer** component provides resume improvement and refinement tips,   
* **Anonymizer** eliminates all sensitive information from the resume to prevent any hiring bias.   
* **S.M.A.R.T Profile** provides a structured, detailed profile of the candidate using SMART methodology for more accurate matching.  
* **Talent Match Score** provides a match score that determines a candidate for the job opportunity fit.   
* **Talent Bridge**: Matches the candidates to job postings.  
* **Company Profile Finder**: Assists the company’s onboarding process by suggesting publicly available company data.

### Component View
![ClearView AI Engine](architecture/images/ClearView%20AI%20Engine-C3_Diagram.png "ClearView AI Engine C3 components view")

### Architectural Characteristic Mapping

#### Feature 1
Components such as the Talent Match Score, Anonymizer, and Talent Bridge can handle jobs asynchronously, allowing for efficient handling of large datasets and AI computations without blocking user interaction.
This emphasizes the need to ensure high availability for these components and any systems that rely on them.

> **High Availability**
   * The system must be highly available to support continuous business operations.
   * As the services directly impact the trust of both candidates and hiring companies, any downtime would be detrimental.
   * Techniques such as load balancing, failover strategies, and cloud-based infrastructure should be considered to ensure this availability.

> **Functional Correctness**
  * The correctness of the AI engine and its components is crucial, particularly in matching candidates effectively.
  * Testing strategies, including unit testing and AI model validation, must be prioritized.

#### Feature 2 
Components like Resume Enhancer and Company Profile Finder must perform efficiently in real-time, as users interact with them directly. Any delay in response times can impact user experience.

> **Performance**
   * The system should be optimized for speed and responsiveness, ensuring efficient processing and quick response time

#### Feature 3
The architecture must prioritize scalability to support high business volume, such as the need to match a large number of resumes with open roles. This characteristic ensures the system can dynamically adjust its resources based on demand, maintaining performance during peak loads and optimizing resource usage when the load subsides.

> **Scalability**
   * The system must be capable of scaling horizontally by adding more application instances during high demand.
    
> **Job Queue Processing**
   * To handle heavy loads efficiently, tasks such as resume matching should be processed asynchronously using a queuing mechanism. This ensures that tasks are distributed and processed independently without overwhelming the system.
    
> **Load Balancing**
   * Load balancing should be implemented to distribute incoming requests evenly across multiple application instances, ensuring no single instance is overloaded during peak demand.

#### Feature 4
With the rapid advancements in the AI ecosystem, the ClearView engine must be designed to integrate new technologies and innovations seamlessly. The system must be flexible enough to evolve as AI models and algorithms continue to improve. Evolvability is prioritized as one of the key architectural characteristics to achieve this.

> **Evolvability**
  * ClearView AI Engine should support continuous enhancements and the incorporation of new AI capabilities
     
> **Security by Design**
  * Given the sensitivity of user data, security must be integrated at the design level. All components that handle PII should implement secure access controls, encryption, and auditing, ensuring data protection and compliance with regulations.

### Top 3 chosen
* Availability
* Scalability
* Evolvability

### Others Considered
* Performance
* Security

### ADR
* [ADR #002](ADRs/ADR%20002%3A%20Architecture%20Decision%20for%20ClearView%20AI%20Engine.md)
* [ADR #003](ADRs/ADR%20003%3A%20Architecture%20Considered%20for%20ClearView%20AI%20Engine.md)
