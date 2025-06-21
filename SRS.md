# Software Requirements Specification (SRS)

## 1. Introduction
This document outlines the updated requirements for the Campus Accessibility Navigation System (CANS) as part of Project Part 2.

## 2. Overall Description
CANS is designed to assist students, especially those with disabilities, in navigating campus facilities.

## 3. System Features
- Indoor navigation using QR codes
- Accessibility route suggestions
- Admin route management

## 4. Functional Requirements
- [FR1] The system shall allow users to scan QR codes for indoor positioning.
- [FR2] The system shall allow admins to add/edit/delete routes.

## 5. Non-Functional Requirements
- [NFR1] The system shall respond within 2 seconds.
- [NFR2] The system shall be accessible on Android 10+.

## 6. Assumptions and Dependencies
- Users have internet access on campus.
- Admins are registered through the university’s staff system.

## 9.6 Supporting Information

### 🔍 Validation Activities
| Type           | Description                            |
|----------------|----------------------------------------|
| Content        | Missing requirement for route feedback |
| Documentation  | Reworded NFRs for clarity              |
| Agreement      | Stakeholder request added to FR2       |

### ⚔️ Conflict Analysis and Resolution
- Conflict: Stakeholders had differing expectations for route editing.
- Resolution: Added optional note field for route instructions.

### 🔗 Requirements Traceability Matrix
| Requirement | Feature              | Goal                             |
|-------------|----------------------|----------------------------------|
| FR1         | QR Navigation        | Assist visually impaired users   |
| FR2         | Route Management     | Improve facility accessibility   |
| NFR1        | Response Time        | Enhance user experience          |

