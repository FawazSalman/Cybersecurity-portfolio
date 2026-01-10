# Project 3: SQL Filtering for Security Investigations

## Project Overview
As part of investigating potential security incidents and preparing for device updates, I queried two main tables:  
- `log_in_attempts` — to analyze suspicious login behavior  
- `employees` — to identify machines needing security patches  

I used SQL filters (AND, OR, NOT, LIKE with wildcards) to extract only the relevant records quickly and accurately.

All examples below show real terminal executions — query + result — captured from the lab environment.

## Investigated Security Scenarios

### 1. After-Hours Failed Login Attempts
**Goal**: Identify failed login attempts that happened after business hours (> 18:00) for incident review.

![After-hours failed login attempts](images/after-hours-failed-logins.png)

**Brief explanation**:  
Filtered login attempts by time of day (> 18:00) and success status (failed only). This helps detect possible off-hours brute-force or credential-stuffing attempts.

### 2. Login Attempts on Suspicious Dates
**Goal**: Check all login activity on 2022-05-09 and the previous day (2022-05-08).

<!-- INSERT YOUR SCREENSHOT HERE -->
![Login attempts on specific dates](images/specific-dates-logins.png)

**Brief explanation**:  
Targeted logins on and around a known suspicious date to look for unusual patterns or volume.

### 3. Login Attempts Outside of Mexico
**Goal**: Find login attempts coming from locations other than Mexico.

<!-- INSERT YOUR SCREENSHOT HERE -->
![Logins outside Mexico](images/logins-outside-mexico.png)

**Brief explanation**:  
Used pattern matching to exclude Mexico (covering both 'MEX' and 'MEXICO' values). Useful for spotting potentially unauthorized geographic access.

### 4. Employees in Marketing – East Building
**Goal**: List employee devices in the Marketing department located in the East building for targeted patching.

<!-- INSERT YOUR SCREENSHOT HERE -->
![Marketing department - East building](images/marketing-east-building.png)

**Brief explanation**:  
Combined exact department filter with location pattern matching to narrow down the list of machines.

### 5. Employees in Finance or Sales
**Goal**: Identify devices in Finance and Sales departments (different update needed).

<!-- INSERT YOUR SCREENSHOT HERE -->
![Finance or Sales departments](images/finance-or-sales.png)

**Brief explanation**:  
Captured employees from either department to support department-specific security actions.

### 6. All Employees Not in IT
**Goal**: Find all employee machines except those in IT (already patched).

<!-- INSERT YOUR SCREENSHOT HERE -->
![Employees not in IT](images/not-in-it.png)

**Brief explanation**:  
Excluded the IT department to focus patching efforts on the rest of the organization.

## Summary
Through these targeted queries I was able to:
- Quickly surface suspicious login patterns for investigation
- Efficiently identify groups of employee devices needing security updates

**Main skills demonstrated**:
- Practical application of SQL filtering in security contexts
- Using logical operators (AND/OR/NOT) and pattern matching (LIKE)
- Reading and interpreting real database output in terminal

These techniques are directly useful in SOC analyst, threat hunting, and log analysis roles.

Questions / feedback welcome!
