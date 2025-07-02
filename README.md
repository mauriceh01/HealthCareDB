# HealthCareDB

## Overview

**HealthCareDB** is a comprehensive relational database schema designed for managing healthcare data and powering a Healthcare Insights Dashboard. It models a wide range of healthcare-related entities including patients, providers, appointments, diagnoses, procedures, billing, care management, telehealth, prescriptions, notifications, and community health metrics.

This database supports detailed clinical, administrative, and operational workflows and is intended as a backend for healthcare analytics, reporting, and care coordination systems.

---

## Features

- **Core Healthcare Entities:** Patients, Providers, Departments, Appointments, Diagnoses, Procedures, Lab Results, Visits, Insurance, Billing, and Vitals.
- **Care Management:** Care plans, chronic conditions, social determinants of health, and referrals.
- **Provider Management:** Provider schedules and telehealth/virtual visit tracking.
- **Pharmacy & Prescriptions:** Pharmacies, prescriptions, and prescription fill tracking.
- **User & Security:** User authentication, roles, audit logs, and access permissions.
- **Communication:** Notifications, chat messages, and system alerts.
- **Dashboard Customization:** User-specific dashboard widgets and filters.
- **Community Health:** Geolocation data, outbreak alerts, and zip code health statistics.

---

## Technologies Used

- **Database Engine:** MySQL 8.x (compatible with MariaDB and other RDBMS)
- **SQL Language:** ANSI SQL (DDL & DML)
- **Backend Integration:** Designed to be compatible with Python (Flask, Django), Node.js, .NET, or Java backend systems.
- **Analytics & BI Tools:** Optimized for Power BI, Tableau, or custom web-based dashboards
- **Security Model:** Role-Based Access Control (RBAC), Audit Logging, and Tokenized Password Reset
- **Data Types:** ENUMs, DATE/DATETIME, TEXT, DECIMAL for precision tracking
- **Constraints:** Foreign Keys, Primary Keys, AUTO_INCREMENT for data integrity
- **Data Compliance Ready:**
---
## Database Schema Highlights

- **Departments & Providers:** Departments are linked to Providers, with a designated Head of Department.
- **Patients:** Include demographic, contact, and primary physician linkage.
- **Appointments:** Schedule and track patient visits with providers.
- **Clinical Data:** Diagnoses, procedures, medications, lab results, and vital signs.
- **Care Coordination:** Care plans, referrals, and chronic condition management.
- **Billing & Insurance:** Track charges, payments, and insurance coverage.
- **User Management:** Roles such as Admin, Doctor, Nurse, Staff, and Patient.
- **Security:** Audit logs, login tracking, password reset tokens.
- **Community Health:** Geographic data and outbreak monitoring.

---

## Tables Overview

| Table Name            | Purpose                                                         |
|-----------------------|-----------------------------------------------------------------|
| Departments           | Hospital or clinic departments and their heads                  |
| Providers             | Healthcare providers with specialty and contact details         |
| Patients              | Patient demographics and contact info                           |
| Appointments          | Scheduled and completed patient visits                          |
| Diagnoses             | Patient diagnoses with ICD-10 codes                             |
| Medications           | Medication prescriptions and details                            |
| Procedures            | Medical procedures with CPT codes and outcomes                  |
| LabResults            | Laboratory test results with status indicators                  |
| Visits                | Patient visits (inpatient, outpatient, ER)                      |
| Insurance             | Patient insurance details                                       |
| Billing               | Charges, payments, and billing status                           |
| Vitals                | Patient vital signs records                                     |
| Readmissions          | Tracking patient readmissions                                   |
| SatisfactionSurveys   | Patient feedback surveys                                        |
| KPIMetrics            | Key performance indicators by department                        |
| Alerts                | Patient alerts for clinical events                              |
| UserLogins            | User authentication and role management                         |
| UserRolesMapping      | Mapping between users and their roles (Patient, Provider)      |
| AuditLog              | System audit trail of user actions                              |
| CarePlans             | Individualized care plans for patients                          |
| ChronicConditions     | Chronic disease tracking                                       |
| SocialDeterminants    | Social factors affecting health                                 |
| Referrals             | Patient referrals between providers                             |
| ProviderSchedules     | Providers' working schedules                                   |
| TelehealthVisits      | Virtual visit tracking                                         |
| Pharmacies            | Pharmacy contact info                                          |
| Prescriptions         | Medication prescriptions                                      |
| PrescriptionFills     | Tracking prescription fills                                   |
| Notifications         | System notifications for users                               |
| ChatMessages          | Internal user communication                                  |
| DashboardWidgets      | User-configurable dashboard widgets                           |
| DashboardFilters      | Saved dashboard filter settings                              |
| AccessPermissions     | Role-based access control                                    |
| PasswordResetTokens   | Password reset management                                    |
| Geolocation           | Patient geographic information                               |
| OutbreakAlerts        | Community health outbreak tracking                          |
| ZipCodeStats          | Demographic and health statistics by ZIP code              |

---

## 📌 Author
Created by: Maurice Hazan on July 1, 2025

📧 [mauriceh01@hotmail.com](mailto:mauriceh01@hotmail.com)     

🌉 [LinkedIn](https://linkedin.com/in/mohazan)     

🔗 [GitHub](https://github.com/mauriceh01)       


## Installation

1. Ensure you have MySQL (or compatible RDBMS) installed.
2. Create the database and schema by running the provided SQL script:
   ```sql
   CREATE DATABASE HealthCareDB;
   USE HealthCareDB;
   -- Run all CREATE TABLE statements as provided
