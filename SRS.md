![](media/image2.png){width="6.267716535433071in"
height="1.8333333333333333in"}

> **CSE6224 SOFTWARE REQUIREMENTS ENGINEERING**
>
> **PROJECT PART 1**

  -----------------------------------------------------------------------
  **NAME**                             **STUDENT ID**
  ------------------------------------ ----------------------------------
  Iusupov Alimzhan                     1231301318

  GALAL OSMAN GALAL MOHAMED            1221307698

  BALFAQIH AHMED                       1221304386

                                       
  -----------------------------------------------------------------------

## **1. Introduction**

Navigating a university campus can be challenging for individuals with
mobility or accessibility needs, especially when faced with unexpected
obstacles such as elevator outages, construction zones, or event-related
route disruptions. To address this issue, the *Campus Accessibility
Navigation System with Facilities and Event Integration* aims to provide
an intelligent, real-time navigation solution designed specifically for
accessibility.

This system will integrate live data from the university's facilities
management system and event calendar to offer users updated and
accessible route guidance. Through a user-friendly web application,
students, staff, and visitors will be able to plan their routes with
confidence, avoiding inaccessible paths and disruptions.

By focusing on accessibility, real-time updates, and integration with
existing campus infrastructure, this project promotes greater
independence, inclusivity, and efficiency across the university
environment.

### **1.1 Purpose**

The purpose of this Software Requirements Specification (SRS) is to
define the functional and non-functional requirements for the **Campus
Accessibility Navigation System with Facilities and Event Integration
(CANS)**. This system is being developed to improve mobility and
accessibility for students, staff, and visitors across the university
campus, especially for individuals with disabilities or mobility
challenges.

CANS aims to serve as a centralised, intelligent, and real-time
navigation platform that integrates with existing university
systems---including the Facilities Management System and Event
Calendar---to provide accurate and timely information about accessible
routes, infrastructure status, and campus events.

### **Primary Goals of the System:**

1.  **For Students and Campus Visitors:**

- View real-time, accessible navigation routes across campus.

- Receive automated alerts for elevator outages, construction zones, and
  route changes.

- Report accessibility issues with photo uploads and location tagging.

- Discover events with accessibility accommodations using filter
  options.

2.  **For Staff Members:**

- Update real-time facility statuses (e.g., elevators, construction).

- Add and manage event details, specifying accessibility information.

- Address and close accessibility reports submitted by users.

3.  **For Administrators:**

- Manage user roles, permissions, and system access.

- Review and approve submitted event and facility data.

- Synchronise system data with external university services.

- Generate accessibility reports and usage analytics for continuous
  improvement.

This document is intended for the project development team, university
IT administrators, QA personnel, and relevant stakeholders. It provides
a definitive guide for the design, development, validation, and
deployment of the CANS platform, ensuring that the system supports the
university\'s mission of promoting a more inclusive, accessible, and
responsive campus environment.

### **1.2 Scope**

The **Campus Accessibility Navigation System (CANS)** is a web-based
solution designed to improve mobility and navigation for individuals
across the university campus, with a strong focus on supporting those
with disabilities. By combining real-time facility data, event
schedules, and user-generated reports, the system enables students,
staff, and administrators to engage with a more inclusive, responsive
campus environment.

CANS will be developed as a responsive web application, accessible via
both mobile and desktop browsers, and will integrate with existing
university infrastructure where possible. It will address a critical gap
in accessible campus navigation by delivering timely route information,
supporting infrastructure management, and promoting accessibility-first
event planning.

### **System Capabilities and Features**

**1. Accessible Route Planning**

- Allows users to generate optimal navigation routes between locations
  on campus.

- Routing will factor in accessibility preferences such as:

1.  Avoidance of stairs

2.  Elevator availability

3.  Ramp access and wide paths

- Real-time facility data and static map data will be combined to
  produce the most appropriate paths based on user needs.

**2. Real-Time Facility Alerts**

Users will be notified of live disruptions that affect mobility,
including:

- Elevator outages

- Construction or maintenance zones

- Temporarily blocked access routes

Alerts will automatically influence route suggestions to help users
avoid inaccessible areas.

**3. Event Integration with Accessibility Information**

CANS will integrate with the university's event calendar and display
upcoming events.

Each event will include accessibility-related metadata, such as:

- Wheelchair-accessible entrances

- Reserved seating areas

- Availability of sign language interpreters

- Braille signage

Users can filter events based on available accommodations.

**4. Accessibility Issue Reporting**

Students and visitors will be able to report on-campus accessibility
issues.

Reports may include:

- Photo evidence

- Geolocation data

- Time stamps and written descriptions

Submissions will be routed to staff for review and resolution tracking.

**5. Facility and Event Data Management**

Designated staff users will have access to an administrative backend
for:

- Updating facility statuses (e.g., elevator repairs, reopened pathways)

- Creating and editing event listings with accessibility attributes

Changes will be reflected in real-time for all users.

**6. Role-Based User Access Control**

The system will enforce role-based permissions to secure access to
relevant features:

- **Students/Visitors**: View routes, receive alerts, report issues,
  browse events

- **Staff**: Manage infrastructure and event data

- **Administrators**: Manage users, approve updates, generate reports,
  and sync external data

Role-specific dashboards will ensure each user has a tailored
experience.

**7. System Monitoring and Reporting**

Administrators will be able to generate analytical and performance
reports, including:

- Frequency and resolution status of reported accessibility issues

- Most commonly used accessible routes

- System usage statistics categorised by user role

These insights will support strategic planning and continuous service
improvement.

**8. Multi-Platform Accessibility**

CANS will be accessible on:

- Mobile devices (smartphones, tablets)

- Desktop computers

The system will comply with **WCAG 2.1** accessibility standards,
supporting:

- Screen readers

- High-contrast UI options

- Keyboard-only navigation

- Multilingual interface options

### **1.3 Product Overview**

#### **1.3.1 Product Perspective**

![](media/image3.png){width="6.283464566929134in"
height="4.194444444444445in"}

*Figure 2: System Context Diagram*

  -----------------------------------------------------------------------
  Requirements   Goals                                      Author
  ID                                                        
  -------------- ------------------------------------------ -------------
  RQ-01          Generate real-time accessible campus       
                 routes using live facility and map data.   

  RQ-02          Send dynamic alerts for elevator outages,  
                 construction, and path disruptions.        

  RQ-03          Provide 24/7 multi-platform access         
                 (web/mobile) to route and facility         
                 information.                               

  RQ-04          Display and filter upcoming campus events  
                 based on accessibility accommodations.     

  RQ-05          Allow students to report accessibility     
                 issues with photo, geolocation, and        
                 description.                               

  RQ-06          Track the status and resolution of         
                 reported issues for transparency.          

  RQ-07          Support role-based access control:         
                 students, staff, and administrators with   
                 defined permissions.                       

  RQ-08          Allow staff to update facility statuses    
                 and manage event metadata from a secure    
                 backend.                                   

  RQ-09          Store accessibility metadata for campus    
                 events (e.g., ramps, signage,              
                 interpreters).                             

  RQ-10          Generate administrative reports on usage,  
                 issue trends, and accessibility KPIs.      

  RQ-11          Ensure secure integration with external    
                 systems (e.g., Facilities DB, Event        
                 Calendar) via API.                         

  RQ-12          Allow administrators and staff to manually 
                 sync data and monitor integration status.  

  RQ-13          Protect all personal data, reports, and    
                 preferences with secure data handling      
                 protocols.                                 

  RQ-14          Ensure WCAG 2.1 compliance for all UI      
                 components, including screen reader and    
                 contrast support.                          

  RQ-15          Provide multilingual support and           
                 simplified UI for cognitive and visual     
                 impairments.                               
  -----------------------------------------------------------------------

#### **1.3.2 Product Functions**

The Campus Accessibility Navigation System (CANS) offers a suite of
functionalities to support inclusive campus mobility and accessibility
for students, staff, and administrators. These functions are grouped by
role-based access and are designed to operate seamlessly through a
secure web and mobile platform.

  ---------------------------------------------------------------------------
  Function   Function Name     Description                  Actor
  ID                                                        
  ---------- ----------------- ---------------------------- -----------------
  FN-01      Log in to the     Authenticate users and       Student, Staff,
             System            provide access based on      Administrator
                               their assigned role.         

  FN-02      Plan an           Generate optimal accessible  Student
             Accessible Route  routes across campus based   
                               on user preferences.         

  FN-03      Event Status      Notify users in real-time    Student
             Alerting          about construction, elevator 
                               outages, or path blocks      

  FN-04      Accessibility     Allow students to report     Student
             Issue Reporting   accessibility problems with  
                               photos, location, and text.  

  FN-05      Report Status     Enable tracking of the       Student,
             Tracking          resolution status of         Administrator
                               submitted accessibility      
                               reports.                     

  FN-06      Track Report      View the current status of   Staff, Student
             Status            accessibility issue reports  
                               and related actions.         

  FN-07      Facility and      Update facility statuses and Staff
             Event Management  input general event details. 

  FN-08      Manage Event      Add or modify                Staff
             Information       accessibility-specific       
                               metadata for campus events.  

  FN-09      Resolve Reported  Review, address, and mark    Staff
             Issues            accessibility reports as     
                               resolved.                    

  FN-10      Report Resolution Coordinate, validate, and    Administrator,
             Workflow          finalise issue resolution    Staff
                               processes.                   

  FN-11      Data              Sync data from external      Administrator
             Synchronization   systems (e.g., facilities or 
                               event databases).            

  FN-12      User Role &       Assign roles and manage      Administrator
             Permission        access levels for system     
             Management        users.                       

  FN-13      System Monitoring Generate and view usage      Administrator
             & Reporting       statistics and issue         
                               resolution analytics.        

  FN-14      Multilingual and  Provide WCAG-compliant,      Administrator
             Accessible UI     multilingual interface and   
                               accessible design features.  
  ---------------------------------------------------------------------------

![](media/image1.png){width="6.283464566929134in"
height="7.083333333333333in"}

#### **1.3.3 User Characteristics**

