# SysML-Past-Class-Project-AVTS

Modeling a Micro-Transit System operated by Autonomous Vehicles (AVTS)

Introduction

This class project explicitly focusses on modelling an Architecture for the deployment of Autonomous Vehicle Technology within a micro-transit system to provide shuttle service over a short-medium distance of about 2 miles, with multiple stops. This work will reflect upon my understanding to define the autonomous vehicle operations over a small grid of routes with a couple of road intersections comprised under a 1.8 square mile area of a micro-transit system, on a real-time and frequent basis within an industrial park facility. The AVTS employs self-driving transit vehicles that perform sensory recognition, cognition/ processing, storage, judgement and control functions necessary to support safe, reliable and efficient movement of passengers. The technology is evolved from the Advanced Driver Assistance System. It enhances vehicle safety, reduces congestion, with level-4 autonomy in Connected & fully Autonomous Vehicles, deployed for easy accessibility, frequent availability, reliability, affordability and safety of commuters.

System Characteristics: Autonomous vehicles possesses real time-sensitive behaviors as it senses the environment and makes driving decisions in free drivable space around it, by perception (monitoring its environment using combined data from subsystem sensors- cameras, short/long-range radars and lidars to detect and classify objects, speed and direction, building a 3d model and map data), motion planning (computing operation to determine desired vehicle behavior while accounting traffic rules and planning the optimum route to desired destination with multiple backup plans) and control (implements final planned path, commands actuators of steering, throttle, braking and transmission subsystems for full maneuverability with stability and traction). This technology enables human-machine interface i.e., vehicles communicate with each other (V2V) and infrastructure (V2I), also possessing non-time-sensitive behaviors of execution and operations.

System Challenges: Integrate the main computing system with signal communications between sub-systems, perception sensors (far-field and near field cameras to recognize, classify and track objects; radar to identify objects and track rate of speed of other vehicles), collision detector (safety backup), vehicle controls (through steering and braking sub-systems) with backup, independent vehicle localization (by lidar), to form simple interfaces and interact with computers, sensors and actuators for alternative operational measures. Detect traffic signals and respond to traffic laws by onboard sensors against map data. Deploy vehicle health monitoring strategy for diagnostics integrated across systems within, to determine vehicle health and perform fallback maneuvers when needed[1].

The System Architecture shall capture functional coverage of the automated driving capabilities in a micro-transit system. In my opinion, this system is complex enought to interpret and respond to the dynamic environment within a facility. It possesses real-time behaviour owing to departure and arrival at the destination within set schedules while executing the operations of perception, motion planning and control. It enables real-time architecting on account of interactions with the surrounding environment through machine perception. Thus, overall this project can be consolidated as a broad-based autonomous ride-hailing services/ delivery service. It also enables an opportunity to practice enterprise architecting of a system ventured by industry and government partners with automakers and software giants provided within a specifically-defined area of a city under supporting weather conditions and shortfalls that shall be addressed in formally modeling the System with Cameo Systems Modeler during the course progress[2].

Architecture Development Resources

The AVTS architecture is developed and maintained through the Model-Based System Architecture Process (MBSAP) implemented in Cameo Systems Modeler, V19.0 SP-3. The estimated architecture development schedule, level of effort, and other required resources are defined in the scope and statement of work provided under the project management plan[3].

Scope

The AVTS architecture is baselined in a model conforming to the Systems Modeling Language (SysML) Profile of the Unified Modeling Language (UML) and includes artifacts in accordance with the MBSAP methodology that define Operational, Logical/ Functional, and Physical Viewpoints (OV, LV, and PV). The model supports visualization of architecture data in various formats as appropriate for technical and programmatic reviews and decisions/ to meet specific stakeholder needs. The AVTS architecture model is the foundation of a Model-based System Engineering (MBSE) methodology that integrates tools, processes, and products for an efficient and effective program of development, integration, test, deployment, and support to realize system requirements.3

Architecture Model and Artifacts

The architecture starts with a requirements baseline, which is refined and updated based on the results of the architecture analysis. It proceeds through Operational, Functional, and Physical Viewpoints, each of which is organized into Perspectives that group artifacts according to the basic aspects of the architecture such as behavior, structure, data, and services. The Operational Viewpoint transforms requirements into an architectural context and establishes the overall organization of the architecture. The Functional Viewpoint instantiates the architecture into a system design, with elements that represent each part of the system solution but without defining specific technologies, products, or standards. Finally, the Physical Viewpoint defines the implementation of the system by adding point design detail. The system then proceeds through build, integration, and test stages, and in a spiral development, the outcome of each architecture cycle is used to refine the requirements baseline and establish the functionality to be implemented. Both a physical prototype and a virtual prototype composed of various system models and simulations tie the process together and support design and analysis at each stage. The process is fully iterative[3].

