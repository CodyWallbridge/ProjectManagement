# U↑ Software Project Management Plan

**Version:** 1.0
**Date:** November 24, 2023
**Team Name:** Shaowei's Angels

## VERSION HISTORY

| Version # | Implemented By | Revision Date | Approved By | Approval Date | Reason |
|-----------|----------------|---------------|-------------|---------------|--------|
| 1.0       | Mia            | 11/13/23      | Mia         | 11/13/23      | Added Template. |
| 1.1       | Cody           | 11/14/23      | Everyone    | 11/14/23      | Added introduction and project organization. |
| 1.2       | Barbara        | 11/16/23      | Mia         | 11/19/23      | Added Managerial Process.                    |
| 1.3       | Mia            | 11/19/23      |             |               | Edited some wording and formatting. |
| 1.4       | Mia            | 11/20/23      |             |               | Added Work Packages, Schedule and Budget. Moved items from Managerial Process appropriately. |

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
- Procedures for contingency planning and the methods that will be used for tracking certain risk factors, changes in levels of the factors and responses to those changes. The U↑ team will maintain the project’s risk factors and strategies for risk mitigation in [Section 3.4 Risk Management Plan]().

### 2.6 External Structure
The client for this project is the TA, Pengfei, who is acting as a company interested in this product for internal use. All formal communication between the client and team was done through email on an as-needed basis. All team communication was done in person during class meetings or via Discord as needed.


## 3 MANAGERIAL PROCESS PLAN

To achieve success, the team needs to provide a software product that aligns with the client's requirements as specified in the "U↑" SRS. Throughout the project, the team strives to consider and attain the stated goals whenever feasible.

To achieve its objectives the "U↑" team has the following goals and priorities:

- Deliver a quality cloud-based telephony system that meets the client expectations by (the end of the timeline).
  - The whole team will accomplish this by sticking to the plan and delivering a finished product on time.
  - Accomplishing this will ensure the clients are happy and we successfully finished the project

- Reduce downtime in the project after the system has been up and running for a month.
  - The Administrators will accomplish this goal by offering training sessions.
  - Accomplishing this will reduce the time when people are waiting for a response.

- Cut down onboarding time by 10% by the end of December 2024.
  - The Administrators will accomplish this goal by asking for feedback after onboarding new customers on how to make onboarding faster for them.
  - Accomplishing this will make communications more efficient and lead to happier customers.

- When making a call it should be rerouted within 5 seconds by the end of December 2024.
  - The developer will accomplish this goal by having a clean structure and implementing clean code.
  - Accomplishing this goal will make the users have a smooth experience with the phone.

### 3.1 Start-up plan

#### 3.1.1 Estimates

The total project cost is estimated to be 500,000 with a 20,000 emergency fund. Our team has with high confidence levels.

Table of the estimated cost allocated for the yearly cost

| Category              | Estimated Cost ($) | Notes                                            | Basis of Estimation                                                                                                                         |
| --------------------- | ------------------ | ------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------- |
| Development           | 200,000            | Software design, coding, and feature development | Based on a combination of factors, including the complexity of software design and coding, anticipated features, and development time       |
| Testing               | 50,000             | Quality assurance and testing activities         | The testing estimate is based on the anticipated testing activities, quality assurance efforts, and the size and complexity of the software |
| Infrastructure        | 80,000             | Servers, hosting, and network infrastructure     | Expected costs of servers, hosting services, and network infrastructure                                                                     |
| Equipment             | 50,000             | Laptop, screens, mouses, etc for development     | Based on a cost models factors related to the hardware and devices required for the project                                                 |
| User Interface/Design | 35,000             | UI/UX design and user interface development      | Complexity of the user interface (UI) and user experience (UX) design, as well as the anticipated design work required                      |
| Documentation         | 15,000             | Technical documentation, training sessions       | expected effort for creating technical documentation and conducting training sessions                                                       |
| Project Management    | 40,000             | Project planning, coordination, and management   | Based on the expected time and effort required for project planning, coordination, and management activities and cost models                |
| Legal and Compliance  | 10,000             | Licensing, legal consultations, compliance       | Based on cost models anticipated costs for licensing, legal consultations, and ensuring regulatory compliance                               |
| Emergency fund        | 20,000             | Unforeseen expenses and changes in requirements  | This is a rule of thumb to account for unexpected challenges                                                                                |
| Total Budget          | 500,000            | Total Estimation                                 |  |         

