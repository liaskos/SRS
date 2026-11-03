---
status: in progress
author:
accountable:
consult:
inform:
---
# 1. Introduction
## 1.1. Purpose
Identify the product that this SRS is about. 2-3 sentences max.
## 1.2. Document Conventions
Specify any conventions followed in this document (e.g., systematic use of **boldface**, *italics* or `monospace font`, different kinds of numbering, approach to referring and citing evidence, etc.).
## 1.3. Project Scope
2-3 sentences and reference to your vision and scope presentation - in the form of a functioning hyperlink.
# 2.  Overall Description

## 2.1. Product Perspective.
Describe how this project fits a context of other/similar or earlier projects, if any. Refer to Vision and Scope presentation as appropriate.
## 2.2. User Classes and Characteristics.
As in Vision and Scope, but refine based on any feedback, and, of course, refer to the Vision and Scope. Focus on users not stakeholders. 
## 2.3. Operating Environment.
Include commentary on: hardware, operating systems and versions, locations of users, servers and databases, hosting. Focus is on context of
operation.
## 2.4. Design and Implementation Constraints.
Include commentary on: programming languages, libraries to adopt or avoid, coding conventions, development team. Focus is on context of development.
## 2.5. Assumptions and Dependencies. 
Describe what is believed to be true at the technical level independent of desires of stakeholders or BAs. Describe also relevant dependencies. Do not duplicate content from interfaces.
# 3. System Features
## 3.0. Overview.
Offer a use case diagram of the specified system. Use case titles in the diagram must be absolutely consistent with use case documentation listed below. Then, specify the bulk of functional requirements using the following structure.

**The subsections below are examples.**
## 3.1. Assignment management
Describes the functions that an instructor can perform in order to create, subsequently manage an assignment on the system. Includes uploading the assignment statement and enabling the ability of students to submit the assignment. 
### 3.1.1. Create New Assignment
[Open](uc/3.1.1.CreateNewAssignment)
### 3.1.2. Update Assignment
[Open](uc/3.1.2.UpdateAssignment)
## 3.2. Student Report submission
Describes functions that students perform for submitting a report in response to an assignment posted by the instructor.
### 3.2.1. Submit Report
[Open](uc/3.2.1.SubmitReport)
## 3.3. ...

**The subsections above are examples.**

# 4. Data Requirements 
## 4.1. ER Diagram.
[open](datareqs/4.1.ERDiagram)
## 4.2. Data Dictionary
[open](datareqs/4.2.DataDictionary)
## 4.3. Data Acquisition, Integrity, Retention, and Disposal
[open](datareqs/4.2.AcquisitionIntegrityRetentionDisposal)
# 5. External Interface Requirements
## 5.1. User Interfaces
[open](ifaces/5.1.UI)
## 5.2. Software Interfaces
[open](ifaces/5.2.SI)
## 5.3. Hardware Interfaces
[open](ifaces/5.3.HI)
## 5.4. Communication Interfaces
[open](ifaces/5.4.CI)
# 6. Quality Attributes

## 6.1. Availability
[open](qualities/6.1.Availability)
## 6.2. Reliability
[open](6.2.Reliability.md)
## 6.3. Robustness
[open](qualities/6.3.Robustness)
## 6.4. Integrity
[open](qualities/6.4.Integrity)
## 6.5. Security
[open](qualities/6.5.Security)
## 6.6. Performance
[open](qualities/6.6.Performance)
## 6.7. Interoperability
[open](qualities/6.4.Interoperability)
# Appendices

## Glossary
[open](glossary)
## Business Rules
[open](br/BusinessRules)
## Domain Evidence
### Stakeholder 1 Interview
[open](evidence/stakeholder1interview)
### Stakeholder 2 Interview
[open](evidence/stakeholder2interview)
### Stakeholder 2 Interview
[open](evidence/stakeholder2interview)
### Report X
[open](evidence/reportX)
## Acceptance Criteria and Tests
Organize in files as appropriate. For example, per feature
### Assignment Management
[open](tests/AsignmentManagement)
### Student Report Submission
[open](tests/StudentReportSubmission)
