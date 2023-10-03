# U↑ (U Up)

**Software Requirements Specification**:

**Version:** 

**Date:** 10/02/23

**Your Team Name:** Shaowei's Angels

---

## Revision History

| Date       | Description                      | Author        | Comments             |
|------------|----------------------------------|---------------|----------------------|
| 10/02/23   | Making the word file into a .md  | Barbara       |                      |
| 10/03/23   | Fill in sections 3.4 through 3.13 | Cody       |                      |


---

## Table of Contents

1. [Introduction](#1-introduction)
   1. [Purpose](#11-purpose)
   2. [Definitions, Acronyms, and Abbreviations](#12-definitions-acronyms-and-abbreviations)
   3. [References](#13-references)
2. [General Description](#2-general-description)
   1. [User Characteristics](#21-user-characteristics)
   2. [Assumptions and Dependencies](#22-assumptions-and-dependencies)
3. [Specific Requirements](#3-specific-requirements)
   1. [Functional Requirements](#31-functional-requirements)
   2. [Non-Functional Requirements](#32-non-functional-requirements)
      1. [Performance](#321-performance)
      2. [Reliability](#322-reliability)
      3. [Availability](#323-availability)
      4. [Security](#324-security)
      5. [Interfaces](#325-interfaces)
   3. [Design Constraints](#33-design-constraints)
   4. [Legal, Copyright, and Other Notices](#34-legal-copyright-and-other-notices)
   5. [Other Requirements](#35-other-requirements)
4. [Other Supporting Documents](#4-other-supporting-documents)
   - [Appendices](#a-appendices)

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


#### 3.1.1 Audio Communications
- The system shall allow the user to make an outgoing call
- The system shall allow the user to make an outgoing call
- The system shall allow the user to end an ongoing call

#### 3.1.2 Text Communications
- The system shall allow users to participate in text conversations with other users
- The system shall allow users to view past conversations with a user

#### 3.1.3 Displaying Details
- The system shall show the calling users info on incoming calls
- The system shall show a directory of all users

#### 3.1.4 Profile Management
- The system shall allow the user to block certain users
- The system shall allow the creation of a new user
- The system shall authenticate user credentials to view the profile.
- The system shall allow user to update the profile information. 

#### 3.1.5 Notifications
- The system shall notify the user of an incoming call
- The system shall notify the user of incoming text messages

#### 3.1.6 Search Functionality
- The system shall allow for searching of users
- The system shall allow for searching within text conversations
- The system shall show all users matching the searched criteria
- The system shall show all messages matching the searched criteria
- The system shall show the 15 most recent messages matching the searched criteria
- The system shall have a "show more" button which loads 15 more messages

#### 3.1.7 Interactivity
- The system shall allow the user to enter numbers
- The system shall inform the user if an inactive number is dialed
- The system shall inform the user if a call is not available at the moment

#### 3.1.8 Display
- The system shall show the user that a call is active
- The system shall show the user who they are in a call with
- The system shall show a list of previous conversations
- The system shall show an "end call" button

#### 3.1.9 Customer Support
- The system shall provide online help, FAQ’s customer support, and sitemap options for customer support.
- The system shall allow user to select the support type he wants.
- The system shall allow user to enter the customer and product information for the support.
- The system shall display the customer support contact numbers on the screen.
- The system shall allow user to enter the contact number for support personnel to call.
- The system shall display the online help upon request.
- The system shall display the FAQ’s upon request

### 3.2 Non-Functional Requirements

#### 3.2.1 Graphical User Interface
- The system shall provide a uniform look and feel between all the web pages.
- The system shall provide a digital image for each product in the product catalog.
- The system shall provide use of icons and toolbars.

#### 3.2.2 Accessibility
- The system shall provide handicap access.
- The system shall provide multi language support.

### 3.3 Reliability & Availability

#### 3.3.1 Back-end Internal Computers
- The system shall provide storage of all databases on redundant computers with automatic switchover.
- The system shall provide for replication of databases to off-site storage locations.
- The system shall provide RAID V Disk Stripping on all database storage disks.

#### 3.3.2 Internet Service Provider
- The system shall provide a contractual agreement with an internet service provider for T3 access with 99.9999% availability.
- The system shall provide a contractual agreement with an internet service provider who can provide 99.999% availability through their network facilities onto the internet. 

### 3.4 Performance
- The product shall be based on web and has to be run from a web server.
- The product shall take initial load time depending on internet connection strength which also depends on the media from which the product is run.
- The performance shall depend upon hardware components of the client/customer.

### 3.5 Security

#### 3.5.1 Data Transfer
- The system shall use secure sockets in all transactions that include any confidential customer information.
- The system shall automatically log out all customers after a period of inactivity.
- The system shall confirm all transactions with the customer’s web browser.
- The system shall not leave any cookies on the customer’s computer containing the user’s password.
- The system shall not leave any cookies on the customer’s computer containing any of the user’s confidential information.

#### 3.5.2 Data Storage
- The customer’s web browser shall never display a customer’s password. It shall always be echoed with special characters representing typed characters.
- The customer’s web browser shall never display a customer’s credit card number after retrieving from the database. It shall always be shown with just the last 4 digits of the credit card number.
- The system’s back-end servers shall never display a customer’s password. The customer’s password may be reset but never shown.
- The system’s back-end servers shall only be accessible to authenticated administrators.
- The system’s back-end databases shall be encrypted.

### 3.6 Supportability

#### 3.6.1 Configuration Management Tool
- The source code developed for this system shall be maintained in configuration management tool.

### 3.7 Design Constraints

#### 3.7.1 Standard Development Tools
- The system shall be built using a standard web page development tool that conforms to either IBM’s CUA standards or Microsoft’s GUI standards.

#### 3.7.2 Web Based Product
- There are no memory requirements
- The computers must be equipped with web browsers such as Internet explorer.
- The product must be stored in such a way that allows the client easy access to it.
- Response time for loading the product should take no longer than five minutes.
- A general knowledge of basic computer skills is required to use the product

### 3.8 On-line User Documentation and Help System Requirements
- As the product is E-store, On-line help system becomes a critical component of the system which shall provide –
- It shall provide specific guidelines to a user for using the E-Store system and within the system.
- To implement online user help, link and search fields shall be provided.

### 3.9 Purchased Components
- Not Applicable

### 3.10 Interfaces
- There are many types of interfaces as such supported by the E-Store software system namely; User Interface, Software Interface and Hardware Interface.
- The protocol used shall be HTTP.
- The Port number used will be 80.
- There shall be logical address of the system in IPv4 format. 

#### 3.10.1 User Interfaces
- The user interface for the software shall be compatible to any browser such as Internet Explorer, Mozilla or Netscape Navigator by which user can access to the system.
- The user interface shall be implemented using any tool or software package like Java Applet, MS Front Page, EJB etc.

#### 3.10.2 Hardware Interfaces
- Since the application must run over the internet, all the hardware shall require to connect internet will be hardware interface for the system. As for e.g. Modem, WAN – LAN, Ethernet Cross-Cable. 

#### 3.10.3 Software Interfaces

1. The web call system shall communicate with the Configurator to identify all the available components to configure the product.

2. The web call system shall communicate with the content manager to get the product specifications, offerings and promotions.

3. The web call system shall communicate with the load balancer to determine call availability 

#### 3.10.4 Communications Interfaces

The e-store system shall use the HTTP protocol for communication over the internet and for the intranet communication will be through TCP/IP protocol suite.

#### 3.11 Licensing Requirements
- Not Applicable

#### 3.12 Legal, Copyright, and Other Notices
- Call app should display the disclaimers, copyright, word mark, trademark and product warranties of Shaowei's Angels

#### 3.13 Applicable Standards
- It shall be as per the industry standard. 