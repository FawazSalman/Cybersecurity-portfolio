# Project 3: Applying Filters to SQL Queries for Security Investigations

## Project Overview
As a security professional investigating potential threats and ensuring system integrity, I used SQL to query large datasets from **log_in_attempts** and **employees** tables.  

This involved filtering records to identify suspicious login activity (e.g., after-hours failures, specific dates, non-local attempts) and to target employee devices for security updates (e.g., by department or location).  

Key techniques demonstrated:
- Filtering with **AND**, **OR**, **NOT**
- Pattern matching with **LIKE** and wildcards (`%`)
- Handling time/date and categorical data

These skills are essential for log analysis, incident response, threat detection, and asset management in cybersecurity roles.

## Key SQL Queries & Explanations

### 1. Retrieve After-Hours Failed Login Attempts
Goal: Identify failed login attempts after business hours (> 18:00) for investigation.

```sql
SELECT *
FROM log_in_attempts
WHERE login_time > '18:00'
  AND success = FALSE;