The Campus Accessibility Navigation System (CANS) will be used by a
diverse group of users with varying levels of technical expertise and
accessibility needs. The design must accommodate their requirements
through intuitive interfaces, role-based access control, and
accessibility-compliant features.

  ----------------------------------------------------------------------------
  Rule            Description                     Expected Knowledge
  --------------- ------------------------------- ----------------------------
  Student         Primary users who use the       Basic familiarity with
                  system to plan accessible       mobile and web applications.
                  routes, view event              No technical background
                  accessibility info, and report  required.
                  issues.                         

  Staff           Facility managers or event      Moderate understanding of
                  organisers who update facility  digital forms, data entry
                  statuses, input event           systems, and admin
                  accessibility metadata, and     dashboards.
                  resolve reports.                

  Administrator   System administrators are       High IT proficiency.
                  responsible for managing user   Comfortable with
                  roles, monitoring system        configuration tools,
                  activity, syncing external      role-based access control,
                  data, and generating reports.   and system-level reporting.
  ----------------------------------------------------------------------------

#### **1.3.4 Limitations**

Despite its robust design, the Campus Accessibility Navigation System
(CANS) has some technical and operational limitations that must be
acknowledged:

- **Dependence on External Systems:\**
  The accuracy of real-time data (e.g., elevator outages, construction
  notices, event updates) depends on timely and accurate inputs from the
  university\'s facilities and event management systems.

- **Internet Connectivity Requirement:\**
  Since the platform is web and cloud-based, users must have an active
  internet connection to access real-time routing, alerts, and event
  data.

- **Campus-Only Scope:\**
  The navigation and accessibility features are restricted to the
  university's campus boundaries. Off-campus locations are not
  supported.

- **Manual Data Entry for Accessibility Tags:\**
  Staff are responsible for entering accessibility metadata for events
  and facilities. Incomplete or delayed updates may affect route
  accuracy or event filtering.

- **Limited Indoor Navigation Precision:\**
  Indoor mapping (e.g., within multi-story buildings) may be limited in
  precision unless further integrated with advanced positioning systems
  (planned for future versions).

- **Device Compatibility:\**
  While designed for modern browsers and devices, older hardware or
  unsupported operating systems may not provide optimal performance.

### 

### **1.4 Definitions** This section defines key terms, acronyms, and concepts used in this document to ensure clarity and consistency for all stakeholders.

  -----------------------------------------------------------------------
  Term                                Definition
  ----------------------------------- -----------------------------------
  AES Encryption                      Advanced Encryption Standard: A
                                      secure method for encrypting
                                      sensitive data.

  API                                 Application Programming Interface:
                                      A protocol enabling integration
                                      with external systems (e.g.,
                                      Facilities DB).

  Accessibility Metadata              Data describing accessibility
                                      features of campus events (e.g.,
                                      wheelchair access, sign language
                                      interpreters).

  CANS                                Campus Accessibility Navigation
                                      System: The web-based platform
                                      being developed to provide
                                      accessible navigation and
                                      event/facility management for the
                                      university.

  CCPA                                California Consumer Privacy Act: US
                                      regulation protecting consumer data
                                      rights.

  ERD                                 Entity-Relationship Diagram: A
                                      visual representation of the
                                      database structure and
                                      relationships.

  Event Participation                 A record of a user's registration
                                      or attendance at a campus event.

  Foreign Key                         A database field linking two tables
                                      to enforce referential integrity
                                      (e.g., linking Users to Reports).

  GDPR                                General Data Protection Regulation:
                                      EU regulation governing data
                                      privacy and user consent.

  Geolocation Data                    GPS or map-based coordinates
                                      identifying a user's location for
                                      route planning or issue reporting.

  Load Balancing                      Distributing network traffic across
                                      servers to optimize performance and
                                      reliability.

  Multi-Platform Accessibility        System compatibility across devices
                                      (desktop, mobile) and adherence to
                                      accessibility standards.

  Normalization                       Database design technique to
                                      minimize redundancy and ensure data
                                      integrity.

  Real-Time Facility Data             Live updates about the operational
                                      status of campus infrastructure
                                      (e.g., elevators, pathways).

  Referential Integrity               Database rule ensuring valid
                                      relationships between tables via
                                      foreign keys.

  Role-Based Access Control (RBAC)    Security model restricting system
                                      access based on user roles
                                      (Student, Staff, Administrator).

  SSL/TLS                             Secure communication protocols for
                                      encrypting data transmitted over
                                      networks.

  Static Map Data                     Pre-existing campus maps with fixed
                                      accessibility features (e.g., ramp
                                      locations, staircases).

  System Context Diagram              A visual model showing interactions
                                      between the system and external
                                      entities (e.g., users, databases).

  User-Generated Reports              Issues submitted by users (e.g.,
                                      blocked ramps, broken elevators)
                                      with photos, geolocation, and
                                      descriptions.

  WCAG 2.1                            Web Content Accessibility
                                      Guidelines 2.1: International
                                      standards for digital accessibility
                                      (e.g., screen reader
                                      compatibility).
  -----------------------------------------------------------------------

> Notes:

- Terms are ordered alphabetically for quick reference.

- Technical jargon is simplified where possible to accommodate
  non-technical readers.

- Regulatory terms (e.g., GDPR, CCPA) are included to clarify compliance
  requirements.

### 

### 

### **1.5 Apportioning of Requirements** This section outlines how the system's requirements (functional and non-functional) will be prioritized, grouped, and phased during development. Requirements are apportioned based on criticality, dependencies, resource availability, and stakeholder priorities.

## **Phase 1: Core Functionality (MVP -- Minimum Viable Product)**

> Objective: Deliver foundational features to address urgent
> accessibility needs.
>
> Requirements Included:

- RQ-01: Generate real-time accessible routes using static map data.

- RQ-02: Basic real-time alerts for elevator outages and construction.

- RQ-03: Web-based platform accessible on desktop browsers.

- RQ-07: Role-based access control for Students and Staff.

- FN-01: User authentication and login system.

- FN-02: Route planning with basic accessibility filters (e.g., avoid
  stairs).

- FN-04: Basic issue reporting without photo uploads (text-only).

- RQ-13: Data encryption for user credentials.

## **Phase 2: Enhanced Features & Event Integration**

> Objective: Expand functionality with event integration, advanced
> reporting, and mobile support.
>
> Requirements Included:

- RQ-04: Event calendar integration with accessibility metadata.

- RQ-05: Full issue reporting with photo uploads and geolocation.

- RQ-06: Report tracking dashboard for users and staff.

- RQ-09: Event accessibility metadata (e.g., interpreters, seating).

- FN-03: Real-time alert delivery via push notifications.

- FN-08: Staff backend for event accessibility tagging.

- FN-14: Mobile-responsive UI.

- RQ-15: Basic multilingual support (English + one additional language).

## **Phase 3: Advanced Features & Scalability**

> Objective: Optimize performance, add administrative tools, and ensure
> compliance.
>
> Requirements Included:

- RQ-10: Advanced analytics and reporting for administrators.

- RQ-11: API integration with external systems (Facilities DB, Event
  Calendar).

- RQ-12: Manual data sync and integration monitoring.

- RQ-14: Full WCAG 2.1 compliance (e.g., screen reader optimization).

- FN-13: System monitoring dashboard for administrators.

- FN-12: Bulk user import/export and role management.

- RQ-15: Expanded multilingual support (3+ languages).

## **Future Considerations (Post-Launch)**

> Objective: Address lower-priority or resource-intensive features.
>
> Requirements Included:

- Indoor navigation precision (e.g., building-floor mapping).

- AI-driven predictive routing (e.g., anticipating disruptions).

- Integration with IoT sensors for real-time facility monitoring.

## **Prioritization Criteria**

- Criticality: Features directly impacting accessibility (e.g., route
  planning) are prioritized.

- Dependencies: Role-based access (RQ-07) must precede staff/admin
  features.

- User Impact: High-demand features (e.g., mobile compatibility) are
  accelerated.

- Regulatory Compliance: WCAG 2.1 (RQ-14) and GDPR (RQ-13) are mandatory
  for launch.

### 

### **1.6 User Interface**

#### **1.6.1 Overview**

The *Campus Accessibility Navigation System (CANS)* user interface (UI)
is designed to provide an inclusive, intuitive, and responsive
experience across all supported platforms, namely desktop, mobile, and
tablet. The UI adheres to WCAG 2.1 accessibility standards, ensuring
compatibility with assistive technologies, such as screen readers and
keyboard navigation. Key components include:

- **Role-Specific Dashboards:**

  - Students/Visitors: Route planning, event filtering, and issue
    reporting.

  - Staff: Facility/event management and report resolution.

  - Administrators: User management, analytics, and system monitoring.

- **Interactive Campus Map:**

  - Displays real-time accessible routes, facility statuses (e.g.,
    elevator outages), and event locations.

- **Alert System:**

  - Push notifications and in-app banners for disruptions (e.g.,
    construction zones).

- **Reporting Module:**

  - Photo upload, geolocation tagging, and structured forms for
    accessibility issues.

#### **1.6.2 UI Guidelines**

- **Accessibility Standards:**

  - WCAG 2.1 AA compliance (e.g., keyboard navigation, alt text for
    images).

  - Screen reader support (ARIA labels).

  - Adjustable font sizes and high-contrast themes.

- **Consistency:**

  - Uniform color scheme (university branding) and iconography.

  - Predictable layout across all pages (e.g., navigation bar always at
    top).

