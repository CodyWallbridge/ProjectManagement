# U↑ (U Up)

**Project Charter**:

**Version**: 1.1

**Date**: September 26, 2023

**Team Name**: Shaowei's Angels

## VERSION HISTORY

Provide information on how the development and distribution of the Project Charter up to the final point of approval was controlled and tracked. Use the table below to provide the version number, the author implementing the version, the date of the version, the name of the person approving the version, the date that particular version was approved, and a brief description of the reason for creating the revised version.

| Version # | Implemented By | Revision Date | Approved By | Approval Date | Reason |
|-----------|----------------|---------------|-------------|---------------|--------|
| 1.0       | Mia  | 09/24/23    | Cody      | 09/25/23    | Added product overview and project deliverables. |
| 1.1       | Barbara  | 09/26/23    | Mia      | 09/26/23    | Added project objectives and requirements. |

| Name | Email | Period of being project manager |
| ---- | ----- | ------------------------------- |
| Mia Battad | battadm@myumanitoba.ca | September 22, 2023 - September 29, 2023 |

## 1 INTRODUCTION

### 1.1 Purpose of Project Charter

The U↑ project charter documents and tracks the necessary information required by decision maker(s) to approve the project for funding. The project charter should include the needs, scope, justification, and resource commitment as well as the project’s sponsor(s) decision to proceed or not to proceed with the project. It is created during the Initiating Phase of the project.

The intended audience of the U↑ project charter is the project sponsor and senior leadership.

## 2 PROJECT AND PRODUCT OVERVIEW

U↑ is an internet-based phone system for company employees. Employees can make and receive calls over the internet using their desktop computers, smartphones, tablets, or other devices connected to the U↑ system. Each device connected to U↑ will be associated with the same business phone number for incoming and outgoing calls. Any connected device can make or receive calls using U↑ whenever and wherever necessary.

The project will take place over an estimated [], with an estimated budget of [].

## 3 JUSTIFICATION

### 3.1 Objectives

The objectives of U↑ are as follows:

1. Develop the system structure of U↑ the by the end of the first sprint. The developers will accomplish this goal by:
    - Researching the issue of communication over sockets between the server and clients.
    - Developing a document where it outlines how the system is going to work, what technologies are going to be used and explaining the choices that they made.
Accomplishing this goal will ensure we have a good foundation when implementing the structure.

2. Implement the system structure of U↑ the by the end of the first quarter. The developers will accomplish this goal by:
    - Making user stories and breaking them down into tasks.
    - Having daily meetings to check up on the work people is doing.
Accomplishing this goal will ensure we have a strong foundation when implementing future features.

3. Basic Call processing by the end of the first quarter. The developers will accomplish this goal by:
    - Making user stories and breaking them down into tasks.
    - Having daily meetings to check up on the work people is doing.
Accomplishing this goal will ensure that our clients can successfully call whoever they need to reach.

4. Dialing Plan Processing by the end of the  second quarter. The developers will accomplish this goal by:
    - Making user stories and breaking them down into tasks.
    - Having daily meetings to check up on the work people is doing.
Accomplishing this goal will ensure that our clients don't have to worry about reaching the right person when dialing someone.

5. System Console by the end of the second quarter. The developers will accomplish this goal by:
    - Making user stories and breaking them down into tasks.
    - Having daily meetings to check up on the work people is doing.
Accomplishing this goal will ensure that our clients have unique accounts.

6. Users can create accounts by the end of the third quarter. The developers will accomplish this goal by:
    - Making user stories and breaking them down into tasks.
    - Having daily meetings to check up on the work people is doing.
Accomplishing this goal will ensure that our clients have personal accounts and can make and receive calls.

7. Load balancing calls by the end of the third quarter. The developers will accomplish this goal by:
    - Making user stories and breaking them down into tasks.
    - Having daily meetings to check up on the work people is doing.
Accomplishing this goal will ensure that our servers wont be overloaded by the users.

8. Billing user calls by the end of the third quarter. The developers will accomplish this goal by:
    - Making user stories and breaking them down into tasks.
    - Having daily meetings to check up on the work people is doing.
