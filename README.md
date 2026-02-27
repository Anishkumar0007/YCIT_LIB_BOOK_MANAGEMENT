📚 Library Book Management System

A modern, cloud-ready book management application built on the SAP BTP ABAP Environment.
This project leverages the RESTful ABAP Programming Model (RAP) to manage book master data with enterprise-grade audit tracking and domain-controlled value help.

🌟 Project Vision

To design a scalable, cloud-ready library system that ensures:

Structured book classification

Controlled master data via domain values

Full audit traceability

Seamless Fiori integration

RAP-compliant lifecycle management

🏗 Architectural Approach
Domain (Category Control)
        ↓
Data Element
        ↓
Transparent Table (ZCIT_010_BOOK)
        ↓
Interface CDS View
        ↓
Projection View
        ↓
Managed Behavior Definition
        ↓
OData V4 Service Binding
        ↓
Fiori Elements UI

This layered architecture ensures maintainability, extensibility, and cloud readiness.

✨ Functional Highlights
📘 Book Master Data Management

Manage book records including:

Title

Author

Publisher

Genre

Category

Status

🏷 Domain-Driven Category Control

Book categories are controlled through domain fixed values, ensuring:

Data consistency

Built-in value help

Prevented invalid entries

Fiori dropdown integration

📊 Availability Status Tracking

Structured availability indicator:

Code	Meaning
A	Available
B	Borrowed
R	Reserved

Designed for future extensibility (e.g., Lost, Damaged, Archived).

🔍 Enterprise Audit Compliance

Cloud-compliant audit fields included:

CREATED_BY

CREATED_AT

LAST_CHANGED_BY

LAST_CHANGED_AT

LOCAL_LAST_CHANGED_AT

Supports:

ETag handling

Concurrency control

Draft enablement readiness

Managed RAP lifecycle

🛠 Technology Stack
Layer	Technology
Backend	ABAP Cloud (SAP BTP)
Framework	RAP – Managed Scenario
Persistence	SAP HANA
Data Modeling	CDS
Service Layer	OData V4
UI	Fiori Elements (List Report & Object Page)
Development Tool	Eclipse ADT

📁 Repository Structure
/src/zcit_010_book.tabl.xml
/src/zi_cit_010_book.ddls.asddls
/src/zc_cit_010_book.ddls.asddls
/src/zbp_i_cit_010_book.clas.abap
/src/zui_cit_010_book_v4.srvd.srvdsrv

Each layer follows RAP best practices and naming conventions.

⚙ Deployment Guide

1️⃣ Import via abapGit into SAP BTP ABAP Environment
2️⃣ Activate all dictionary objects and CDS artifacts
3️⃣ Publish the Service Binding (ZUI_CIT_010_BOOK_V4)
4️⃣ Launch the Fiori Elements Preview

🎓 Key Learning Outcomes

This project demonstrates proficiency in:

ABAP Dictionary (Domain + Data Element)

Modern Transparent Table Definition

RAP Managed Implementation

Domain-based Value Help Integration

OData V4 Exposure

Cloud-compliant audit modeling

Enterprise data architecture

🚀 Future Roadmap

Borrower Management Entity

Book Issue / Return Transaction Logic

Fine & Penalty Calculation

Draft Enablement

Analytical CDS Reporting

Authorization Controls

KPI Dashboard

👨‍💻 Developer
Anish Kumar T

Built with ❤️ using ABAP Cloud.

📝 License

Licensed under the MIT License.



📸 App Preview


<img width="1867" height="829" alt="Screenshot 2026-02-27 113338" src="https://github.com/user-attachments/assets/3ddfa6cc-248a-4f16-a75e-e3fe559c39f2" />
