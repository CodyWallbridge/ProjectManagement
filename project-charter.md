# U↑ (U Up)

**Project Charter**:

**Version**: 1.6

**Date**: September 26, 2023

**Team Name**: Shaowei's Angels

## VERSION HISTORY

Provide information on how the development and distribution of the Project Charter up to the final point of approval was controlled and tracked. Use the table below to provide the version number, the author implementing the version, the date of the version, the name of the person approving the version, the date that particular version was approved, and a brief description of the reason for creating the revised version.

| Version # | Implemented By | Revision Date | Approved By | Approval Date | Reason |
|-----------|----------------|---------------|-------------|---------------|--------|
| 1.0       | Mia            | 09/24/23      | Cody        | 09/25/23      | Added product overview and project deliverables. |
| 1.1       | Dan            | 09/25/23      | Cody        | 09/25/23      | Added project assumptions, constraints, and risks. |
| 1.2       | Barbara        | 09/26/23      | Mia         | 09/26/23      | Added project objectives and requirements. |
| 1.3       | Cody           | 09/26/23      | Mia         | 09/26/23      | Added descriptions of roles & responsibility. |
| 1.4       | Mia            | 09/26/23      | Mia         | 09/26/23      | Added timeline and executive milestones. |
| 1.5       | Group          | 09/26/23      | Group       | 09/26/23      | Final Review. |
| 1.6       | Dan            | 09/27/23      | Barbara     | 09/27/23      | Tweak assumptions and constraints. |

| Name | Email | Period of being project manager |
| ---- | ----- | ------------------------------- |
| Mia Battad | [battadm@myumanitoba.ca](battadm@myumanitoba.ca )| September 22, 2023 - September 29, 2023 |

## 1 INTRODUCTION

### 1.1 Purpose of Project Charter

The U↑ project charter documents and tracks the necessary information required by the decision maker(s) to approve the project for funding. The project charter should include the needs, scope, justification, and resource commitment as well as the project’s sponsor(s) decision to proceed or not to proceed with the project. It is created during the Initiating Phase of the project.

The intended audience of the U↑ project charter is the project sponsor and senior leadership.

## 2 PROJECT AND PRODUCT OVERVIEW

U↑ is an internet-based phone system for company employees. Employees can make and receive calls over the Internet using their desktop computers, smartphones, tablets, or other devices connected to the U↑ system. Each of the user's devices connected to U↑ will be associated with a unique business phone number for incoming and outgoing calls. Any connected device can make or receive calls using U↑ whenever and wherever necessary.

The project will take place over an estimated 12 months, with an estimated budget of $2M.

## 3 JUSTIFICATION

### 3.1 Objectives

The objectives of U↑ are as follows:

- Reduce downtime in the project after the system has been up and running for a month. The Administrators will accomplish this goal by offering training sessions. Accomplishing this will reduce the time when people are waiting for a response.

- Cut down onboarding time by 10% by the end of December 2024. The Administrators will accomplish this goal by asking for feedback after onboarding new customers on how to make onboarding faster for them. Accomplishing this will make communications more efficient and lead to happier customers.

- When making a call it should be rerouted within 5 seconds by the end of December 2024. The developer will accomplish this goal by having a clean structure and implementing clean code. Accomplishing this goal will make the users have a smooth experience with the phone.

### 3.2 High-Level Requirements

| Req. # | Requirement Description |
| ------ | ----------------------- |
| 1 | There is a document describing the system architecture. |
| 2 | There is a structure following the architecture of the first requirement and producing more documentation if they decide to change it. |
| 3 | Users can send and receive calls using sockets. |
| 4 | Users calls are mapped from IP address and port. |
| 5 | There is a User Interface that the Administrators can log in to and use to control a network of phones. |
| 6 | Regular users can create an account that can originate or receive calls, and block other users or have privileges. |
| 7 | The Administrators can change the maximum number of callers allowed in the system.  |
| 9 | We successfully charge the users a price for making a call based on the regular fee, how many times they call, and discount rates for the periods. |

### 3.3 Major Deliverables

| Major Deliverable | Deliverable Description |
| ----------------- | ----------------------- |
| Architecture design document | A high-level document describing the functional requirements and system architecture for the U↑ system. |
| Client app UI mock-ups | Interactive user interface mock-ups representing how the U↑ mobile and desktop apps will look and respond to user interaction. |
| System back-end and console | Server software and database for the U↑ system that can be interacted with and tested through an administrator console. |
| Client app integration | Functional client applications that connect to the U↑ back-end and database to make and receive calls. |
| System metrics & performance report | A report detailing the measured increases in efficiency, customer satisfaction, and system availability after implementing U↑ within the company. |

### 3.4 Scope

#### Inclusive Boundaries

- Support calls inside the client company.
- Support audio and text.
- Support major tech hardware and software.

