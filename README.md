# Salesforce_Project_Amrutha
Phase 1: Problem Understanding & Industry Analysis
Project Title: Smart Healthcare CRM – Patient Engagement & Appointment System
1. Introduction
Hospitals and clinics face challenges in managing patient appointments, follow-ups, and medical history. Manual processes often result in missed appointments, poor patient engagement, and inefficiency in operations.

This project aims to build a Salesforce-based Healthcare CRM that streamlines patient registration, appointment scheduling, doctor availability, prescription tracking, and automated reminders.
2. Problem Statement
The current system of appointment management and patient engagement is manual and fragmented. Key issues include:
- Manual appointment bookings leading to errors and double bookings.
- No centralized system for patient medical history.
- Poor follow-up on prescriptions and lab reports.
- Doctors lack a clear daily schedule view.
- Management struggles with patient visit trends and doctor workload tracking.
3. Requirement Gathering
Key Questions Addressed:
- How should patient records be stored (allergies, medical history, prescriptions)?
- What is the preferred channel for reminders (SMS, Email)?
- Should appointments require approval for specialist consultations?
- How should prescriptions and reports be attached to patient records?
- What performance metrics should management track?
Sample User Stories:
• “As a patient, I want to receive SMS reminders for my appointment so I don’t miss it.”
• “As a doctor, I want to see my daily schedule and patient details in one place.”
• “As a receptionist, I want to quickly book appointments and assign doctors based on availability.”
• “As an admin, I want dashboards that show patient visits, missed appointments, and doctor utilization.”
4. Stakeholder Analysis
Stakeholder
Role in System
Needs
Doctors
Service Providers
Access patient records, view schedule, update visit notes, prescribe medications
Receptionists
Front Desk Ops
Register patients, schedule appointments, manage doctor availability
Patients
End Customers
Book/cancel appointments, receive reminders, access prescriptions/reports
Hospital Admin
Management
Monitor doctor workload, revenue reports, patient inflow analysis
Lab Technicians
Support Staff
Upload test reports linked to patients

5. Business Process Mapping
Appointment Booking Process:
1. Receptionist enters patient details → Patient record created (Custom Object: Patient__c).
2. Appointment created and assigned to a doctor (Custom Object: Appointment__c).
3. System sends confirmation via Email/SMS.
4. Appointment visible on doctor’s Salesforce calendar.
5. After consultation → Prescription uploaded & Follow-up Task auto-created (Apex Trigger).

Lab Reports Process:
1. Doctor orders lab test → Request logged in system.
2. Lab uploads report and attaches it to patient record.
3. Notification sent to patient.
6. Industry-Specific Use Case Analysis
- Compliance: Ensure secure storage of medical data (HIPAA/GDPR best practices).
- Data Modeling:
   • Patient ↔ Appointment (One-to-Many)
   • Appointment ↔ Doctor (Lookup)
   • Patient ↔ Prescription/Lab Reports (One-to-Many)
- Automation Needs:
   • Appointment reminders via Flow.
   • Follow-up task creation via Apex Trigger.
   • Specialist referral approvals via Approval Process.
- Dashboards:
   • Doctor Utilization (appointments/day).
   • Patient Visits Trend (monthly).
   • Missed vs Attended Appointments.
7. AppExchange Exploration
Recommended Apps:
- Twilio / 360 SMS App → Automated SMS reminders.
- Calendar Management Apps → Enhanced doctor availability calendar.
- Document Management Apps → Secure prescription & report storage.
- Health Cloud (optional) → Advanced healthcare features (if budget allows).
8. Deliverables of Phase 1
1. Business Requirement Document (BRD) – Problems, requirements, user stories.
2. Stakeholder Matrix – Users and their roles.
3. Business Process Maps – Appointment, Prescription, and Lab workflows.
4. Entity-Relationship Diagram (ERD) – Patients, Doctors, Appointments, Reports.
5. Gap Analysis Report – Manual process vs Salesforce solution.
6. AppExchange Research Report – Suggested integrations (SMS, calendar, reports).

