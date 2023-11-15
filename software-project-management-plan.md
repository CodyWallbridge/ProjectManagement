# U↑ Software Project Management Plan
**Version:** 1.0
**Date:** November 24, 2023
**Team Name:** Shaowei's Angels

## VERSION HISTORY
| Version # | Implemented By | Revision Date | Approved By | Approval Date | Reason |
|-----------|----------------|---------------|-------------|---------------|--------|
| 1.0       | Mia            | 11/13/23      | Mia         | 11/13/23      | Added Template. |
| 1.1       | Cody           | 11/14/23      | Everyone    | 11/14/23      | Added introduction and project organization. |

## 1 INTRODUCTION
The Software Project Management Plan (SPMP) for the U↑ project defines the project management goals of the project and includes a description of the deliverables and deadlines. As the world shifts rapidly towards remote working and digital collaboration, the demand for advanced, cloud-based communication solutions is surging. Recognizing this trend, our client seeks to develop a comprehensive, cloud-based telephony system, "U↑". This system is designed to revolutionize communication within businesses by providing a versatile platform that supports making and receiving calls via the internet, rather than traditional landline connections. The primary goal of this project is to create a user-friendly, scalable virtual phone system that integrates seamlessly with desktop and mobile devices, enabling users to manage all communication under one unified business number. This innovation aims to cater to the evolving needs of modern businesses, providing a more flexible, efficient, and cost-effective communication solution. The SPMP for "U↑" details the steps, resources, and timeline required to turn this vision into a reality, ensuring that the final product aligns perfectly with the client's expectations and the market demands.

The U↑ team consists of: Mia Battad, Daniel La Rocque, Barbara Guzman Romero and Cody Wallbridge.
### 1.1 Project Overview
This section of the Software Project Management Plan (SPMP) gives an overview of the purpose, scope, and objectives of the project. It also contains sections regarding the assumptions and constraints, the project deliverables, the summary of the schedule, and the plan for change in the SPMP. 

### 1.1.1 Purpose, scope and objective
The objective of the project is the development of the U↑ platform. U↑ is an internet-based phone system for company employees. Employees can make and receive calls over the Internet using their desktop computers, smartphones, tablets, or other devices connected to the U↑ system. Each of the user's devices connected to U↑ will be associated with a unique business phone number for incoming and outgoing calls. Any connected device can make or receive calls using U↑ whenever and wherever necessary.

The project will take place over an estimated 12 months, with an estimated budget of $500K.

### 1.1.2 Assumptions and constraints
There are several assumptions and constraints that are of importance for the project and its team members.

#### 1.1.2.1 Assumptions

1. **Client-Server Communication**: The system architecture will support seamless interaction between multiple clients and the central server via sockets.
2. **Database Integrity**: The database, potentially supporting the system, will maintain a consistent state even with concurrent access from call processing and administration.
3. **Billing Accuracy**: The system can calculate bills with high precision to avoid discrepancies.
4. **Client Adaptability**: All versions will provide a uniform user experience across clients using desktop, mobile, etc...
5. **Singular Administrator Access**: Only one Administrator accesses the System Console at a time.

#### 1.1.2.2 Constraints

1. **4-Digit Dialing**: The system has an inherent limitation on the number of unique extensions with a 4-digit dialing plan.
2. **Socket-Only Communication**: The mandate that communication should exclusively occur over sockets restricts alternative communication methods.
3. **Load Limits**: The system has an upper threshold for the number of concurrent calls it can handle, determined by the Administrator.

### 1.1.3 Project Deliverables
| Major Deliverable | Deliverable Description |
| ----------------- | ----------------------- |
| Architecture design document | A high-level document describing the functional requirements and system architecture for the U↑ system. |
| Client app UI mock-ups | Interactive user interface mock-ups representing how the U↑ mobile and desktop apps will look and respond to user interaction. |
| System back-end and console | Server software and database for the U↑ system that can be interacted with and tested through an administrator console. |
| Client app integration | Functional client applications that connect to the U↑ back-end and database to make and receive calls. |
| System metrics & performance report | A report detailing the measured increases in efficiency, customer satisfaction, and system availability after implementing U↑ within the company. |