#### Exclusive Boundaries

- No integration with other calling software.
- No support for calls outside the client company.
- No support for video calls.

## 4 DURATION

### 4.1 Timeline

| Date (MM/YY) |     |
| ------------ | --- |
| 10/23        | Project plan finalized |
| 11/23        | Requirements finalized and approved |
| 04/24        | System prototypes developed |
| 12/24        | System integrated into company |

### 4.2 Executive Milestones

The table below lists the high-level Executive Milestones of the project and their estimated completion time frame.

| Executive Milestones | Estimated Completion Time frame |
| -------------------- | ------------------------------ |
| Project plan created and approved | 2 weeks after Project Charter's initial draft is completed |
| Visual prototypes developed | 8 weeks after requirements are finalized |
| Software version 1 completed | 16 weeks after prototypes are completed |
| Security and load testing of system | 4 weeks after completion of Version 1 |
| Limited integration of system into company | 2 weeks after security and load testing |
| Full system integration into company | 8 weeks after limited system integration |

## 5 ASSUMPTIONS, CONSTRAINTS AND RISKS

### 5.1 Assumptions

1. **Client-Server Communication**: The system architecture will support seamless interaction between multiple clients and the central server via sockets.
2. **Database Integrity**: The database, potentially supporting the system, will maintain a consistent state even with concurrent access from call processing and administration.
3. **Billing Accuracy**: The system can calculate bills with high precision to avoid discrepancies.
4. **Client Adaptability**: All versions will provide a uniform user experience across clients using desktop, mobile, etc...
5. **Singular Administrator Access**: Only one Administrator accesses the System Console at a time.

### 5.2 Constraints

1. **4-Digit Dialing**: The system has an inherent limitation on the number of unique extensions with a 4-digit dialing plan.
2. **Socket-Only Communication**: The mandate that communication should exclusively occur over sockets restricts alternative communication methods.
3. **Load Limits**: The system has an upper threshold for the number of concurrent calls it can handle, determined by the Administrator.

### 5.3 Risks

| Risk | Mitigation |
| --- | --- |
| **Unforeseen Call Scenarios** causing system glitches, such as calls to busy lines or invalid numbers. | Integrate advanced call routing algorithms and fallback mechanisms. |
| **Data Breach or Unauthorized Access** especially for the System Console and User Accounts. | Employ stringent security measures, including multi-factor authentication and end-to-end encryption. |
| **Billing Discrepancies** leading to potential customer grievances. | Implement robust billing verification mechanisms and provide users with a transparent breakdown of charges. |
| **System Overload**, especially if the number of calls nears the set limit, affecting call quality. | Design an alert system for administrators and consider elastic scalability solutions. |

## 6 PROJECT ORGANIZATION

### 6.1 Stakeholders

#### Internal

- Sales Representative
- IT department
- Developers
- Team Lead
- Project Manager
- Director/CEO

#### External

- Investors
- Client Company
- General Public
- Future External Companies
- Technology Manufacturers

### 6.2 Roles and Responsibilities

This section describes the key roles supporting the project.

#### Internal Roles and Responsibilities

| Name & Organization | Project Role | Project Responsibilities |
| ------------------- | ------------ | ------------------------ |
| Sales Representative     | Project Team Member  | Market the product by communicating its purpose and features |
| IT Department            | Project Team Member  | Support the onboarding of customers and requests from the developers |
| Developers               | Project Team Member  | Engage in day-to-day activities, be on call when needed, technical writing, and contribute to project success |
| Team Lead                | Project Team Member  | Monitor team progress, ensure the team stays on track, run work breakdowns, organize work assignments and provide updates to Project Manager |
| Project Manager          | Project Team Member  | Ensure Team Lead is familiar with requirements, provide updates to Director/CEO, break tasks |
| Director/CEO             | Project Sponsor      | Ensure Project Manager is up to date on the requirements and update Investors if needed |

#### External Roles and Responsibilities

| Name & Organization      | Project Role                 | Project Responsibilities |
| Investors                | Secondary Stakeholder        | Provide financial support to the project |
| Client Company           | Customer                     | Provide feedback and requests |
| General Public           | Future Customer              | Offer future feedback and requests |
| Future External Companies| Future Customer              | Offer future feedback and requests |
| Technology Manufacturers | Hardware/software supporter  | Accommodate project requirements and support system changes |

## 7 PROJECT CHARTER APPROVAL

Signature: ________  Date: ________
Print Name: ________
Title: ________
Role: ________

Signature: ________  Date: ________
Print Name: ________
Title: ________
Role: ________

Signature: ________  Date: ________
Print Name: ________
Title: ________
Role: ________

## APPENDIX A: REFERENCES

The following table summarizes the documents referenced in this document.

| Document Name and Version | Description | Location |
| ------------------------- | ----------- | -------- |