##### 3.1.1.1 Monthly Breakdown



Using this budget, the positions we can hire for the full year are:

- 4 Full Stack developers (Development Budget)
- 1 Project Manager (Project Management Budget)
- 1 IT Person (Infrastructure Budget)
- 1 Technical Writer (Documentation Budget)

The positions we can hire for the last 6 months are:

- 1 Quality Assurance developer (Testing Budget)

While maintaining:

- Stable infrastructure
- Documentation and quality training sessions
- A legal team supporting the project and development company

##### 3.1.1.2 Estimation of Work

The developers and Project Manager will use Agile methodology to estimate work.

##### 3.1.1.3 Re-estimation of Work

We will re-estimate work on every project milestone and upon any changes in the budget. The re-estimation will use the Work Breakdown Structure, and will be done given how much work was done on the previous milestone we can adjust to it.

#### 3.1.2 Staffing Plan

The staffing plan introduced in 3.1.1.1 Monthly Breakdown is broken down in further detail below:

| Skill Level         | Full Stack Developers | QA Developer | Project Manager    | IT Person      | Technical Writer |
| - | - | - | - | - | - |
| Entry-Level         | 1                     | 0            | 0                  | 1              | 1 |
| Mid-Level           | 2                     | 1            | 1                  | 0              | 0 |
| Senior-Level        | 1                     | 0            | 0                  | 0              | 0 |
|  |  |  |  |  | |
| Total Personnel     | 4                     | 1            | 1                  | 1              | 1 |
|  |  |  |  |  |
| Project Phase       | Development           | Testing      | Project Management | Infrastructure | Documentation |
|  |  |  |  |  | |
| Planning            | 1 Mid-Level           | 0            | 1 Mid-Level        | 0              | 0 |
| Development         | 2 Mid-Level, 1 Senior | 0            | 0                  | 0              | 1 Entry-level |
| Testing             | 1 Mid-Level           | 1            | 0                  | 0              | 0 |
| Deployment          | 1 Entry-Level         | 0            | 0                  | 1 Entry-Level  | 0 |
|  |  |  |  |  | |
| Duration            | 12 months             | 6 months     | 12 months          | 12 months      | 12 months |
|  |  |  |  |  | |
| Source of Personnel | New Hires             | New Hire     | Internal Transfer  | Contracted     | New Hire |

## 3.2 Project Tracking Plan

### 3.2.1 Process for Measuring

We will measure success in how many user stories where completed in a 2-week sprint, comparing it to the deadlines in our project schedule and the high-level project milestones.

### 3.2.2 Changes Request

Since we are using Agile, changes will be more usual. Developers can implement changes at their own discretion, but are expected to bring it up to the Project Manager and the other developers in case stakeholders need to be consulted. For large-scale changes, we will ensure a meeting with all the stakeholders. At this meeting, the stakeholders will evaluate whether the change follows the vision for the project, and approve or deny it accordingly.

### 3.2.3 Schedule Control

Since we are using Agile, the schedule will be reassessed every 2 weeks in Retrospective and Sprint Planning meetings. We will measure how much work has been done in the milestone, compare it to the expected deadlines in the project schedule, and determine which actions we need to take to meet the task deadlines of the next sprint in time.

### 3.2.4 Communication Plan

As we are going to use Agile, we will have:
- 2 week sprints, starting on Mondays, with a 1 hour Sprint Planning meeting
- Daily 15 minute standup with the developers to review their day-to-day tasks, share their progress, and ask for help
- 1 hour Retrospective meetings at the end of each sprint cycle, i.e., every 2 weeks

The developers and the Project Manager are required to attend these meetings. Once Quality Assurance begins, the QA Developer will join them.

IT will request equipment from the Project Manager as needed. They will meet with the Project Manager at least twice a week to review their hardware or software requirements.

### 3.3 Risk Management Plan

### 3.3.1 Main Risks

1. **Unforeseen Call Scenarios** - They cause system glitches, such as calls to busy lines or invalid numbers.

2. **Data Breach or Unauthorized Access** - especially for the System Console and User Accounts.

3. **Billing Discrepancies** - leading to potential customer grievances.

4. **System Overload** - especially if the number of calls nears the set limit, affecting call quality.

### 3.3.2 Response Plan

