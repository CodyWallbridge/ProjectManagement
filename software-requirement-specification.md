# U↑ (U Up)

**Software Requirements Specification**:

**Version:** 1.2

**Date:** 10/10/23

**Your Team Name:** Shaowei's Angels

---

## Revision History

| Date       | Description                         | Author        | Comments             |
|------------|-------------------------------------|---------------|----------------------|
| 10/02/23   | Making the word file into a .md     | Barbara       |                      |
| 10/03/23   | Entered functional requirements     | Mia           |                      |
| 10/03/23   | Entering sections 3.3-4             | Cody          |                      |
| 10/03/23   | Entered non-functional requirements | Daniel        |                      |
| 10/04/23   | Entering sections 1 and 2           | Barbara       |                      |
| 10/06/23   | Edits after meeting with the TA     | Barbara       |                      |
| 10/10/23   | Final read-through and edits        | Group         |                      |
---

## Table of Contents

- [U↑ (U Up)](#u-u-up)
  - [Revision History](#revision-history)
  - [Table of Contents](#table-of-contents)
  - [1. Introduction](#1-introduction)
    - [1.1 Purpose](#11-purpose)
    - [1.2 Definitions, Acronyms, and Abbreviations](#12-definitions-acronyms-and-abbreviations)
    - [1.3 References](#13-references)
  - [2. General Description](#2-general-description)
    - [2.1 User Characteristics](#21-user-characteristics)
          - [2.1.1 Phase 1](#211-phase-1)
          - [2.1.2 Phase 2](#212-phase-2)
    - [2.2 Assumptions](#22-assumptions)
    - [2.3Dependencies](#23-dependencies)
  - [3. Specific Requirements](#3-specific-requirements)
    - [3.1 Functional Requirements](#31-functional-requirements)
      - [3.1.1 Allow audio communication between users](#311-allow-audio-communication-between-users)
      - [3.1.2 Allow text-based communication between users](#312-allow-text-based-communication-between-users)
      - [3.1.3 Manage user accounts](#313-manage-user-accounts)
      - [3.1.4 Allow users to search system records](#314-allow-users-to-search-system-records)
      - [3.1.5 Provide technical support to users](#315-provide-technical-support-to-users)
    - [3.2 Non-Functional Requirements](#32-non-functional-requirements)
      - [3.2.1 Performance](#321-performance)
      - [3.2.2 Reliability](#322-reliability)
      - [3.2.3 Availability](#323-availability)
      - [3.2.4 Security](#324-security)
      - [3.2.5 Interfaces](#325-interfaces)
    - [3.3 Design Constraints](#33-design-constraints)
      - [3.3.1 Standard Development Tools](#331-standard-development-tools)
      - [3.3.2 Web Based Product](#332-web-based-product)
    - [3.4 Legal, Copyright, and Other Notices](#34-legal-copyright-and-other-notices)
    - [3.5 Other Requirements](#35-other-requirements)
      - [3.5.1 Configuration Management Tool](#351-configuration-management-tool)
      - [3.5.2 Licensing Requirements](#352-licensing-requirements)
      - [3.5.3 Applicable Standards](#353-applicable-standards)
      - [3.5.4 Purchased Components](#354-purchased-components)
  - [4 Other Supporting Documents](#4-other-supporting-documents)
    - [A. Appendices](#a-appendices)
      - [A.1 Meeting Minutes with Shayan](#a1-meeting-minutes-with-shayan)

---

## 1. Introduction

The Software Requirements Specification (SRS) begins by offering a comprehensive overview of the entire document, encompassing its purpose, scope, definitions, acronyms, abbreviations, references, and an outline of its content. This document serves the purpose of extensively examining and providing a deep understanding of the U↑ (U Up) software system, primarily by elaborating on the problem statement. Furthermore, it places emphasis on identifying the capabilities required by stakeholders and addressing their needs while defining high-level product features. The document proceeds to outline the intricate requirements of the U↑ software system.

### 1.1 Purpose

The primary purpose of this Software Requirements Specification (SRS) is to establish a comprehensive and detailed set of specifications for the development of U↑, an internet-based phone system for a company's employees. This document aims to define the functional and non-functional requirements of the software, outline its intended features and capabilities, and provide a clear roadmap for its development.

By creating this SRS, we aim to ensure a thorough understanding of the project's scope, objectives, and technical specifications among all stakeholders, including developers, designers, and clients. It will serve as a vital reference guide throughout the development process, helping to maintain consistency, meet user expectations, and ultimately deliver a high-quality, reliable, and efficient internet-based phone call software solution.

### 1.2 Definitions, Acronyms, and Abbreviations

| Acronym / Abbreviation  | Definition                            |
|-------------------------|---------------------------------------|
|  Kbps                   |  Kilobytes per seconds                |
|  SRS                    |  Software Requirements Specification  |
|  CUA                    |  Common User Access                   |
|  GUI                    |  Graphical User Interface             |
|  OS                     |  Operating System                     |
|  API                    |  Application Programming Interface    |
|  TCP                    |  Transmission Control Protocol        |
|  IP                     |  Internet Protocol                    |

### 1.3 References

Used the template and referenced the example SRS given.

## 2. General Description

### 2.1 User Characteristics

#### 2.1.1 Phase 1

The initial release of this project will be for companies and their employees are going to be the main users:

- Company Employees: The main users of U↑, we can assume they know how to use the internet. The developers will make the UI easy to use but after a couple uses they should know how to intuitively use U↑.
- Administrators: They will manage the maximum number of callers allowed in the system. They will be very knowledgeable of the system.

#### 2.1.2 Phase 2

After U↑ is successfully launched the project could be released to the public and anyone can use our system. The details regarding the necessary user profiles will be determined in a future version so as to minimize scope creep.

### 2.2 Assumptions

- There is going to be some training and resources will be given to the company.
- A member of the development team will provide support to the client company for the first month after release.
- An administrator could be a member of our company, the client company or a third-party company.

### 2.3 Dependencies

- The OS of the system that the user is going to use to make the calls.
- The client having access to a network infrastructure.
- The client having 300 Kbps of bandwidth.
- The client having a microphone.

## 3. Specific Requirements

This will be the largest and most important section of the SRS. The customer requirements will be embodied within Section 2, but this section will give the D-requirements that are used to guide the project’s software design, implementation, and testing.

### 3.1 Functional Requirements

#### 3.1.1 Allow Audio Communication Between Users

- A user shall be able to dial other users' contact numbers.
- The system shall inform the user if the number they have dialed is not associated with a user.
- The system shall inform the user if the user whose number they have dialed is unavailable.
- A user shall be able to make an outgoing call to an individual user at a time.
- A user shall be able to end an ongoing call.
- The system shall inform users of incoming calls.
- The system shall display information about the caller when a call is incoming.
- The system shall indicate to a user when they are part of an ongoing call.
- A user shall be able to view the users participating in a call they are a part of.
- The system shall list the users a user has most recently called with.

#### 3.1.2 Allow Text-Based Communication Between Users

- A user shall be able to send text messages to an individual user at a time.
- The system shall notify users of incoming text messages.
- The system shall store a user's text conversation history with other users.
- A user shall be able to delete their text conversation history with other users.
- The system shall list the users a user has most recently contacted via text.

#### 3.1.3 Manage User Accounts

- A user shall be able to register an account in the system.
- A user shall be able to remove their account from the system.
- The system shall authenticate user credentials to access that user's account.
- Each user account shall have a unique contact number.
- The system shall have a directory of all users' profiles.
- A user shall be able to choose personal information to display in their profile.
- A user shall be able to prevent certain user accounts from contacting them.

#### 3.1.4 Allow Users to Search System Records

- A user shall be able to search for other users within the system.
- A user shall be able to search for keywords within their text conversation history.
- The system shall paginate all search results.

#### 3.1.5 Provide Technical Support to Users

- The system shall provide instructions on its common uses.
- The system shall display a list of frequently asked questions.
- The system shall display troubleshooting advice.
- A user shall be able to send text-based help requests to customer support.
- A user shall be able to supply customer and product information in a help request.
- A user shall be able to contact customer support personnel internally through the system.
- The system shall display instructions to contact customer support externally to the system in the case of errors or outages.

### 3.2 Non-Functional Requirements

This section outlines the non-functional requirements crucial for the U↑ internet-based phone system, focusing on performance, reliability, availability, security, and interfaces.

#### 3.2.1 Performance

- **System Latency:** Call rerouting should happen within a 5-second window.
- **Concurrency:** The system must support at least 500 concurrent calls without degradation in performance.
- **Scalability:** The system should accommodate a 20% increase in user devices annually without requiring a system overhaul.

#### 3.2.2 Reliability

- **Data Integrity:** The system must achieve a data accuracy rate of 99.999%.
- **Backup:** Weekly automated backups are mandatory, with a successful restore rate of at least 99%.

#### 3.2.3 Availability

- **Uptime:** The system should guarantee 99.9% uptime, aside from planned maintenance.
- **Failover Capabilities:** Advanced call routing algorithms and fallback mechanisms must be in place to manage unforeseen call scenarios.
- **Maintenance Window:** Planned maintenance must be confined to off-peak hours, occurring no more than once a month.

#### 3.2.4 Security

- **Data Encryption:** All calls must be end-to-end encrypted.
- **Authentication:** Multi-factor authentication must be implemented for both Administrators and regular users.
- **Session Timeout:** Administrator sessions in the User Interface should automatically timeout after 30 minutes of inactivity.

#### 3.2.5 Interfaces

- **User Interface:** The UI must be intuitive and require no more than one hour of training for efficient utilization.
- **Onboarding Time:** New users should be able to complete the onboarding process within 20 minutes, on average.
- **Hardware Compatibility:** The system should be usable across desktop computers, smartphones, tablets, and other devices.
- **Network Protocol:** Communication between devices and the central server should be standardized over TCP/IP using secure sockets, ensuring a packet drop rate of less than 0.1%.
- **API Integration:** The system should have an API with a response time of no more than 2 seconds for integration with other internal systems or third-party services.

### 3.3 Design Constraints

#### 3.3.1 Standard Development Tools

- The system shall be built using a standard web page development tool that conforms to either IBM’s CUA standards or Microsoft’s GUI standards.

#### 3.3.2 Web Based Product

- There are no memory requirements
- The product must be stored in such a way that allows the client easy access to it.
- Response time for loading the product should take no longer than five minutes.
- A general knowledge of basic computer skills is required to use the product.

### 3.4 Legal, Copyright, and Other Notices

- Call app should display the disclaimers, copyright, word mark, trademark and product warranties of Shaowei's Angels.

### 3.5 Other Requirements

#### 3.5.1 Configuration Management Tool

- The source code developed for this system shall be maintained in configuration management tool.

#### 3.5.2 Licensing Requirements

- Not Applicable.

#### 3.5.3 Applicable Standards

- It shall be as per the industry standard.

### 3.5.4 Purchased Components

- Not Applicable.

## 4 Other Supporting Documents

### A. Appendices

#### A.1 Meeting Minutes with Shayan

Barbara had a 10 minutes meeting with Shayan and asked the following questions.

- How specific does the software need to be?
Not much since the Product Managers don't usually know about the libraries.

- Do we need to be specific with the references?
Not much, there needs to be something there but don't use Harvard or any formal referencing.

- Do we need to include group calling?
I think it would be easy to implement since you have one person call planned but its up to you, since you didn't specify on the first document, is your decision.

- Who are the intended users?
For the first phase it would be the client company but eventually it will be open for the world to use.