### 1.3 Evolution of SPMP
The SPMP for the U↑ project will be under version control, so any changes will be made to the plan itself. The updated document will be made available to all project members and interested stakeholders. The most recent version will also be available in the U↑ repository.

### 1.4 Schedule
| Executive Milestones | Estimated Completion Time frame |
| -------------------- | ------------------------------ |
| Project plan created and approved | 2 weeks after Project Charter's initial draft is completed |
| Visual prototypes developed | 8 weeks after requirements are finalized |
| Software version 1 completed | 16 weeks after prototypes are completed |
| Security and load testing of system | 4 weeks after completion of Version 1 |
| Limited integration of system into company | 2 weeks after security and load testing |
| Full system integration into company | 8 weeks after limited system integration |

## 2 PROJECT ORGANISATION
The SPMP will identify the organizational entities external to the project and their interaction with the project team, as well as internal project structure and roles and responsibilities for the project. Section 2.1 describes the external interfaces to the U↑ project team, section 2.2 describes the internal structure of the team, while section 2.3 describes the roles performed by the team members.

### 2.1 Process Model
The U↑ project will follow an incremental and an iterative development model for its deliverables. The development will be done in several phases and each phase will represent a complete development cycle, with certain functionality of the system delivered at the end of each phase The phased approach to delivery provides flexibility in what the team will deliver, gives an opportunity to reassess the effort for each phase and allows both the team and the client to change any of the phase’s content.

### 2.2 Organisational Structure
#### The project team follows a hierarchical internal structure within the following levels:
- **Director/CEO**
  - **Project Manager**
    - **Team Lead**
      - **Development Manager**
        - **Developers**
      - **Planning Manager**
      - **QA Manager**
      - **Support Manager**
    - **Sales Representative**
    - **IT Department**

#### The external parties with interest or influence on U↑'s development include:
- **Client Company**
- **Investors**
- **Future External Companies**
- **Technology Manufacturers**
- **General Public**

### 2.3 Organisational Boundaries
#### 2.3.1 Inclusive Boundaries

- Support calls inside the client company.
- Support audio and text.
- Support major tech hardware and software.

#### 2.3.2 Exclusive Boundaries

- No integration with other calling software.
- No support for calls outside the client company.
- No support for video calls.

### 2.4 Project Responsibilities
#### 2.4.1 Internal Roles and Responsibilities

| Name & Organization | Project Role | Project Responsibilities |
| ------------------- | ------------ | ------------------------ |
| Sales Representative     | Project Team Member  | Market the product by communicating its purpose and features |
| IT Department            | Project Team Member  | Support the onboarding of customers and requests from the developers |
| Developers               | Project Team Member  | Engage in day-to-day activities, be on call when needed, technical writing, and contribute to project success |
| Team Lead                | Project Team Member  | Monitor team progress, ensure the team stays on track, run work breakdowns, organize work assignments and provide updates to Project Manager |
| Project Manager          | Project Team Member  | Ensure Team Lead is familiar with requirements, provide updates to Director/CEO, break tasks |
| Director/CEO             | Project Sponsor      | Ensure Project Manager is up to date on the requirements and update Investors if needed |

#### 2.4.2 External Roles and Responsibilities

| Name & Organization      | Project Role                 | Project Responsibilities |
| ------------------------ | ---------------------------- | ------------------------ |
| Investors                | Secondary Stakeholder        | Provide financial support to the project |
| Client Company           | Customer                     | Provide feedback and requests |
| General Public           | Future Customer              | Offer future feedback and requests |
| Future External Companies| Future Customer              | Offer future feedback and requests |
| Technology Manufacturers | Hardware/software supporter  | Accommodate project requirements and support system changes |

### 2.5 Risk Management Plan
The SPMP shall specify:
- Risk management plan for identifying, analyzing and prioritizing project risk factors.
- Procedures for contingency planning and the methods that will be used for tracking certain risk factors, changes in levels of the factors and responses to those changes. The U↑ team will maintain the project’s risk factors and strategies for risk mitigation in a separate document, The U↑ Risk Management Plan.