- **Feedback Mechanisms:**

  - Visual cues (e.g., loading spinners) for system actions.

  - Error messages with actionable solutions (e.g., \"Please upload a
    photo to submit this report\").

- **Mobile Optimization:**

  - Touch-friendly buttons and collapsible menus.

  - Priority to core functions (route planning, alerts) on smaller
    screens.

### **1.7 External Interfaces**

#### **1.7.1 University Facilities Management System**

#### **Purpose:** Fetch real-time data on elevator outages, construction zones, and pathway closures.

#### **Interface Type:** REST API (JSON).

#### **Data Flow:**

#### CANS polls the Facilities API every 5 minutes for updates.

#### Facility status changes trigger alerts in CANS (e.g., \"Elevator B-12 out of service\").

#### **Security:** OAuth 2.0 authentication; encrypted data transmission (SSL/TLS).

#### **1.7.2 Campus Event Calendar**

#### **Purpose:** Sync event details (date, location, accessibility metadata).

#### **Interface Type:** iCal feed + custom API for accessibility tags

#### **Data Flow:**

#### Automated nightly syn

#### c for event schedules.

#### Manual override for staff to add accessibility metadata via CANS backend.

#### **Security:** API key authentication; read-only access for CANS.

## **2. References**

# **Referenced Standards, Guidelines, Tools & Technologies**

## **Standards & Guidelines**

- WCAG 2.1 (Web Content Accessibility Guidelines)

Description: International standard for web accessibility.

URL:
[[https://www.w3.org/TR/WCAG21/]{.underline}](https://www.w3.org/TR/WCAG21/)

- GDPR (General Data Protection Regulation)

Description: EU regulation for data privacy and protection.

URL: [[https://gdpr-info.eu/]{.underline}](https://gdpr-info.eu/)

- CCPA (California Consumer Privacy Act)

Description: US regulation for consumer data rights.

URL:
[[https://oag.ca.gov/privacy/ccpa]{.underline}](https://oag.ca.gov/privacy/ccpa)

- AES Encryption Standard

Description: Specification for secure data encryption.

URL:
[[https://csrc.nist.gov/publications/detail/fips/197/final]{.underline}](https://csrc.nist.gov/publications/detail/fips/197/final)

## **Tools & Technologies**

- Figma

Description: UI/UX design tool for prototyping the system interface.

URL: [[https://www.figma.com/]{.underline}](https://www.figma.com/)

- MySQL

Description: Relational database management system (RDBMS) for storing
user, facility, and event data.

URL: [[https://www.mysql.com/]{.underline}](https://www.mysql.com/)

- React.js

Description: Frontend framework for building the web application.

URL: [[https://reactjs.org/]{.underline}](https://reactjs.org/)

- Node.js

Description: Backend runtime environment for server-side logic.

URL: [[https://nodejs.org/]{.underline}](https://nodejs.org/)

## **3. Requirements**

### **3.1.1 Log in to the System**

+-------------------+--------------------------------------------------+
| Use Case ID/Name  | Log in to the System                             |
+-------------------+--------------------------------------------------+
| Precondition      | The user is registered in the system and has     |
|                   | valid credentials.                               |
+-------------------+--------------------------------------------------+
| Postcondition     | The user is authenticated and redirected to      |
|                   | their role-specific dashboard.                   |
+-------------------+--------------------------------------------------+
| Main Flow         | - The user opens the login page.                 |
|                   |                                                  |
|                   | - Enter username and password.                   |
|                   |                                                  |
|                   | - The system verifies credentials.               |
|                   |                                                  |
|                   | - System redirects to user-specific interface    |
|                   |   (Student/Staff/Admin).                         |
+-------------------+--------------------------------------------------+
| Alternate Flow    | If users forget their password, they click       |
|                   | \"Forgot Password\" and follow the recovery      |
|                   | process.                                         |
+-------------------+--------------------------------------------------+
| Exception Flow    | If the staff lacks permission or the record is   |
|                   | locked, the system blocks the update and shows   |
|                   | an appropriate message.                          |
+===================+==================================================+

### **3.1.2 Plan Accessible Route**

+-------------------+--------------------------------------------------+
| Use Case ID/Name  | Plan Accessible Routet                           |
+-------------------+--------------------------------------------------+
| Precondition      | The user is logged into the system.              |
+-------------------+--------------------------------------------------+
| Postcondition     | A recommended accessible route is displayed on   |
|                   | the map                                          |
+-------------------+--------------------------------------------------+
| Main Flow         | - Student inputs current location and            |
|                   |   destination.                                   |
|                   |                                                  |
|                   | - The system fetches real-time facility data     |
|                   |   (e.g., elevator status).                       |
|                   |                                                  |
|                   | - The system considers user preferences (e.g.,   |
|                   |   avoid stairs).                                 |
|                   |                                                  |
|                   | - The system displays the optimised accessible   |
|                   |   route on the map.                              |
+-------------------+--------------------------------------------------+
| Alternate Flow    | If real-time data is unavailable, the system     |
|                   | uses static map data to generate a basic route.  |
+-------------------+--------------------------------------------------+
| Exception Flow    | If route generation fails (e.g., no accessible   |
|                   | path found), the system notifies the user with   |
|                   | alternative suggestions (e.g., nearest help      |
|                   | desk).                                           |
+===================+==================================================+

### **3.1.3 Accessibility Issue Reporting**

+-------------------+--------------------------------------------------+
| Use Case ID/Name  | Manage Facility Data                             |
+-------------------+--------------------------------------------------+
| Precondition      | Student is logged in and at a valid reporting    |
|                   | location.                                        |
+-------------------+--------------------------------------------------+
| Postcondition     | The issue is submitted and appears in the staff  |
|                   | dashboard for review.                            |
+-------------------+--------------------------------------------------+
| Main Flow         | - Student clicks "Report Issue."                 |
|                   |                                                  |
|                   | - Uploads a photo, selects location (via GPS or  |
|                   |   map), and enters a description.                |
|                   |                                                  |
|                   | - Submits the report.                            |
|                   |                                                  |
|                   | - The system logs the issue and notifies the     |
|                   |   responsible staff.                             |
+-------------------+--------------------------------------------------+
| Alternate Flow    | If GPS is unavailable, the student selects a     |
|                   | location manually.                               |
+-------------------+--------------------------------------------------+
| Exception Flow    | If required fields are empty, the system prompts |
|                   | the user to complete them before submission.     |
+===================+==================================================+

### **3.1.4 Facility and Event Management**

+-------------------+--------------------------------------------------+
| Use Case ID/Name  | Facility and Event Management                    |
+-------------------+--------------------------------------------------+
| Precondition      | The staff member is logged in with valid         |
|                   | permissions.                                     |
+-------------------+--------------------------------------------------+
| Postcondition     | Facility or event data is updated in the system. |
+-------------------+--------------------------------------------------+
| Main Flow         | - Staff navigates to the management dashboard.   |
|                   |                                                  |
|                   | - Selects a facility (e.g., elevator) or event   |
|                   |   to update.                                     |
|                   |                                                  |
|                   | - Enters new status or adds event metadata       |
|                   |   (e.g., ramps, interpreters).                   |
|                   |                                                  |
|                   | - Saves changes.                                 |
|                   |                                                  |
|                   | - System updates the backend and refreshes       |
|                   |   user-facing information.                       |
+-------------------+--------------------------------------------------+
| Alternate Flow    | Staff uploads event details in bulk using a form |
|                   | or template.                                     |
+-------------------+--------------------------------------------------+
| Exception Flow    | If submission fails (e.g., due to missing fields |
|                   | or network error), the system displays an error  |
|                   | and logs the failure.                            |
+===================+==================================================+

### **3.1.5 Report Resolution Workflow**

+-------------------+--------------------------------------------------+
| Use Case ID/Name  | Report Resolution Workflow                       |
+-------------------+--------------------------------------------------+
| Precondition      | A reported issue exists in the system; a staff   |
|                   | member or admin is logged in.                    |
+-------------------+--------------------------------------------------+
| Postcondition     | The issue is marked resolved or otherwise        |
|                   | updated.                                         |
+-------------------+--------------------------------------------------+
| Main Flow         | - Staff reviews new issue reports.               |
|                   |                                                  |
|                   | - Verifies validity (onsite or via user input).  |
|                   |                                                  |
|                   | - Marks the issue as "Resolved," "In Progress,"  |
|                   |   or "Dismissed."                                |
|                   |                                                  |
|                   | - The reporter receives a status update.         |
+-------------------+--------------------------------------------------+
| Alternate Flow    | Admin oversees and audits the resolution history |
|                   | and status changes.                              |
+-------------------+--------------------------------------------------+
| Exception Flow    | If the staff lacks permission or the record is   |
|                   | locked, the system blocks the update and shows   |
|                   | an appropriate message.                          |
+===================+==================================================+

### **3.1.6 Event Status Alerting**

+-------------------+--------------------------------------------------+
| Use Case ID/Name  | Event Status Alerting                            |
+-------------------+--------------------------------------------------+
| Precondition      | Student is logged in; real-time event and        |
|                   | facility data are available.                     |
+-------------------+--------------------------------------------------+
| Postcondition     | Alerts are displayed in the interface or sent as |
|                   | notifications.                                   |
+-------------------+--------------------------------------------------+
| Main Flow         | - The system continuously monitors facility and  |
|                   |   event changes.                                 |
|                   |                                                  |
|                   | - If a relevant event or obstruction occurs      |
|                   |   (e.g., elevator outage), it triggers an alert. |
|                   |                                                  |
|                   | - Student receives notification on dashboard or  |
|                   |   mobile push..                                  |
+-------------------+--------------------------------------------------+
| Alternate Flow    | The student views the alert history for          |
|                   | previously triggered events.                     |
+-------------------+--------------------------------------------------+
| Exception Flow    | If alert delivery fails, the system logs the     |
|                   | error and retries or prompts the user to         |
|                   | refresh.                                         |
+===================+==================================================+

### **3.1.7 Track Report Status** 

+-------------------+--------------------------------------------------+
| Use Case ID/Name  | Track Report Status                              |
+-------------------+--------------------------------------------------+
| Precondition      | The student or staff has previously submitted or |
|                   | received an issue report.                        |
+-------------------+--------------------------------------------------+
| Postcondition     | The user can view the current status (e.g.,      |
|                   | pending, resolved).                              |
+-------------------+--------------------------------------------------+
| Main Flow         | - The user opens the "My Reports" section.       |
|                   |                                                  |
|                   | - The system displays a list of submitted or     |
|                   |   assigned reports.                              |
|                   |                                                  |
|                   | - Each report shows the current status and       |
|                   |   update history.                                |
+-------------------+--------------------------------------------------+
| Alternate Flow    | User filters reports by status or type.          |
+-------------------+--------------------------------------------------+
| Exception Flow    | If the report data fails to load, the system     |
|                   | shows an error message and a retry option.       |
+===================+==================================================+

### **3.1.8 Manage Event Information** 

+-------------------+--------------------------------------------------+
| Use Case ID/Name  | Sync with External Systems                       |
+-------------------+--------------------------------------------------+
| Precondition      | Staff are authenticated and have permission to   |
|                   | manage events.                                   |
+-------------------+--------------------------------------------------+
| Postcondition     | Accessibility information for an event is        |
|                   | updated or added.                                |
+-------------------+--------------------------------------------------+
| Main Flow         | - Staff access the event management interface.   |
|                   |                                                  |
|                   | - Selects or creates an event.                   |
|                   |                                                  |
|                   | - Adds accessibility metadata (e.g., wheelchair  |
|                   |   access, sign language).                        |
|                   |                                                  |
|                   | - Submits changes.                               |
+-------------------+--------------------------------------------------+
| Alternate Flow    | Staff imports event data from the external       |
|                   | calendar via sync.                               |
+-------------------+--------------------------------------------------+
| Exception Flow    | If metadata is missing or invalid, the system    |
|                   | shows validation errors.                         |
+===================+==================================================+

### **3.1.9 Resolve Reported Issues** 

+-------------------+--------------------------------------------------+
| Use Case ID/Name  | Resolve Reported Issues                          |
+-------------------+--------------------------------------------------+
| Precondition      | An issue has been submitted by a user and is     |
|                   | pending.                                         |
+-------------------+--------------------------------------------------+
| Postcondition     | The issue is resolved, and the status is         |
|                   | updated.                                         |
+-------------------+--------------------------------------------------+
| Main Flow         | - Staff review incoming reports in the           |
|                   |   dashboard.                                     |
|                   |                                                  |
|                   | - Investigate the issue onsite or via details.   |
|                   |                                                  |
|                   | - Takes action to resolve (e.g., repair, remove  |
|                   |   blockage).                                     |
|                   |                                                  |
|                   | - Updates the report status.                     |
+-------------------+--------------------------------------------------+
| Alternate Flow    | Staff escalates the issue to the administrator   |
|                   | or the maintenance unit.                         |
+-------------------+--------------------------------------------------+
| Exception Flow    | If staff lack the authority or resources to      |
|                   | resolve, the system flags for escalation.        |
+===================+==================================================+

### **3.1.10 Data Synchronization**

+-------------------+--------------------------------------------------+
| Use Case ID/Name  | Data Synchronization                             |
+-------------------+--------------------------------------------------+
| Precondition      | Admin is logged in, and the sync connection with |
|                   | external systems is available.                   |
+-------------------+--------------------------------------------------+
| Postcondition     | External facility or event data is updated in    |
|                   | the system.                                      |
+-------------------+--------------------------------------------------+
| Main Flow         | - Admin opens the sync interface.                |
|                   |                                                  |
|                   | - Initiates manual or automatic sync.            |
|                   |                                                  |
|                   | - System fetches and updates data from external  |
|                   |   APIs (e.g., facilities DB).                    |
|                   |                                                  |
|                   | - Status is logged.                              |
+-------------------+--------------------------------------------------+
| Alternate Flow    | The system runs a scheduled auto-sync and logs   |
|                   | sync success/failure.                            |
+-------------------+--------------------------------------------------+
| Exception Flow    | If the API connection fails, the system retries  |
|                   | or alerts the admin of the failed sync.          |
+===================+==================================================+

### **3.1.11 User Role & Permission Management**

+-------------------+--------------------------------------------------+
| Use Case ID/Name  | User Role & Permission Management                |
+-------------------+--------------------------------------------------+
| Precondition      | Admin is authenticated with configuration        |
|                   | rights.                                          |
+-------------------+--------------------------------------------------+
| Postcondition     | User roles and access levels are updated.        |
+-------------------+--------------------------------------------------+
| Main Flow         | - Admin opens the user management panel.         |
|                   |                                                  |
|                   | - View current users and roles.                  |
|                   |                                                  |
|                   | - Adds new users, assigns or changes roles       |
|                   |   (Student, Staff, Admin).                       |
|                   |                                                  |
|                   | - Saves configuration.                           |
+-------------------+--------------------------------------------------+
| Alternate Flow    | Admin imports the user list from a CSV or        |
|                   | external system.                                 |
+-------------------+--------------------------------------------------+
| Exception Flow    | If an invalid role is assigned, the system       |
|                   | blocks and shows an error.                       |
+===================+==================================================+

### **3.1.12 System Monitoring & Reporting**

+-------------------+--------------------------------------------------+
| Use Case ID/Name  | System Monitoring & Reporting                    |
+-------------------+--------------------------------------------------+
| Precondition      | Admin is logged in.                              |
+-------------------+--------------------------------------------------+
| Postcondition     | Monitoring logs or analytical reports is         |
|                   | generated.                                       |
+-------------------+--------------------------------------------------+
| Main Flow         | - Admin opens the system analytics dashboard.    |
|                   |                                                  |
|                   | - Selects report type (e.g., usage logs, issue   |
|                   |   stats).                                        |
|                   |                                                  |
|                   | - Generates and exports a report.                |
+-------------------+--------------------------------------------------+
| Alternate Flow    | Admin schedules recurring reports via system     |
|                   | tools.                                           |
+-------------------+--------------------------------------------------+
| Exception Flow    | If a data source is unavailable, the system      |
|                   | shows "report generation failed" and logs an     |
|                   | error.                                           |
+===================+==================================================+

### **3.1.13 Multilingual and Accessible UI**

+-------------------+--------------------------------------------------+
| Use Case ID/Name  | Multilingual and Accessible UI                   |
+-------------------+--------------------------------------------------+
| Precondition      | The system is running, and the user is           |
|                   | interacting with an interface.                   |
+-------------------+--------------------------------------------------+
| Postcondition     | Interface adjusts according to the user's        |
|                   | language and accessibility settings.             |
+-------------------+--------------------------------------------------+
| Main Flow         | - The user selects the preferred language or     |
|                   |   accessibility mode.                            |
|                   |                                                  |
|                   | - System updates UI with selected settings       |
|                   |   (e.g., screen reader mode, high contrast).     |
+-------------------+--------------------------------------------------+
| Alternate Flow    | Admin sets default accessibility settings per    |
|                   | role or user group.                              |
+-------------------+--------------------------------------------------+
| Exception Flow    | If the selected language is unsupported, the     |
|                   | system defaults to English and notifies the      |
|                   | user.                                            |
+===================+==================================================+

### **3.2 Performance Requirements** The system must work smoothly and efficiently for all users. Below are the key performance standards it must meet:

1.  Speed of the System

> Finding Routes: When a user asks for a route, the system should show
> it within 2 seconds most of the time.
>
> Alerts: If an elevator breaks down or a path is blocked, users should
> get a notification within 10 seconds.
>
> Reporting Issues: When a user submits a problem (like a blocked ramp),
> the system should save it within 5 seconds, even with photos.

2.  Handling Many Users at Once

> The system should work without slowing down even when 1,000+ people
> use it at the same time (e.g., during busy hours like mornings).

3.  Always Available

> The system should be up and running 99.5% of the time (24/7), except
> during planned maintenance.

4.  Managing Updates

> The system should handle 100+ updates per second (e.g., elevator
> status changes) without delays.

5.  Easy to Use on All Devices

> The website should load quickly on phones, tablets, and computers
> (within 3 seconds).

6.  Accuracy

> The map should show the user's location within 5 meters outdoors to
> help them find the best route.

7.  Reports for Admins

> When administrators generate reports (e.g., monthly usage stats), it
> should take no longer than 30 seconds.

8.  Recovery from Problems

> If the system crashes, it should restart and work normally within 5
> minutes.

9.  No Overloads

> The servers should never use more than 80% of their power, even during
> busy times, to avoid crashes.

### **3.3 Usability Requirements**

The system will attempt to meet the following usability criteria to
ensure efficiency, learnability, and satisfaction for all user roles:

- **Learnability:**

  - New users should be able to perform core tasks (e.g., plan a route,
    report an issue) within 5 minutes without prior training.

  - Contextual tooltips and an optional guided tutorial may be provided
    for first-time users.

- **Efficiency:**

  - Frequently carried out tasks (e.g., route planning) should require
    less than 3 clicks from the homepage.

  - Autocomplete for location inputs (e.g., \"Lib\" → \"Library
    Building\").

- **Error Handling:**

  - Form validation with inline feedback to prevent submission errors
    (e.g., \"Photo required for issue reports\").

  - Undo options should be provided for critical actions to prevent
    unintentional accidents (e.g., accidental report deletion).

- **Satisfaction:**

  - Post-release surveys should achieve roughly ≥ 90% positive feedback
    on ease of use.

### **3.4 Interface Requirements**

- **Hardware Interfaces:**

  - Compatible with touchscreens (mobile/tablet) and mouse/keyboard
    (desktop) input.

  - GPS support for outdoor location tracking (estimate of around 5m
    accuracy).

- **Software Interfaces:**

  - Frontend: React.js (desktop/mobile browsers).

  - Backend: Node.js APIs for data processing and business logic.

  - Database: MySQL with read replicas for scalability.

- **Communication Interfaces:**

  - HTTPS for all client-server communication, encrypted via SSL/TLS.

  - WebSocket for real-time alerts (e.g., push notifications).

# 3.5 Logical Database Requirements

3.5.1 [Entity-Relationship Diagram]{.mark}

### The Entity-Relationship Diagram (ERD) for the Campus Accessibility Navigation System (CANS) provides a structured database model to manage accessibility-related data efficiently. The design includes core entities such as Users, Facilities, Events, Reports, Notifications, and Permissions, linked through defined relationships to ensure data integrity and streamlined operations. The User entity is categorized into Students, Staff, and Admins, enabling role-based access control and functionality. Users interact with Reports to document accessibility issues and with Events to track participation in campus activities. Facilities are managed by staff, with updates triggering Notifications to inform users of relevant changes. The Permissions entity enforces security by regulating access based on user roles. Primary and foreign keys maintain relational integrity, supporting efficient data retrieval and consistency. This ERD framework facilitates real-time navigation, event management, facility oversight, and user engagement, ensuring a cohesive and secure system for accessibility management.

+-----------------------------------------------------------------------+
| > ![](media/image4.png){width="7.499876421697288in"                   |
| > height="4.760416666666667in"}                                       |
+-----------------------------------------------------------------------+
| **ERD**                                                               |
+=======================================================================+

3.5.2 Relationship

The Entity-Relationship Diagram (ERD) establishes the database structure
for efficient accessibility data management, with the User entity
serving as the central component connected to Student, Staff, and Admin
roles through one-to-one (1:1) relationships for authentication and role
differentiation. Users engage with the system by submitting Reports
through a one-to-many (1:M) relationship and managing Events via another
1:M relationship, while the Event Participation entity tracks attendee
data in a separate 1:M relationship. The Facility entity maintains a
many-to-one (M:1) relationship with Staff for management purposes and
generates Notifications through a 1:M relationship to alert users, who
receive these alerts in another 1:M configuration. The Permissions
entity enforces system security by regulating access through a 1:M
relationship. Primary and foreign keys ensure data integrity, enabling
seamless functionality across facility management, event coordination,
report handling, and user authentication within the accessibility
framework.

## 3.5.3 Data Dictionary

3.5.3.1 User Table

  -----------------------------------------------------------------------------
  ***Field   ***Data        ***Description***          ***Constraints***
  Name***    Type***                                   
  ---------- -------------- -------------------------- ------------------------
  user_id    INTEGER        Unique identifier for each PRIMARY KEY, NOT NULL,
                            user                       UNIQUE

  email      VARCHAR(225)   User email for             UNIQUE, NOT NULL
                            authentication             

  password   VARCHAR(225)   Encrypted password for     NOT NULL
                            authentication             

  role       ENUM           Defines user type          NOT NULL
  -----------------------------------------------------------------------------

3.5.3.2 Student Table

  -------------------------------------------------------------------------------
  ***Filed Name***   ***Data Type*** ***Description***   ***Constraints***
  ------------------ --------------- ------------------- ------------------------
  student_id         INTEGER         Unique identifier   PRIMARY KEY, NOT NULL,
                                     for each student    UNIQUE

  user_id            INTEGER         Foreign key linking FOREIGN KEY REFERENCES\
                                     to User table       User(user_id), UNIQUE

  enrolment_number   VARCHAR(50)     Student's           UNIQUE, NOT NULL
                                     registration number 
  -------------------------------------------------------------------------------

3.5.3.2 Stuff Table

  ----------------------------------------------------------------------------
  ***Filed        ***Data Type*** ***Description***   ***Constraints***
  Name***                                             
  --------------- --------------- ------------------- ------------------------
  stuff_id        INTEGER         Unique identifier   PRIMARY KEY, NOT NULL,
                                  for each staff      UNIQUE
                                  membe               

  user_id         INTEGER         Foreign key linking FOREIGN KEY REFERENCES
                                  to User table       User(user_id), UNIQUE

  department      VARCHAR(100)    Staff department or NOT NULL
                                  assigned unit       
  ----------------------------------------------------------------------------

3.5.3.3 Admin Table

  ---------------------------------------------------------------------------
  ***Filed        ***Data Type*** ***Description***   ***Constraints***
  Name***                                             
  --------------- --------------- ------------------- -----------------------
  admin_id        INTEGER         Unique identifier   PRIMARY KEY, NOT NULL,
                                  for each admin      UNIQUE

  user_id         INTEGER         Foreign key linking FOREIGN KEY REFERENCES
                                  to User table       User(user_id), UNIQUE

  permissions     TEXT            Admin-level access  NOT NULL
                                  rights              
  ---------------------------------------------------------------------------

3.5.3.4 Report Table

  ----------------------------------------------------------------------------
  ***Filed        ***Data Type*** ***Description***   ***Constraints***
  Name***                                             
  --------------- --------------- ------------------- ------------------------
  report_id       INTEGER         Unique identifier   PRIMARY KEY, NOT NULL,
                                  for each report     UNIQUE

  user_id         INTEGER         Foreign key linking FOREIGN KEY REFERENCES
                                  to User table       User(user_id), NOT NULL

  description     TEXT            Details of          NOT NULL
                                  accessibility issue 

  status          ENUM            Current report      ENUM(\'Pending\',
                                  status              \'Resolved\',
                                                      \'In-Progress\') NOT
                                                      NULL

  created_at      TIMESTAMP       Timestamp when the  DEFAULT
                                  report was          CURRENT_TIMESTAMP
                                  submitted           
  ----------------------------------------------------------------------------

3.5.3.5 Event Table

  ----------------------------------------------------------------------------
  ***Filed        ***Data Type*** ***Description***   ***Constraints***
  Name***                                             
  --------------- --------------- ------------------- ------------------------
  event_id        INTEGER         Unique identifier   PRIMARY KEY, NOT NULL,
                                  for each event      UNIQUE

  organizer_id    INTEGER         Foreign key linking FOREIGN KEY REFERENCES
                                  to User table       User(user_id), NOT NULL

  facility_id     INTEGER         Foreign key linking FOREIGN KEY REFERENCES
                                  to Facility table   Facility(facility_id),
                                                      NOT NULL

  event_name      VARCHAR(255)    Title or name of    NOT NULL
                                  the event           

  event_date      DATE            Scheduled date for  NOT NULL
                                  the event           
  ----------------------------------------------------------------------------

3.5.3.6 Event Participation Table

  ----------------------------------------------------------------------------------
  ***Filed Name***      ***Data Type*** ***Description***   ***Constraints***
  --------------------- --------------- ------------------- ------------------------
  participation_id      INTEGER         Unique identifier   PRIMARY KEY, NOT NULL,
                                        for event           UNIQUE
                                        attendance          

  event_id              INTEGER         Foreign key linking FOREIGN KEY REFERENCES
                                        to Event table      Event(event_id), NOT
                                                            NULL

  user_id               INTEGER         Foreign key linking FOREIGN KEY REFERENCES
                                        to User table       User(user_id), NOT NULL

  registration_status   ENUM            Attendee status     ENUM(\'Confirmed\',
                                                            \'Waitlisted\') NOT NULL
  ----------------------------------------------------------------------------------

3.5.3.7 Facility Table

  ---------------------------------------------------------------------------------
  ***Filed Name***      ***Data        ***Description***   ***Constraints***
                        Type***                            
  --------------------- -------------- ------------------- ------------------------
  facility_id           INTEGER        Unique identifier   PRIMARY KEY, NOT NULL,
                                       for each facility   UNIQUE

  facility_name         VARCHAR(255)   Name of the         NOT NULL
                                       facility            

  type                  ENUM           Facility type       ENUM(\'Elevator\',
                                       (Elevator, Ramp,    \'Ramp\', \'Room\',
                                       Room, Pathway)      \'Pathway\') NOT NULL

  status                ENUM           Current facility    ENUM(\'Operational\',
                                       operational status  \'Out-of-Service\') NOT
                                                           NULL

  last_updated          TIMESTAMP      Timestamp for last  DEFAULT
                                       update              CURRENT_TIMESTAMP

  managed_by_staff_id   INTEGER        Foreign key linking FOREIGN KEY REFERENCES
                                       to Staff table      Staff(staff_id), NOT
                                                           NULL
  ---------------------------------------------------------------------------------

3.5.3.8 Notification Table

  ------------------------------------------------------------------------------
  ***Filed Name***  ***Data Type*** ***Description***   ***Constraints***
  ----------------- --------------- ------------------- ------------------------
  notification_id   INTEGER         Unique identifier   PRIMARY KEY, NOT NULL,
                                    for each            UNIQUE
                                    notification        

  facility_id       INTEGER         Foreign key linking FOREIGN KEY REFERENCES
                                    to Facility table   Facility(facility_id),
                                                        NOT NULL

  user_id           INTEGER         Foreign key linking FOREIGN KEY REFERENCES
                                    to User table       User(user_id), NOT NULL

  message           TEXT            Notification        NOT NULL
                                    content             

  timestamp         TIMESTAMP       Timestamp when      DEFAULT
                                    notification was    CURRENT_TIMESTAMP
                                    sent                
  ------------------------------------------------------------------------------

3.5.3.9 Permission Table

  ---------------------------------------------------------------------------
  ***Filed        ***Data Type*** ***Description***   ***Constraints***
  Name***                                             
  --------------- --------------- ------------------- -----------------------
  permission_id   INTEGER         Unique identifier   PRIMARY KEY, NOT NULL,
                                  for access          UNIQUE
                                  permissions         

  user_id         INTEGER         Foreign key linking FOREIGN KEY REFERENCES
                                  to User table       User(user_id), NOT NULL

  access_level    ENUM            Defines access      ENUM(\'View\',
                                  rights              \'Edit\', \'Manage\')
                                                      NOT NULL
  ---------------------------------------------------------------------------

## 3.6 Design Constraints

The Design Constraints Table outlines the key limitations and
requirements for the development of the Campus Accessibility Navigation
System (CANS). The constraints are organized into technical,
environmental, and regulatory categories to guide system development.

Technical constraints include database scalability, real-time
notifications, role-based access control, and security encryption.
Environmental constraints cover device compatibility, network
limitations, and accessibility compliance. Regulatory constraints
involve data privacy laws, facility accessibility standards, and legal
record-keeping requirements.

Each constraint is assigned a priority level to guide development focus.
These constraints ensure the system meets performance, usability, and
compliance standards while remaining scalable and secure.

  -----------------------------------------------------------------------------------------------
  ***ID***          ***Constraint***   ***Description***                         ***Priority***
  ----------------- ------------------ ----------------------------------------- ----------------
  ***REQ_DC001***   Database           The system must efficiently handle large  High
                    Scalability        volumes of users, reports, events, and    
                                       notifications while ensuring fast data    
                                       retrieval and query execution. Indexing   
                                       and optimized relational mapping should   
                                       be implemented to maintain performance.   

  ***REQ_DC002***   Real-time          Facility updates must trigger immediate   High
                    Notifications      notifications to affected users, ensuring 
                                       timely awareness of accessibility         
                                       changes. Asynchronous processing and      
                                       message queuing may be required for       
                                       scalability.                              

  ***REQ_DC003***   Role-Based Access  Role-based permissions must be enforced   High
                    Control (RBAC)     to control data access for Students,      
                                       Staff, and Admins, preventing             
                                       unauthorized actions while ensuring a     
                                       seamless user experience.                 

  ***REQ_DC004***   Security & Data    Sensitive user data, including            High
                    Protection         authentication credentials and reports,   
                                       must be encrypted and stored securely.    
                                       Secure protocols such as **AES            
                                       encryption**, **SSL/TLS** for data        
                                       transmission, and regular security audits 
                                       should be enforced.                       

  ***REQ_DC005***   Multi-Platform     The system must be accessible across      Medium
                    Compatibility      different platforms, including desktops,  
                                       mobile devices, and tablets, with         
                                       responsive UI design and adaptive         
                                       components for various screen             
                                       resolutions.                              

  ***REQ_DC006***   Accessibility      The user interface must comply with       High
                    Compliance         **WCAG 2.1 standards**, ensuring          
                                       usability for individuals with            
                                       disabilities through features like screen 
                                       reader compatibility, keyboard            
                                       navigation, and adjustable contrast       
                                       settings.                                 

  ***REQ_DC007***   Device & Network   The system should function on low-end     Medium
                    Limitations        devices and operate efficiently in        
                                       low-bandwidth environments by optimizing  
                                       resource usage and minimizing heavy       
                                       processing requirements.                  

  ***REQ_DC008***   Localization &     Multi-language functionality should be    Low
                    Language Support   supported based on user demographics,     
                                       ensuring accessibility for a diverse      
                                       audience.                                 

  ***REQ_DC009***   Server             The hosting environment must be optimized High
                    Infrastructure     for **scalability**, **load balancing**,  
                                       and **failover mechanisms** to maintain   
                                       system stability during peak usage        
                                       periods. Cloud-based solutions should be  
                                       considered for reliability.               

  ***REQ_DC010***   Data Privacy &     The system must comply with global and    High
                    Compliance         local data protection laws, including     
                                       **GDPR**, **CCPA**, and institutional     
                                       guidelines to protect user privacy and    
                                       prevent unauthorized data exposure.       

  ***REQ_DC011***   Public Facility    The system must align with government and High
                    Regulations        institutional accessibility policies to   
                                       ensure proper tracking of infrastructure  
                                       updates.                                  

  ***REQ_DC012***   Legal              Reports and facility updates must be      High
                    Record-Keeping     stored securely with **audit logs**,      
                                       ensuring traceability and preventing data 
                                       manipulation to maintain accountability.  

  ***REQ_DC013***   Copyright &        The system must enforce copyright         Medium
                    Intellectual       compliance, ensuring that all stored and  
                    Property           shared content adheres to legal           
                                       regulations and ethical usage policies.   
  -----------------------------------------------------------------------------------------------

### **3.7 Software System Attributes** These attributes define the overall quality and operational characteristics of the Campus Accessibility Navigation System (CANS):

> 1\. Reliability
>
> The system shall operate consistently under normal use, with ≤ 1
> critical failure per month.
>
> Real-time updates (e.g., elevator statuses, route changes) must be
> accurate and reflect the latest facility data.
>
> User-submitted reports shall be stored without loss of data (e.g.,
> photos, geolocation).
>
> 2\. Availability
>
> The system shall be accessible 24/7, with scheduled maintenance
> limited to ≤ 2 hours per month.
>
> During peak hours (8 AM--5 PM), uptime shall remain ≥ 99.5%.
>
> 3\. Security
>
> All user data (passwords, reports, preferences) shall be encrypted
> using AES-256 encryption.
>
> Role-based access control (RBAC) shall prevent unauthorized users from
> accessing sensitive features (e.g., staff dashboards).
>
> 4\. Maintainability
>
> The codebase shall be modular, with clear documentation for future
> updates (e.g., adding new accessibility filters).
>
> Database backups shall be performed daily to enable quick recovery
> from failures.
>
> 5\. Portability
>
> The web application shall function on Chrome, Firefox, Safari, and
> Edge browsers (latest stable versions).
>
> Mobile responsiveness shall ensure usability on devices with screen
> sizes ≥ 5 inches.
>
> 6\. Compliance
>
> The UI shall fully comply with WCAG 2.1 AA standards for
> accessibility.
>
> Data handling shall adhere to GDPR and CCPA regulations for user
> privacy.
>
> 7\. Scalability
>
> The system shall support a 20% annual increase in users without
> requiring architectural changes.

### 

### **3.8 Supporting Information** 

> Balancing \"Must-Have\" Minorities:This section provides context for
> the system's requirements based on the Kano Model survey conducted
> during the requirements elicitation phase. The results explain how
> user feedback shaped the prioritization and categorization of
> features, even though most responses fell into the \"Indifferent\"
> category.

## **1. Elicitation Methodology**

- Technique:

> A Kano Model survey was distributed via Google Forms to gather user
> preferences for accessibility and navigation features.

- Execution:

> Survey Link: Shared via class WhatsApp groups and social media.
>
> Duration: Open for 2 weeks (May 7--21, 2025).

- Participants:

> Total submissions: 45
>
> Valid responses (complete Kano pairs): 30

- Analysis:

> A Python script categorized responses into Kano categories (Must-Have,
> Attractive, Indifferent, Reverse, etc.).

## **2. Survey Results and Requirement Mapping**

> The table below summarizes the Kano categorization of features and
> their linkage to system requirements:

  ---------------------------------------------------------------------------------
  Feature             Kano Category  Counts         Linked         Interpretation
                                                    Requirements   
  ------------------- -------------- -------------- -------------- ----------------
  Accessible routes   Indifferent    I:25, A:15,    RQ-01, FN-02   Neutral
  across campus                      E:1, M:3                      reception;
                                                                   prioritized due
                                                                   to institutional
                                                                   accessibility
                                                                   mandates.

  Real-time elevator  Indifferent    I:23, A:14,    RQ-02, FN-03   Some users
  outage alerts                      R:2, M:5                      expect alerts
                                                                   (M), but most
                                                                   indifferent.
                                                                   Critical for
                                                                   compliance.

  Live                Indifferent    I:21, A:17,    RQ-02, FN-03   Helpful for
  construction/path                  R:2, M:4                      safety; retained
  information                                                      despite neutral
                                                                   feedback.

  Event-based         Indifferent    I:21, A:14,    RQ-04, RQ-09   Notable
  rerouting                          M:7, R:1                      \"Must-Have\"
                                                                   (M) subgroup
                                                                   justified
                                                                   inclusion.

  Speech/screen       Indifferent    I:27, A:14,    RQ-14          Basic
  reader support                     M:3                           accessibility
                                                                   expectation;
                                                                   required for
                                                                   WCAG 2.1
                                                                   compliance.
  ---------------------------------------------------------------------------------

> Key: I: Indifferent, A: Attractive, M: Must-Have, R: Reverse, E:
> Excitement

## **3. Implications for System Design**

- Indifferent Features as Requirements:

> Despite neutral user responses, features like accessible routes
> (RQ-01) and screen reader support (RQ-14) were prioritized to comply
> with university accessibility policies and WCAG 2.1 standards.

- 

> Features with notable \"Must-Have\" votes (e.g., event-based
> rerouting) were prioritized to serve niche but critical user needs.

## **4. Limitations of Elicitation**

> • Sample Bias: Most respondents were tech-savvy students; staff and
> visitors were underrepresented.
>
> • Scope: The survey focused on usability, not technical feasibility
> (e.g., API integration challenges in RQ-11).

## **5. Supporting Artifacts**

> • Raw Data: Survey responses stored in a CSV file (see repository).
>
> • Python Script: Automated Kano categorization tool (shared with the
> development team).
>
> • Survey Design: can be seen from the link
> [[https://docs.google.com/forms/d/e/1FAIpQLSc9RD4jTCL5mbspPtAizovIrXu8ecASnML_RfMZHT-r71SQIw/viewform?usp=header]{.underline}](https://docs.google.com/forms/d/e/1FAIpQLSc9RD4jTCL5mbspPtAizovIrXu8ecASnML_RfMZHT-r71SQIw/viewform?usp=header)

### 

### 

## 

## **4. Verification**

### **4.1 Functions Verification**

The **Campus Accessibility Navigation System (CANS)** includes a range
of user-facing and administrative functions that must be verified to
ensure they meet the defined requirements and support real-world usage
by students, staff, and administrators. This section outlines how each
major function will be verified through interaction testing, role-based
checks, and validation of expected behavior.

Each function corresponds to one or more use cases and requirement IDs
defined earlier. Verification focuses on ensuring the correctness,
completeness, and usability of system features as experienced by all
types of users.

### **4.2 Performance Verification**

This section outlines the procedures to verify that the Campus
Accessibility Navigation System (CANS) meets its performance
requirements. Each requirement from Section 3.2 is mapped to a
verification method, success criteria, and tools used for testing.

  ------------------------------------------------------------------------
  Requirement       Verification      Tools/Techniques   Success Criteria
                    Method                               
  ----------------- ----------------- ------------------ -----------------
  Route generation  Simulate 500      JMeter, Postman    95% of requests
  ≤ 2 seconds       concurrent users                     complete within 2
                    requesting                           seconds.
                    routes; measure                      
                    average response                     
                    time.                                

  Alerts ≤ 10       Trigger an        Selenium, Manual   Alert delivered
  seconds           elevator outage   Testing            within 10 seconds
                    and measure time                     to all affected
                    until the alert                      users.
                    appears on user                      
                    devices.                             

  Report submission Submit 100        JMeter, AWS        All reports saved
  ≤ 5 seconds       reports with      LoadRunner         within 5 seconds.
                    photos                               
                    simultaneously;                      
                    track processing                     
                    time.                                

  Handle 1,000+     Simulate 1,200    LoadNinja,         No errors or
  concurrent users  users accessing   BlazeMeter         crashes; response
                    the system during                    times remain
                    peak hours (8                        within acceptable
                    AM--5 PM).                           thresholds.

  99.5% uptime      Monitor system    Nagios,            System available
                    availability over UptimeRobot        ≥ 99.5% of the
                    30 days using                        time, excluding
                    uptime tracking                      scheduled
                    tools.                               maintenance.

  100+              Send 150          Postman, AWS       API processes ≥
  updates/second    updates/second to Lambda             100
                    the Facilities                       updates/second
                    API and monitor                      with ≤ 500ms
                    processing                           latency.
                    latency.                             

  Load time ≤ 3     Test page load    Google Lighthouse, All pages load
  seconds           times on mobile   WebPageTest        within 3 seconds
                    (Chrome, Safari)                     on devices with ≥
                    and desktop                          5-inch screens.
                    (Firefox, Edge)                      
                    browsers.                            

  Geolocation ≤ 5m  Compare           GPS Visualizer,    Location accuracy
  accuracy          system-reported   Manual Testing     within 5 meters
                    user location                        for 95% of tests.
                    with GPS                             
                    benchmarks in                        
                    outdoor campus                       
                    areas.                               

  Admin reports ≤   Generate a usage  MySQL Workbench,   Report generated
  30 seconds        report covering 6 Custom Scripts     within 30
                    months of data;                      seconds.
                    measure                              
                    processing time.                     

  Recovery ≤ 5      Simulate a server AWS CloudWatch,    System fully
  minutes           crash and measure Manual Testing     operational
                    time to restore                      within 5 minutes.
                    functionality.                       

  Server capacity ≤ Monitor           New Relic, Datadog Server resource
  80%               CPU/memory usage                     usage never
                    during peak load                     exceeds 80%.
                    (1,200 users).                       
  ------------------------------------------------------------------------

## **Verification Process**

Test Environment:\
\
• Use cloud servers (AWS EC2) to replicate production conditions.\
• Simulate campus Wi-Fi speeds (50 Mbps download/20 Mbps upload).

Data Collection:\
\
• Log response times, errors, and resource usage during tests.\
• Validate geolocation accuracy using campus landmarks (e.g., library,
cafeteria).

Reporting:\
\
• Document results in a verification report, highlighting any deviations
from success criteria.\
• Retest failed scenarios after fixes.

## **Pass/Fail Criteria**

Pass: All success criteria are met for ≥ 95% of test cases.\
\
Fail: Any critical requirement (e.g., uptime, route generation) fails
more than 5% of tests.

### 

### **4.3 Usability Verification**

  ---------------------------------------------------------------------------------
  **Requirement**   **Verification        **Success Criteria**    **Possible
                    Method**                                      Tools**
  ----------------- --------------------- ----------------------- -----------------
  Learnability      Observe 10 new users  90% complete tasks      UserTesting.com
                    performing core       within 5 minutes.       
                    tasks.                                        

  Efficiency        Log clicks for 50     ≤ 3 clicks to generate  Hotjar, Google
                    route-planning        a route.                Analytics
                    sessions.                                     

  Error Recovery    Simulate 20 erroneous 100% receive actionable Jest, Selenium
                    form submissions.     error messages.         

  Satisfaction      Post-release survey   ≥ 4.0 average           SurveyMonkey
                    (Likert scale 1--5).  satisfaction score.     
  ---------------------------------------------------------------------------------

### 

### **4.4 Interface Verification**

  ---------------------------------------------------------------------------
  **Component**   **Test**                **Success Criteria** **Possible
                                                               Tools**
  --------------- ----------------------- -------------------- --------------
  Facilities API  Mock outage data →      Alerts appear within Postman, Jest
                  validate alert          10 seconds.          
                  triggers.                                    

  Event Calendar  Compare iCal feed with  100% data parity     Python scripts
  Sync            CANS event listings.    after sync.          

  GPS Accuracy    Test at 10 campus       Location accuracy ≤  Google Maps
                  landmarks.              5m.                  API

  Cross-Browser   Render UI on Chrome,    Consistent           BrowserStack
  Support         Safari, Firefox, Edge.  functionality        
  ---------------------------------------------------------------------------

**Verification Process:**

- Test Environment: AWS cloud servers replicating production.

- Pass/Fail: ≥ 95% success rate for all criteria.

### 

### **4.5 Logical Database Verification**

[The logical database verification process involves systematic
validation activities to ensure the database design meets specified
system requirements and stakeholder expectations. These verification
procedures focus on confirming proper database normalization to
eliminate redundancy and maintain structural efficiency. Indexing
strategies are evaluated to optimize query performance and data
retrieval operations. Relationship integrity checks validate the correct
implementation of primary and foreign key constraints across database
tables. Security protocols are reviewed to confirm appropriate data
protection measures are in place. These verification activities
collectively ensure the database maintains data integrity, supports
consistent operations, and delivers optimal performance. The process
contributes to the system\'s overall reliability, scalability, and
ability to effectively manage user interactions, content organization,
and real-time data processing requirements.]{.mark}

4.5.1 Verification Procedures

  -----------------------------------------------------------------------
  ***[Verification                ***[Description]{.mark}***
  Step]{.mark}***                 
  ------------------------------- ---------------------------------------
  ***[Schema                      [Ensures all tables, primary keys, and
  Validation]{.mark}***           foreign keys are properly defined
                                  according to relational database
                                  principles]{.mark}

  ***[Referential                 [Confirms that all foreign key
  Integrity]{.mark}***            constraints correctly enforce
                                  relationships and prevent orphaned
                                  records.]{.mark}

  ***[Normalization               [Validates that the schema follows
  Check]{.mark}***                **normalization rules (up to 3NF)** to
                                  minimize data redundancy and ensure
                                  efficient data storage.]{.mark}

  ***[Data Type                   [Verifies that each column has the
  Accuracy]{.mark}***             appropriate data type to maintain data
                                  consistency and prevent processing
                                  errors.]{.mark}

  ***[Unique & Not Null           [Ensures primary keys are **unique**,
  Constraints]{.mark}***          and mandatory fields are enforced using
                                  **NOT NULL constraints**.]{.mark}

  ***[Index                       [Confirms that indexes are correctly
  Optimization]{.mark}***         applied to frequently queried fields,
                                  improving database query
                                  efficiency]{.mark}

  ***[Relationship                [Verifies that **one-to-many (1:M),
  Consistency]{.mark}***          many-to-one (M:1), and one-to-one (1:1)
                                  relationships** between entities align
                                  with the expected system
                                  behavior.]{.mark}

  ***[Security & Access           [Validates that **role-based
  Controls]{.mark}***             permissions** are correctly implemented
                                  to prevent unauthorized access and
                                  protect sensitive data.]{.mark}
  -----------------------------------------------------------------------

### 

### **4.6 Design Constraints Verification**

[The Design Constraints Verification process outlines the methods for
validating each constraint identified in [**[section
3.6]{.underline}**](#design-constraints) throughout system development.
This verification ensures compliance with technical specifications,
environmental requirements, and regulatory standards while confirming
the system\'s functionality and performance capabilities. For technical
constraints, verification will involve testing database scalability,
access control mechanisms, and security protocols. Environmental
constraints will be validated through compatibility testing across
devices and network conditions, along with accessibility compliance
checks. Regulatory requirements will be verified through documentation
reviews and compliance audits. These verification activities serve to
objectively demonstrate that all design constraints have been properly
implemented and that the final system meets both technical
specifications and stakeholder expectations across all constraint
categories.]{.mark}

  -----------------------------------------------------------------------------------
  ***[ID]{.mark}***          ***[Constaint]{.mark}***   ***[Verification
                                                        method]{.mark}***
  -------------------------- -------------------------- -----------------------------
  ***[REQ_DC001]{.mark}***   [Database                  [Load testing and stress
                             Scalability]{.mark}        tests will be conducted to
                                                        measure the system\'s ability
                                                        to handle increasing data
                                                        volumes efficiently]{.mark}

  ***[REQ_DC002]{.mark}***   [Real-Time                 [System stress testing and
                             Notifications]{.mark}      event simulations will
                                                        confirm timely notification
                                                        delivery without
                                                        delays.]{.mark}

  ***[REQ_DC003]{.mark}***   [Role-Based Access Control [Unit testing will validate
                             (RBAC)]{.mark}             user permissions by ensuring
                                                        restricted access for
                                                        different roles]{.mark}

  ***[REQ_DC004]{.mark}***   [Security & Data           [Security audits, penetration
                             Protection]{.mark}         testing, and encryption
                                                        validation will ensure data
                                                        is protected against
                                                        unauthorized access.]{.mark}

  ***[REQ_DC005]{.mark}***   [Multi-Platform            [Cross-device testing across
                             Compatibility]{.mark}      desktop, mobile, and tablet
                                                        interfaces will verify UI
                                                        adaptability and
                                                        performance.]{.mark}

  ***[REQ_DC006]{.mark}***   [Accessibility             [WCAG 2.1 compliance testing
                             Compliance]{.mark}         will ensure usability for
                                                        individuals with
                                                        disabilities, including
                                                        screen reader and keyboard
                                                        navigation tests.]{.mark}

  ***[REQ_DC007]{.mark}***   [Device & Network          [Performance testing on
                             Limitations]{.mark}        low-end devices and
                                                        simulations in low-bandwidth
                                                        environments will verify
                                                        system efficiency]{.mark}

  ***[REQ_DC008]{.mark}***   [Localization & Language   [Language selection testing
                             Support]{.mark}            and UI validation will ensure
                                                        accurate translations and
                                                        proper layout
                                                        adjustments.]{.mark}

  ***[REQ_DC009]{.mark}***   [Server                    [Load balancing and failover
                             Infrastructure]{.mark}     testing will validate system
                                                        reliability during peak
                                                        traffic and hardware
                                                        failures.]{.mark}

  ***[REQ_DC010]{.mark}***   [Data Privacy &            [GDPR and data protection
                             Compliance]{.mark}         compliance audits will be
                                                        performed to ensure secure
                                                        user data handling.]{.mark}

  ***[REQ_DC011]{.mark}***   [Public Facility           [Institutional review and
                             Regulations]{.mark}        accessibility policy
                                                        validation will confirm
                                                        adherence to facility
                                                        management standards.]{.mark}

  ***[REQ_DC011]{.mark}***   [Legal                     [Automated logging and
                             Record-Keeping]{.mark}     integrity tests will verify
                                                        accurate storage of reports
                                                        and facility updates for
                                                        auditing purposes.]{.mark}

  ***[REQ_DC012]{.mark}***   [Copyright & Intellectual  [Legal review of digital
                             Property]{.mark}           content storage and
                                                        distribution policies will
                                                        ensure compliance with
                                                        copyright
                                                        regulations.]{.mark}
  -----------------------------------------------------------------------------------

### **4.7 Software System Attributes Verification**

This section describes how the **quality attributes** of the Campus
Accessibility Navigation System (CANS) will be verified to ensure that
the system meets operational, performance, and compliance expectations.

  ---------------------------------------------------------------------------
  Attribute         Verification Method           Success Criteria
  ----------------- ----------------------------- ---------------------------
  Reliability       Conduct continuous usage      ≤ 1 critical failure per
                    simulations under normal and  month; data (e.g., reports,
                    peak load conditions.         routes) saved without loss.

  Availability      Monitor system uptime via     ≥ 99.5% uptime (excluding ≤
                    tools (e.g., UptimeRobot,     2 hours/month for scheduled
                    Nagios) over a 30-day window. maintenance).

  Security          Perform penetration testing,  AES-256 encryption, secure
                    encryption validation, and    password storage, no
                    access control testing.       unauthorised access to any
                                                  feature.

  Maintainability   Review source code modularity Clear module boundaries;
                    and documentation; evaluate   daily backups confirmed;
                    backup systems.               future updates supported
                                                  easily.

  Portability       Conduct compatibility testing The system functions
                    across latest versions of     properly on all tested
                    Chrome, Safari, Edge, and     devices and browsers.
                    Firefox on various devices.   

  Compliance        Validate system against WCAG  Full WCAG 2.1 AA
                    2.1 AA accessibility          compliance; no unencrypted
                    standards and GDPR/CCPA data  user data; user privacy
                    handling guidelines           settings active.

  Scalability       Simulate 20% annual user      System performs smoothly
                    growth and measure system     without architectural
                    performance and resource      changes or performance
                    usage.                        degradation.
  ---------------------------------------------------------------------------

### **4.8 Supporting Information Verification**

This section outlines how the requirements elicited using the **Kano
Model** were validated and mapped to system functions, ensuring that
stakeholder feedback shaped the final product design-even when responses
indicated mixed priorities.

**4.8.1 Verification of Elicitation Validity**

- **Technique**: Kano Model-based survey

- **Execution**: Google Forms

- **Cross-validation**: Mapped Kano categories to corresponding
  requirements (e.g., RQ-01, FN-02).

**4.8.2 Mapping Survey to System Requirements**

  ---------------------------------------------------------------------------
  Feature             Kano Category                Design Justification
  ------------------- ---------------------------- --------------------------
  Accessible routes   Mostly Indifferent           Prioritized for compliance
  across campus                                    with accessibility
                                                   standards.

  Elevator outage     Indifferent / Must-Have      Included due to compliance
  alerts                                           needs and safety concerns.

  Construction/path   Indifferent / Attractive     Important for accurate
  disruptions                                      real-time routing.

  Event accessibility Some Must-Have responses     Retained to support
  filtering                                        inclusive campus event
                                                   participation.

  Screen              Indifferent / Must-Have      Required for WCAG 2.1
  reader/speech                                    compliance and inclusive
  support                                          design.
  ---------------------------------------------------------------------------

**4.8.3 Elicitation Gaps & Adjustments**

- **Underrepresented Roles: Staff and visitors were underrepresented in
  the survey.**

- **Design Adjustment: Despite neutral responses, features were retained
  to meet university policy and legal requirements (e.g., WCAG, GDPR).**

## **5. Appendices**

### **5.1 Assumptions and Dependencies**

\- All users have access to internet-enabled devices (smartphones,
tablets, laptops).

\- The university facilities and event databases provide accurate and
timely data via APIs.

\- Users will report accessibility issues honestly and with relevant
evidence (e.g., photos).

\- The university administration supports and enforces the use of the
system among departments.

\- Integration with external systems: University Facilities Management
System and Event Calendar API.

\- Real-time data availability from third-party systems (e.g., elevator
status).

\- Availability of accurate campus map data including accessibility
metadata.

\- Continuous collaboration from IT and Accessibility departments during
development and deployment.

### **5.2 Acronyms and Abbreviations**

Refer to [[Section
1.4]{.underline}](#definitions-this-section-defines-key-terms-acronyms-and-concepts-used-in-this-document-to-ensure-clarity-and-consistency-for-all-stakeholders.)
-- Definitions -- for the full list of acronyms and abbreviations used
in this document.


## **6. Supporting Information**

### **6.1 Validation Sessions**

| **Session ID** | **Date and Time**     | **Technique** | **Section Reviewed** | **Participant & Role**                                               | **No. of Defect** |
|----------------|-----------------------|---------------|-----------------------|---------------------------------------------------------------------|-------------------|
| VS-01          | 2/6/2025; 10am–2pm    | Inspection    | 2.1, 3.2, 3.3         | Alice (Inspector), Ben (Inspector), Chen (Moderator)                | 7                 |
| VS-02          | 3/6/2025; 2pm–6pm     | Inspection    | 3.4, 3.5              | Chen (Inspector), Dana (Author), Ben (Presenter), Alice (Inspector) | 5                 |


### **6.2 Defect Summary**

#### **A. Content Defects**

| **Req ID** | **Validation and Defect Description** | **Detected By** | **Comment/Suggested Fix**       | **Session ID** | **Severity (1–5)** |
|-----------|----------------------------------------|-----------------|----------------------------------|----------------|--------------------|
| REQ-001   | Missing acceptance criteria            | Alice           | Define measurable outcomes       | VS-01          | 4                  |
| REQ-004   | “Fast” not defined                     | Ben             | ≤ 2s response time               | VS-01          | 3                  |

#### **B. Documentation Defects**

| **Page No.** | **Validation and Defect Description** | **Detected By** | **Comment/Suggested Fix** | **Session ID** | **Severity (1–5)** |
|--------------|----------------------------------------|-----------------|----------------------------|----------------|--------------------|
| Pg 3         | Outdated policy reference              | Chen            | Replace with Policy 102    | VS-02          | 2                  |

#### **C. Agreement Defects**

| **Req ID**  | **Validation Description / Stakeholder Concern** | **Mismatch**               | **Detected By** | **Session ID** | **Severity (1–5)** |
|-------------|--------------------------------------------------|-----------------------------|-----------------|----------------|--------------------|
| REQ-012     | 24/7 uptime without failover                     | Operational feasibility gap | Ben             | VS-02          | 5                  |


### **6.3 Conflict Analysis**

| **Conflict ID** | **Conflict Description**         | **Conflict Analysis**                                                                                                                                                 | **Stakeholders Involved** | **Session ID** |
|-----------------|----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------|----------------|
| CF-01           | Performance vs cost tradeoff     | Interest conflict – the QA and Development teams prioritized high performance, while the Product Owner (PO) emphasized minimizing costs. The underlying cause is differing role-based objectives: QA and Dev aim to ensure system reliability and responsiveness, while PO focuses on budget. | PO, QA, Dev Team           | VS-01          |


### **6.4 Conflict Resolution**

| **Conflict ID** | **Conflict Resolution Strategy**                                                                                          | **Resolved (Y/N)** | **Outcome (If Resolved)**                                                                                 | **Justification**                                                                                                                |
|-----------------|----------------------------------------------------------------------------------------------------------------------------|--------------------|-----------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
| CF-01           | Structured negotiation facilitated by the Scrum Master, including trade-off analysis and review of stakeholder priorities. | Y                  | Agreement reached to prioritize performance, with acceptable cost adjustments approved by the PO.         | The resolution process considered stakeholder goals and project constraints, resulting in a sustainable and well-justified agreement. |

---

### **6.5 Change Log**

| **Change ID** | **Req ID(s)** | **Summary of Change**           | **Proposed By** | **Date**       | **Session ID** |
|---------------|---------------|----------------------------------|-----------------|----------------|----------------|
| CH-01         | REQ-001       | Added acceptance criteria       | Alice           | dd-mm-yyyy     | VS-01          |
| CH-02         | REQ-012       | Adjusted uptime expectation     | Ben             | dd-mm-yyyy     | VS-02          |

---

### **6.6 Requirements Traceability Matrix**

| **Req ID** | **Requirement Description**  | **Linked Goal(s)** | **Feature(s)** | **Use Case(s)** | **Traceability Score (1–4)** | **Description**                                                              |
|-----------|-------------------------------|---------------------|----------------|------------------|-------------------------------|------------------------------------------------------------------------------|
| REQ-001   | System shall respond <2s       | G1                  | F1             | UC-01            | 4                             | Linked to 3 artifacts with high confidence, correctness, and completeness   |
| REQ-004   | Real-time notifications        | G2                  | F3             | UC-04            | 3                             | Linked to 3 artifacts, but links may be basic or unverified                 |

---

### **6.7 Roles in Validation & Management**

| **Name** | **Primary Responsibility**                                     | **No. of Sessions Participated** |
|---------|---------------------------------------------------------------  |----------------------------------|
| Alice   | Content validation, traceability matrix                         | 2                                |
| Ben     | GitHub version control, changelog maintenance, conflict logging | 2                                |
| Chen    | Conflict analysis, stakeholder concern tracking                 | 2                                |
| Dana    | Documentation review, defect classification                     | 1                                |

---

### **6.8 Version Control & Configuration**

| **Repo Branch**          | **Key Files**                                                                 |
|--------------------------|-------------------------------------------------------------------------------|
| `project-part-2`         | - `SRS.md`: Working version of updated SRS                                    |
|                          | - `TTXL_GX_SRS.doc`: Final version                                            |
|                          | - `changelog.md`: Record of all requirement-related changes                   |
|                          |                                                                               |
| **Commits by StudentX**                 | XX                                                             |
| **Pull Requests Merged by StudentX**    | XX                                                             |
| **Change Log Entries Made by StudentX** | XX                                                             |