| Risk                                   | Response Strategy | Mitigation                                                                                                  |
| -------------------------------------- | ----------------- | ----------------------------------------------------------------------------------------------------------- |
| **Unforeseen Call Scenarios**          | Avoidance         | Integrate advanced call routing algorithms and fallback mechanisms.                                         |
| **Data Breach or Unauthorized Access** | Avoidance         | Employ stringent security measures, including multi-factor authentication and end-to-end encryption.        |
| **Billing Discrepancies**              | Avoidance         | Implement robust billing verification mechanisms and provide users with a transparent breakdown of charges. |
| **System Overload**                    | Avoidance         | Design an alert system for administrators and consider elastic scalability solutions.                       |

#### 3.4 Project Closeout

To ensure that we can close out the project, we will conduct the following:

- Final Code Review: Conduct a thorough review of the final codebase to ensure it meets quality standards and follows coding conventions.
- Testing and Quality Assurance: Perform final testing to verify the software's functionality and address any remaining bugs or issues.
- Documentation Completion: Ensure all project documentation, and training was done successfully
- Meet Milestone: Make sure that the project has met its objectives from milestones set by the stakeholders.
- Archive Project Materials: Archive all project-related materials, including code repositories, documents, and any other relevant data for future reference.
- Final Retrospective: Hold a team retrospective session to discuss the project's successes, challenges, and lessons learned.
- Equipment and Resource Return: Arrange for the return of any borrowed or leased equipment and release resources allocated for the project.
- Post-Implementation Support Plan: Establish a plan for post-implementation support, including maintenance and addressing any post-launch issues.
- Legal and Contractual Closure: Ensure all legal and contractual obligations are fulfilled, and contracts are officially closed.
- Celebrate Project Completion: Celebrate the successful completion of the project with the team, acknowledging their hard work and dedication.

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
  - **Deployment:** Continuous Integration/Continuous Deployment (CI/CD) pipeline using Jenkins.

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

The work packages are organized in a WBS diagram. As the project will use Agile methodology, one unit of work is a "story point," an abstract measure of work that can be completed in a 2-week sprint. After the first 2 sprints, the team will re-evaluate the WBS based on how many story points they were able to accomplish in each prior sprint.

![WBS diagram](/WBS%20Tasks.png)

### 5.2 Dependencies

The dependencies of each task in the WBS are illustrated in a PERT chart. This diagram also shows the critical path, which is the chain of dependent tasks estimated to take the longest to accomplish.

![PERT diagram](/pert-diagram.png)

As work is re-estimated throughout project execution, the PERT chart and critical path will be updated accordingly.

### 5.3 Resource Requirements

The project will require hardware resources, software 

#### 5.3.1 Hardware Resources

Each team member will work from home. To ensure consistent hardware specifications, each team member will be given a 14-inch MacBook Pro with:
- 11-core CPU14-core GPU
- 18GB Unified Memory
- 512GB SSD Storage

As working from home is the expectation, if employers need dongles, mice, or extra screens, they will request it to the IT Person.

#### 5.3.2 Infrastructure Resources

