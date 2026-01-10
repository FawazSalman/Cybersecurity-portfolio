Here is the **updated and clean Markdown version** for your **Project 4** (Portfolio Activity: Apply filters to SQL queries) — written in pure Markdown, ready to copy-paste into your GitHub `project-4-sql-filters/README.md` file.

I've removed all image references and instead left clear **placeholders** where you can easily insert your own terminal screenshots later (just upload your images to an `images/` folder inside the project and replace the placeholder comments with real Markdown image links).

```markdown
# Project 4: Applying SQL Filters for Security Investigations

## Project Overview
As a security professional, I used SQL queries to investigate potential security issues by analyzing login attempts and employee device data.  

This involved filtering large datasets from two tables — `log_in_attempts` and `employees` — to:
- Identify suspicious after-hours login failures
- Examine activity on specific dates
- Detect logins from unusual locations
- Target employee machines for security updates by department and location

Core SQL techniques demonstrated:
- Logical operators: **AND**, **OR**, **NOT**
- Pattern matching: **LIKE** with `%` wildcard
- Filtering by time, date, and categorical values

These skills are valuable for log analysis, threat detection, incident investigation, and asset management in cybersecurity.

## Key SQL Queries & Explanations

### 1. Retrieve After-Hours Failed Login Attempts
**Goal**: Find all failed login attempts that occurred after business hours (after 18:00) for further investigation.

```sql
SELECT *
FROM log_in_attempts
WHERE login_time > '18:00'
  AND success = FALSE;
```

**Explanation**:  
Selected all columns from the `log_in_attempts` table. Used **AND** to combine two conditions:  
- `login_time > '18:00'` → after business hours  
- `success = FALSE` → failed login attempts

<!-- INSERT YOUR SCREENSHOT HERE -->
<!-- Example: ![After-hours failed logins](images/after-hours-failed.png) -->
<!-- Upload your terminal screenshot showing both the query and some output -->

### 2. Retrieve Login Attempts on Specific Dates
**Goal**: Investigate login activity on 2022-05-09 and the day before (2022-05-08).

```sql
SELECT *
FROM log_in_attempts
WHERE login_date = '2022-05-09'
   OR login_date = '2022-05-08';
```

**Explanation**:  
Used **OR** to return records from either of the two specified dates.

<!-- INSERT YOUR SCREENSHOT HERE -->
<!-- Example: ![Specific dates logins](images/specific-dates.png) -->

### 3. Retrieve Login Attempts Outside of Mexico
**Goal**: Identify potentially suspicious login attempts not originating from Mexico (handles both 'MEX' and 'MEXICO').

```sql
SELECT *
FROM log_in_attempts
WHERE country NOT LIKE 'MEX%';
```

**Explanation**:  
Used **NOT** combined with **LIKE** and the `%` wildcard to exclude any country value starting with 'MEX'.

<!-- INSERT YOUR SCREENSHOT HERE -->
<!-- Example: ![Logins outside Mexico](images/outside-mexico.png) -->

### 4. Retrieve Employees in Marketing (East Building)
**Goal**: Get list of employee machines in the Marketing department located in the East building for targeted updates.

```sql
SELECT *
FROM employees
WHERE department = 'Marketing'
  AND office LIKE 'East%';
```

**Explanation**:  
**AND** combines exact department match with pattern matching for office location.

<!-- INSERT YOUR SCREENSHOT HERE -->
<!-- Example: ![Marketing East building](images/marketing-east.png) -->

### 5. Retrieve Employees in Finance or Sales
**Goal**: Identify employees in Finance or Sales departments (different update required).

```sql
SELECT *
FROM employees
WHERE department = 'Finance'
   OR department = 'Sales';
```

**Explanation**:  
**OR** captures employees from either department.

<!-- INSERT YOUR SCREENSHOT HERE -->
<!-- Example: ![Finance or Sales](images/finance-sales.png) -->

### 6. Retrieve All Employees Not in IT
**Goal**: Target employees outside the Information Technology department for security updates.

```sql
SELECT *
FROM employees
WHERE department NOT LIKE 'Information Technology';
```

**Explanation**:  
**NOT** excludes the IT department.

<!-- INSERT YOUR SCREENSHOT HERE -->
<!-- Example: ![Not in IT](images/not-in-it.png) -->

## Summary & Skills Demonstrated
I used SQL filters to extract actionable security insights from login and employee data. This included identifying suspicious patterns, investigating specific events, and preparing targeted device updates.

**Key skills gained**:
- Writing precise, efficient SQL queries for security use cases
- Combining multiple conditions with AND/OR/NOT
- Using LIKE and wildcards for flexible pattern matching
- Translating business/security needs into database queries

These abilities are directly applicable to SIEM log analysis, threat hunting, and managing security posture in real-world environments.