Primary Artifacts

The following are the primary artifacts to be developed and used to define the AVTS architecture:

Operational Viewpoint: The OV transforms requirements into an architectural context. It includes the following Perspectives[3]:
•	Structural Perspective:
-	Domain Composition Diagram- defines system boundary and context by top-level partitioning (domains) with Block Definition Diagram (BDD).
-	Domain Interaction Diagram- represents the internal structure of domains by ports and flows and associated user roles with Internal Block Diagram (IBD).
-	Specifications- for part property, value property, operations, etc. as prescribed by MBSAP.
•	Behavioral Perspective:
-	Use Case Diagrams- showing primary operations and maintenance behaviors with decomposition and associated User Roles.
-	User Roles Diagram- a specialized Use Case diagram illustrating User Role categories.
-	Activity Diagrams- illustrating scenarios, basic behaviors and the flow of operation thread across Domains.
-	State Machine Diagrams- showing the states at which the AVTS system can be and the transitions among those states, as well any stateful behavior associated with Domains.
-	Specifications- for Use Cases, User Roles, etc.
•	Data Perspective: A Conceptual Data Model (CDM) using BDDs with emphasis on Foundation Classes/ Blocks representing basic categories of information content with Values properties, Operations, and any additional specification content for an unambiguous definition.
•	Services Perspective:
-	Domains and their interfaces, ports annotated to describe Services that are supported and exposed.
-	A Services Taxonomy is developed top identify internal and external Services, and allocated to Domains.

Logical/ Functional Viewpoint: The LV begins with functional system design. It includes the following Perspectives:3
•	Structural Perspective- BDDs and IBDs showing decomposition of Domains, interaction among system elements and with external entities, associated User Roles, and specifications.
•	Behavioral Perspective:
-	Sequence Diagrams- illustrating how groups of Blocks, User Roles, external entities, and others collaborate to realize stateless behavior. Includes timing annotation.
-	State Machine Diagrams- illustrating stateful behavior of individual Blocks.
•	Data Perspective: A Logical Data Model (LDM) using BDDs to decompose the CDM to instantiate system data entities with inheritance from Foundation Classes in the CDM.
•	Services Perspective: Blocks and their interfaces, Ports annotated to describe services that are supported and exposed. Allocation of services to Blocks, Flows and Interfaces.    
•	Contextual Perspective: A wide range of supplementary information and documents which cannot be captured in other perspectives can be assembled and incorporated into the model.

Physical Viewpoint: The PV implements logical components with physical product specifications. It includes the following Perspectives:3
•	Design Perspective: adding details to the elements of the functional viewpoint to document architecture implementation in a point design.
•	Standards Perspective: A Standards Profile with approved protocols and standards.
•	Data Perspective: A Physical Data Model (PDM) showing detailed design of databases.
•	Services Perspective: adding detail to service interface specifications, complying with appropriate standards, to the Services Taxonomy. 
•	Contextual Perspective- A wide range of supplementary information and documents, training material, maintenance manuals, etc. can be assembled and incorporated into the model[3].

Architecture Purpose and Uses

The purpose of the architecture is defined in terms of specific stakeholder needs to be met, like:
•	Support to technical and programmatic decisions based on the impact of decision alternatives on overall system technical integrity and achievement of objectives.
•	Requirements analysis and refinement (baseline), including stakeholder dialog with system users and support organizations.
•	Development of performance, design, and procurement specifications.
•	Performance, design and other trade studies.
•	System design and analysis (functional analysis and allocation/ baseline)
•	Standards selection and application.
•	Other system engineering processes[3].

Recommendations

•	The AVTS system architecture should proceed to implementation, including detailed design, integration, and test, following the methodology defined in this report.
•	Quality Attributes should be tracked, analyzed, and reported as the basis for ensuring overall technical integrity of the solution and satisfaction of all stakeholder needs.
•	The architecture model and artifacts, as well as virtual prototypes should be placed under rigorous configuration and change control.
•	Other recommendations shall be added as implementation and operational support of the system proceed [3].

References

[1] A matter of trust. Ford’s approach to developing self-driving vehicles.
[2] Todd Litman (2013-2019) et al Autonomous Vehicle Implementation Predictions.
[3] Appendix C: System Architecture Example: E-X Airborne Multi-Sensor Platform. Effective Model-Based Systems Engineering, John M. Borky, Thomas H. Bradley. https://doi.org/10.1007/978-3-319-95669-5
