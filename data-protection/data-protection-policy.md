## Introduction
This document outlines the data protection measures implemented in the Web-Based Student Registration System to ensure confidentiality, integrity, and availability of user data.

## Scope
Applies to all data processed within the system, including student records, authentication data, and uploaded documents.

## Data Collected
- Personal Information (name, email, matric number, department etc.)
- Authentication Data (hashed passwords)
- Uploaded Documents
- System Logs

## Data Protection Measures
**Authentication & Access Control**
- Role-Based Access Control (RBAC)
- Restricted access for staff vs students
- Total system control for admins

**Password Security**
- Passwords hashed using bcrypt
- No plaintext password storage in DB

**Input Validation**
- All user inputs validated to prevent injection attacks by making use of Nest in-built DTO utility

**Data Storage**
- Sensitive data stored securely in PostgreSQL
- Access limited to authorized roles

**Logging & Monitoring**
- Security events logged using Winston
- Includes login attempts, errors, and access activities

## Logging & Monitoring
- Security events logged using Winston
- Includes login attempts, errors, and access activities

## User Responsibilities
- Maintain strong passwords
- Do not share credentials

## Compliance Alignment
Heavily tailored toward:
- ISO 27001 principles
- Confidentiality, Integrity, Availability (CIA triad)