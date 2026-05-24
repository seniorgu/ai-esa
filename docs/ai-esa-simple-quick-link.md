# AIS (AI Solution) Elements - A Quick Reference

| **Category**           | **Name**             | **Prefix** | **Definition**                                                                                                                                         |
| ---------------------- | -------------------- | ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Intent & Metrics       | Intent               | IT         | Represents the strategic intent, value drivers, and guiding principles that justify and direct the solution.                                           |
| Intent & Metrics       | Capability           | CP         | Represents the business, technical and AI abilities the solution enables or delivers.                                                                  |
| Intent & Metrics       | Requirement          | RQ         | Represents the functional and non-functional needs, scenarios, quality expectations, and acceptance criteria the solution must satisfy.                |
| Intent & Metrics       | Governance           | GV         | Represents the principles, policies, compliance obligations, ethical controls, and accountability structures that guide responsible solution behavior. |
| Intent & Metrics       | Decision             | KC         | Represents the key architectural choices, evaluated trade-offs, and rationale that shape the solution design.                                          |
| Functional             | Access Interface     | UI         | Represents the interaction channels, UI/UX surfaces, and entry points through which humans engage with the solution.                                   |
| Functional             | Application          | AP         | Represents a bounded software system, enterprise application, or business component that integrates with or consumes AI capabilities.                  |
| Functional             | App Logic            | AS         | Represents explicitly defined non-GUI logic, control flow, or compositional behavior of an application.                                                |
| Functional             | Data Service         | DS         | Represents services responsible for data access, integration, transformation, federation, and transactional integrity.                                 |
| Functional             | Technical Component  | TS         | Represents reusable technical capabilities, utility services, and cross-cutting infrastructure functions available across the solution.                |
| Functional             | Interface Contract   | SI         | Represents the defined interface, contract, API, or protocol through which components expose and consume capabilities.                                 |
| Functional-AI Specific | AI Agent             | AG         | Represents an autonomous AI entity capable of goal-directed reasoning, planning, and action.                                                           |
| Functional-AI Specific | AI Orchestrator      | AC         | Represents the coordination logic, workflow control, and multi-agent management that sequences and routes AI operations.                               |
| Functional-AI Specific | Context State        | CN         | Represents the mechanisms for managing conversational state, memory, prompt engineering, and interaction coherence.                                    |
| Functional-AI Specific | AI Model             | ML         | Represents the models, inference engines, and reasoning frameworks that generate predictions, decisions, or outputs.                                   |
| Functional-AI Specific | Knowledge Service    | KA         | Represents the semantic retrieval, RAG, embedding, and knowledge management capabilities that ground AI responses in relevant information.             |
| Functional-AI Specific | AI/ML Lifecycle      | AL         | Represents the lifecycle management processes for model training, experimentation, versioning, and deployment.                                         |
| Functional-AI Specific | Tool                 | TL         | Represents external functions, plugins, and third-party services that extend AI capabilities through invocation.                                       |
| Operational            | Data Store           | DB         | Represents the repositories where structured, unstructured, or semi-structured data is persisted and managed.                                          |
| Operational            | Deployment Package   | DP         | Represents a discrete, deployable and scalable package of software or functionality.                                                                   |
| Operational            | Node                 | ND         | Represents the physical and virtual compute resources that host and execute the solution.                                                              |
| Operational            | Quality & Adaptation | QV         | Represents the testing, validation, and continuous improvement mechanisms that assess solution quality and performance.                                |
| Operational            | Governance Control   | GO         | Represents the operational controls, policy enforcement, observability, security monitoring, and human oversight mechanisms active during execution.   |
| Operational            | Middleware           | MW         | Represents the system and platform software, middleware, and services that underpin application execution and integration.                             |
| General                | Group                | GP         | Represents a logical or functional organizational structure used to partition, layer, or modularize the architecture.                                  |
| General                | Role                 | RO         | Represents the individuals, roles, personas, or entities that interact with or have a stake in the solution.                                           |
| General                | Task                 | TK         | Represents discrete activities, process steps, decisions, and work units performed by humans or automated systems within the solution.                 |
| General                | Input                | IN         | Represents the data, signals, queries, and information consumed by the solution.                                                                       |
| General                | Output               | OU         | Represents the results, recommendations, and responses produced by the solution.                                                                       |
| General                | Note                 | NT         | Represents commentary, annotation, or interpretive explanation of the architecture.                                                                    |

Usage Notes

- As an agile element set, naming may be adapted to reflect solution-specific needs. *Assistive* or instance-specific naming (e.g., RQ-NFR for non-functional requirements, ZN for zone as a group/domain element) is permitted but should be used sparingly, with each assistive element explicitly mapped to its corresponding base element in this table.

- For *connection relationships*, only association and flow link types are used, where flow represents directionality, triggering, access, serving, dependency, and influence relationships, in the interest of simplicity and consistency. Composition relationships can be represented using the *Grouping* element or through labeled relationship links.

- A *Bot* may be classified as either an AI Agent or an Autonomous Tool depending on its architectural role and decision-making scope. For example, a conversational bot with reasoning autonomy is generally an AI Agent; a rule-based, deterministic bot is generally an Autonomous Tool.

- AIS is based on the *ESA specification*, extended with AI-specific elements, but uses only a subset of the foundational ESA elements for simplicity. The excluded ESA elements can be represented through alternative elements or relationship links. For example:
  
  - *Constraint* (e.g., problem, issue, risk, assumption) is represented as part of the *Requirement* element, or within the *Governance* element (e.g., compliance constraints).
  
  - *Message & Event* are represented through the *Interface Contract* element, or indicated via labeled relationship links.
  
  - *System* can be represented by either the *Interface Contract* or *Application* element, depending on context.
  
  - Granularity-related elements such as *Domain* and *Viewframe* (drill-down construct) are represented using the *Grouping* element.
  
  - Solution management or software design elements such as *Deliverable* and *Artifact* are represented using *Output* or *Note* elements.&nbsp;
  
  - Physical equipment and *Robotic Systems* are not core AIS elements. When relevant, they should be represented as *System Device* elements or external system actors.
  
  - Infrastructure concerns such as networks and storage topology are not core AIS elements, as they are peripheral to solution-level architecture. *Network* and *Location* elements are part of the broader ESA specification but are excluded from AIS scope.