In addition to the infrastructure tools listed in [4.1 Methods, Tools, and Techniques](#4-1-methods-tools-and-techniques), we will use Amazon EC2 for:
- Server hosting and management
- Testing work activities on machines with different operating systems and hardware capabilities

#### 5.3.3 Staffing Resources

As outlined in [3.1.2 Staffing Plan](#3-1-2-staffing-plan), the necessary personnel for this project include:
- 4 Full Stack developers
- 1 Project Manager
- 1 IT Person
- 1 Quality Assurance developer
- 1 Technical Writer

### 5.4 Budget, Resource Allocation and Schedule

The following 3 subsections provide a detailed breakdown of the budget per month, resource allocation per work activity, and individual tasks within the development phase.

#### 5.4.1 Budget Allocation per Month
Below is the breakdown of the project budget by month. The budget is designed to leave us with $40,000 in monthly expenses.

| Month | Development ($) | Testing ($) | Infrastructure ($) | UI/Design ($) | Documentation ($) | Project Management ($) | Legal/Compliance ($) | Total Expenses ($) | Confidence Level |
| - | - | - | - | - | - | - | - | - | - |
| 1     | 20,833          | 0           | 6,667              | 2,917         | 1,250             | 3,333                  | 833                  | 35,833             | High             |
| 2     | 20,833          | 0           | 6,667              | 2,917         | 1,250             | 3,333                  | 833                  | 35,833             | High             |
| 3     | 20,833          | 0           | 6,667              | 2,917         | 1,250             | 3,333                  | 833                  | 35,833             | High             |
| 4     | 20,833          | 0           | 6,667              | 2,917         | 1,250             | 3,333                  | 833                  | 35,833             | Medium           |
| 5     | 20,833          | 0           | 6,667              | 2,917         | 1,250             | 3,333                  | 833                  | 35,833             | Medium           |
| 6     | 20,833          | 0           | 6,667              | 2,917         | 1,250             | 3,333                  | 833                  | 35,833             | Medium           |
| 7     | 20,833          | 8,333       | 6,667              | 2,917         | 1,250             | 3,333                  | 833                  | 44,166             | Medium           |
| 8     | 20,833          | 8,333       | 6,667              | 2,917         | 1,250             | 3,333                  | 833                  | 44,166             | Medium           |
| 9     | 20,833          | 8,333       | 6,667              | 2,917         | 1,250             | 3,333                  | 833                  | 44,166             | Medium           |
| 10    | 20,833          | 8,333       | 6,667              | 2,917         | 1,250             | 3,333                  | 833                  | 44,166             | Medium           |
| 11    | 20,833          | 8,333       | 6,667              | 2,917         | 1,250             | 3,333                  | 833                  | 44,166             | Medium           |
| 12    | 20,833          | 8,333       | 6,667              | 2,917         | 1,250             | 3,333                  | 833                  | 44,166             | Medium           |
| Total | 250,000         | 50,000      | 80,000             | 35,000        | 15,000            | 40,000                 | 10,000               | 480,000            | Medium           |

#### 5.4.2 Resource Allocation per Work Activities
Below illustrates the required resources for each work activity in the project.

Note that some resources, such as the machines or software used for development, will be used throughout the project and therefore allocated to multiple work activities. As activities do not necessarily happen concurrently, the same staff personnel may be allocated to two or more activities.

| Activity | Hardware Resources | Software Tools | Infrastructure Tools | Staffing Resources |
| -------- | ------------------ | -------------- | -------------------- | ------------------ |
| Project Management | 14" MacBook Pro (5) | Confluence, JIRA, Slack, Zoom | | Project Manager (1),  Full Stack developer (4) |
| Initial Configuration | 14" MacBook Pro (4) | Visual Studio Code, IntelliJ IDEA, Git, Slack | Jenkins | Full Stack developer (4) |
| Audio Communication | 14" MacBook Pro (2) | Visual Studio Code, IntelliJ IDEA, Git | Jenkins, Amazon EC2 | Full Stack developer (2) |
| Text Communication | 14" MacBook Pro (2) | Visual Studio Code, IntelliJ IDEA, Git | Jenkins, Amazon EC2 | Full Stack developer (2) |
| Manage User Account | 14" MacBook Pro (2) | Visual Studio Code, IntelliJ IDEA, Git | Jenkins | Full Stack developer (2) |
| Search System Records | 14" MacBook Pro (2) | Visual Studio Code, IntelliJ IDEA, Git | Jenkins | Full Stack developer (2) |
| Technical Support | 14" MacBook Pro (2) | Visual Studio Code, IntelliJ IDEA, Git | Jenkins, Amazon EC2 | Full Stack developer (2) |
| Billing | 14" MacBook Pro (2) | Visual Studio Code, IntelliJ IDEA, Git | Jenkins | Full Stack developer (2) |
| System Console | 14" MacBook Pro (2) | Visual Studio Code, IntelliJ IDEA, Git | Jenkins | Full Stack developer (2) |
| Acceptance | 14" MacBook Pro (5) | Visual Studio Code, Confluence, IntelliJ IDEA, Git, Slack | Jenkins, Amazon EC2 | Project Manager (1), Full Stack developer (2), Quality Assurance developer (1), Technical Writer (1) |

#### 5.4.3 Schedule of Project Activities

Each task in the WBS is assigned and scheduled using a Gantt Chart. The Gantt chart may be updated by individual developers throughout the sprint cycle as they make progress on their tasks, but will be formally reviewed and updated by the developer team and Project Manager during each sprint's Retrospective meeting.

As the occupants of each position are not yet known, they are labelled in the Gantt chart with their position and an identifying letter (e.g., "Project Manager A," "Full Stack developer B," etc.). The assignees may also be updated upon staffing changes or reassessment of workload as the project progresses.

![Gantt Chart](/4050Gantt_Light.png)