### 2.6 External Structure
The client for this project is the TA Pengfei who is supposed to be a company wanting to use this product for internal use. All formal communication between the client and team was done through email on an as-needed basis. All team communication was done in person during class meetings or via discord as-needed. 


## 3 MANAGERIAL PROCESS
### 3.1 Management Objectives and Priorities
### 3.2 Assumptions, Dependencies, and Constraints
### 3.3 Risk Management
### 3.4 Monitoring and Controlling Mechanisms
### 3.5 Staffing Plan

## 4 TECHNICAL PROCESS

### 4.1 Methods, Tools, and Techniques

- **Software Development Methodology:** Agile Scrum will be employed, facilitating iterative development and regular reassessment of project priorities.

- **Tools:**

  - **Coding:** Visual Studio Code and IntelliJ IDEA for development.
  - **Version Control:** Git with GitHub for repository management.
  - **Project Management:** JIRA for tracking progress and managing sprints.
  - **Collaboration:** Slack for team communication and Zoom for virtual meetings.

- **Techniques:**

  - **Requirement Gathering:** User story mapping and backlog grooming sessions.
  - **Design:** Use of UML diagrams for system architecture and database design.
  - **Testing:** Test-Driven Development (TDD) approach.
  - **Deployment:** Continuous Integration/Continuous Deployment (CI/CD) pipeline using Jenkins.\

- **Configuration Management Plan:** Utilize Git for version control, with a branching strategy incorporating feature, develop, and master branches.
- **Quality Assurance Plan:** Regular code reviews, adherence to coding standards, and automated testing to ensure quality.

### 4.2 Software Documentation

- **Documentation:** All of the projects documentation will be managed in Confluence, and API documentation will be managed in Swagger.
- **Naming Conventions and Style Guides:** Follow Google's style guides for code documentation. Variables, functions, and classes will use camelCase naming for consistency.
- **Maintenance Plan:** Documentation will be reviewed and updated at the end of each sprint. The responsibility will be assigned on a rotating basis among team members.

### 4.3 Project Support Functions

**Quality Assurance (QA):**

- **Call Quality Testing:** Dedicated QA testing for audio quality and connection stability across different network conditions, ensuring high-quality voice calls.
- **User Interface Testing:** Special focus on testing the user interfaces of the System Console and client apps for usability and responsiveness.
- **Security Testing:** Emphasis on end-to-end encryption testing and user authentication processes, crucial for the privacy and security of calls and user data.

**Secretarial and Administrative Support:**

- **Meeting Coordination:** Regularly scheduled meetings with the client to discuss progress, gather feedback, and refine requirements.
- **Document Management:** Maintaining up-to-date project documentation, including meeting minutes, technical specifications, and revision histories, particularly relevant to the evolving nature of the project requirements.

**Technical Support:**

- **Post-Deployment Support:** Establishing a help-desk system for end-users to address technical issues, usage queries, and troubleshooting post-deployment.
- **Training Material Development:** Creating comprehensive training materials for administrators using the System Console, focusing on system monitoring, user account management, and billing plan adjustments.

**Risk Management:**

- **Network Dependency:** Regular assessment of risks associated with network dependencies, such as server downtimes or bandwidth fluctuations.
- **Software Compatibility Risks:** Evaluating and mitigating risks related to software compatibility across different user devices (laptops, smartphones, desktops).

**Resource Management:**

- **Developer Allocation:** Focused allocation of developers to critical components like server processes, client apps development, and the System Console based on project phase and priorities.
- **Testing Resources:** Allocating sufficient resources for thorough testing phases, including load testing for handling concurrent calls and billing process accuracy.

**Procurement and Contract Management:**

- **Third-party Services:** If any third-party services (like cloud services for hosting the server) are required, managing contracts and ensuring they align with project timelines and quality standards.
- **Software Licensing:** Handling software licensing for any commercial tools or platforms used in the development and deployment of the virtual phone system.

## 5 WORK PACKAGES, SCHEDULE, AND BUDGET
### 5.1 Work Packages
### 5.2 Dependencies
### 5.3 Resource Requirements
### 5.4 Budget, Resource Allocation and Schedule
