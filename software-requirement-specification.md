# U↑ (U Up)

**Software Requirements Specification**:

**Version:** 0.0

**Date:** 10/02/23

**Your Team Name:** Shaowei's Angels

---

## Revision History

| Date       | Description                      | Author        | Comments             |
|------------|----------------------------------|---------------|----------------------|
| 10/02/23   | Making the word file into a .md  | Barbara       |                      |
| 10/03/23 | Entered non-functional requirements | Daniel | |

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
    - [2.2 Assumptions and Dependencies](#22-assumptions-and-dependencies)
  - [3. Specific Requirements](#3-specific-requirements)
    - [3.1 Functional Requirements](#31-functional-requirements)
      - [3.1.1 Functionality](#311-functionality)
      - [3.1.2 Usability](#312-usability)
      - [3.1.3 Accessibility](#313-accessibility)
    - [3.2 Non-Functional Requirements](#32-non-functional-requirements)
      - [3.2.1 Performance](#321-performance)
      - [3.2.2 Reliability](#322-reliability)
      - [3.2.3 Availability](#323-availability)
      - [3.2.4 Security](#324-security)
      - [3.2.5 Interfaces](#325-interfaces)
    - [3.3 Design Constraints](#33-design-constraints)
    - [3.4 Legal, Copyright, and Other Notices](#34-legal-copyright-and-other-notices)
    - [3.5 Other Requirements](#35-other-requirements)
  - [4 Other Supporting Documents](#4-other-supporting-documents)
    - [A. Appendices](#a-appendices)

---

## 1. Introduction

[You may need to refine your scope/purpose defined in the project charter after eliciting requirements with stakeholders].

The introduction to the Software Requirement Specification (SRS) document should provide an overview of the complete SRS document. While writing this document, please remember that this document should contain all the information needed by a software engineer to adequately design and implement the software product described by the requirements listed in this document. (Note: the following subsection annotations are largely taken from the IEEE Guide to SRS).

### 1.1 Purpose

What is the purpose of this SRS and the (intended) audience for which it is written.

### 1.2 Definitions, Acronyms, and Abbreviations

This subsection should provide the definitions of all terms, acronyms, and abbreviations required to properly interpret the SRS. This information may be provided by reference to one or more appendices in the SRS or by reference to other documents.

### 1.3 References

This subsection should:

1. Provide a complete list of all documents referenced elsewhere in the SRS, or in a separate, specified document.
2. Identify each document by title, report number - if applicable - date, and publishing organization.
3. Specify the sources from which the references can be obtained.
This information may be provided by reference to an appendix or to another document.

## 2. General Description

This section of the SRS should describe the general factors that affect the product and its requirements. It should be made clear that this section does not state specific requirements; it only makes those requirements easier to understand.

### 2.1 User Characteristics

This subsection of the SRS should describe those general characteristics of the eventual users of the product that will affect the specific requirements. (See the IEEE Guide to SRS for more details).

### 2.2 Assumptions and Dependencies

This subsection of the SRS should list each of the factors that affect the requirements stated in the SRS. These factors are not design constraints on the software but are, rather, any changes to them that can affect the requirements in the SRS. For example, an assumption might be that a specific operating system will be available on the hardware designated for the software product. If, in fact, the operating system is not available, the SRS would then have to change accordingly.

## 3. Specific Requirements

This will be the largest and most important section of the SRS. The customer requirements will be embodied within Section 2, but this section will give the D-requirements that are used to guide the project’s software design, implementation, and testing.

### 3.1 Functional Requirements

This section describes specific features of the software project. Specify the requirements as user stories.

- Sell Configured to Ordered Products.
- The system shall display all the products that can be configured.
- The system shall allow the user to select the product to configure.
- The system shall display all the available components of the product to configure.

#### 3.1.1 Functionality

#### 3.1.2 Usability

#### 3.1.3 Accessibility

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

### 3.4 Legal, Copyright, and Other Notices

### 3.5 Other Requirements

Catchall section for any additional requirements.

## 4 Other Supporting Documents

### A. Appendices

Appendices may be used to provide additional (and hopefully helpful) information. If present, the SRS should explicitly state whether the information contained within an appendix is to be considered as a part of the SRS’s overall set of requirements.

Example Appendices could include (initial) conceptual documents for the software project, marketing materials, minutes of meetings with the customer(s), etc.
