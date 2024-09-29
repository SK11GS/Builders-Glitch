### Overview of ClearView Engine

ClearView's system relies heavily on AI to drive its core business operations, particularly in generating revenue, fostering trust between candidates and hiring companies, and ensuring effective candidate matching. The goal is to overcome the limitations of existing Applicant Tracking Systems (ATS).

### Driving Factors
To meet these goals, the AI-driven components have been grouped into the core AI engine, which includes the following modules:

* **Resume Enhancer**: Enhances candidate resumes for better matching.
* **Anonymizer**: Ensures anonymization of sensitive information.
* **Talent Match Score**: Provides scoring for matching candidates to job opportunities.
* **S.M.A.R.T Profile**: Provides a structured, detailed profile of candidates for more accurate matching.
* **TalentBridge**: Facilitates communication and interaction between candidates and employers.
* **Company Profile Finder**: Finds and curates profiles for hiring companies.

### Component View
* Diagram will be inserted here

### Supporting Attribute/Rationale 1

Many components, such as the Talent Match Score, Anonymizer, and TalentBridge, can handle jobs asynchronously. This allows for efficient handling of large datasets and AI computations without blocking user interaction.


#### Key Software Architecture Characteristics

    **High Availability**:
    The system must be highly available to support continuous business operations.
    As the services directly impact the trust of both candidates and hiring companies, any downtime would be detrimental.
    Techniques such as load balancing, failover strategies, and cloud-based infrastructure should be considered to ensure this availability.

    **Functional Correctness**:
    The correctness of the AI engine and its components is crucial, particularly in matching candidates effectively.
    Testing strategies, including unit testing and AI model validation, must be prioritized.

### Supporting Attribute/Rationale 2 
Components like Resume Enhancer and Company Profile Finder must perform efficiently in real-time, as these are directly interacted with by users. Any delay in response times can impact user experience.

#### Key Software Architecture Characteristics

    **Performance**:

### Supporting Attribute/Rationale 3
To support high business volume, such as the need to match a large number of resumes with open roles, the architecture must prioritize scalability. This characteristic ensures the system can dynamically adjust its resources based on the demand, maintaining performance during peak loads and optimizing resource usage when the load subsides.
Key Architectural Characteristics: Scalability

#### Key Software Architecture Characteristics

    **Scalability**:
    
    The system must be capable of scaling horizontally by adding more instances of the application during high-demand periods, such as when processing a large volume of resumes and job roles.
    Once the load decreases, the system should automatically reduce the number of instances to optimize resource utilization and lower operational costs.
    
    **Job Queue Processing**:
    
    To handle heavy loads efficiently, jobs such as resume matching should be processed asynchronously using a queuing mechanism.
    This ensures that tasks are distributed and processed independently, without overwhelming the system.
    
    **Load Balancing**:
    
    Load balancing should be implemented to distribute incoming requests evenly across multiple instances of the application, ensuring no single instance is overloaded during peak demand.

### Supporting Attribute/Rationale 4
With the rapid advancements in the AI ecosystem, it is essential that the ClearView engine is designed to seamlessly integrate new technologies and innovations. The system must be flexible enough to evolve as AI models, algorithms, and tools continue to improve. To achieve this, evolvability is prioritized as one of the key architectural characteristics.

Additionally, since the system handles sensitive user data such as resumes and Personally Identifiable Information (PII), security must be prioritized at design levels.

#### Key Software Architecture Characteristics
    **Evolvability**:
    
    System should support continuous enhancements and the incorporation of new AI capabilities
    
    **Modular Design**:
    
    The architecture should follow a modular design, where individual components can be updated, replaced, or enhanced independently. This enables the system to adopt new AI technologies or algorithms without requiring a complete system overhaul.
    
    **Security by Design**:
    
    Given the sensitivity of user data, security must be integrated at the design level. All components that handle PII should implement secure access controls, encryption, and auditing, ensuring data protection and compliance with regulations.

### Top 3 chosen
* Availability
* Scalability
* Evolvability

### Others Considered
* Performance
* Security

### ADR