Accomplishing this goal will ensure that our company gets paid so that we can keep developing this project.

### 3.2 High-Level Requirements

| Req. # | Requirement Description |
| ------ | ----------------------- |
| 1 | There is a document describing the architecture of the system and explaining it|
| 2 | There is a structure following the architecture of the first requirement, and producing more documentation if they decide to change it |
| 3 | Users can send and receive calls using sockets |
| 4 | Users calls are mapped from (IP address, port) |
| 5 | There is an User Interface where the administrators can log in and use to control a network of phones |
| 6 | Regular users can create ana account and originate or receive calls, they can also block other users or have privileges |
| 7 | The Administrators can change the maximum number of callas allowed in the system  |
| 9 | We successfully charge the users for making a call, taking into account, the regular fee, how many times they call, and discount rates for the periods |

### 3.3 Major Deliverables

| Major Deliverable | Deliverable Description |
| ----------------- | ----------------------- |
| Architecture design document | A high-level document describing the functional requirements and system architecture for the U↑ system. |
| Client app UI mock-ups | Interactive user interface mock-ups representing how the U↑ mobile and desktop apps will look and respond to user interaction. |
| System back-end and console | The server software and database for the U↑ system that can be interacted with and tested through an administrator console. |
| Client app integration | Functional client applications that connect to the U↑ back-end and database to make and receive calls. |
| System metrics & performance report | A report detailing the measured increases in efficiency, customer satisfaction, and system availability after implementing U↑ within the company. |

### 3.4 Scope

> [Describe the inclusive and exclusive boundaries of the project. Specifically address items that are out of scope.]

#### Project objective

At U↑ we want to develop the most seamless interaction for users when utilizing the virtual phone.

#### Inclusive Boundaries

Im not sure what he means by this, its no where in the notes imma ask today :)

#### Exclusive Boundaries

#### Out of Scope

- We are not automating load balancing.
- We are not integrating with other calling software.

## 4 DURATION

### 4.1 Timeline

> [An example of a high-level timeline is provided below.]

### 4.2 Executive Milestones

The table below lists the high-level Executive Milestones of the project and their estimated completion timeframe.

| Executive Milestones | Estimated Completion Timeframe |

## 5 ASSUMPTIONS, CONSTRAINTS AND RISKS

### 5.1 Assumptions

1. **Client-Server Communication**: Given the client-server model, it's assumed that the system's architecture will support seamless interaction between multiple clients and the central server via sockets.
2. **Database Integrity**: It's presumed that the database, potentially supporting the system, will maintain a consistent state even with concurrent access from call processing and administration.
3. **Billing Accuracy**: With varying rates based on dialed number, call duration, and timing, we assume the system can calculate bills with high precision to avoid discrepancies.
4. **Client Adaptability**: Given that clients can be desktop apps, mobile apps, etc., it's assumed that all versions will provide a uniform user experience.
5. **Singular Administrator Access**: Only one Administrator accesses the System Console at a time.

### 5.2 Constraints

1. **4-Digit Dialing**: With a 4-digit dialing plan, the system has an inherent limitation on the number of unique extensions.
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

### 6.1 Stakeholders (Internal and External)

### 6.2 Roles and Responsibilities

This section describes the key roles supporting the project.

| Name & Organization | Project Role | Project Responsibilities |
| ------------------- | ------------ | ------------------------ |
| Developers               | Project Team Member  | Engage in day-to-day activities and contribute to project |
| Team Lead                | Project Team Member  | Ensure team stays on track, work breakdowns, work assignment and provide updates to Project Manager |
| Project Manager          | Project Team Member  | Ensure Team Lead is familiar with requirements and provide updates to Director/CEO |
| Director/CEO             | Project Sponsor      | Ensure Project Manager is up to date on requirements and update Investors if needed |
| Investors                | Secondary Stakeholder| Financial support |
| Client Company           | Customer             | Provide feedback and requests |
| General Public           | Future Customer      | Future feedback and requests |
| Future External Companies| Future Customer      | Future feedback and requests |
| Technology Manufacturers | Hardware/software supporter | Follow requirements and support changes|

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
