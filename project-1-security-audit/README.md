# Internal Security Audit - Botium Toys

## Project Overview
This project focuses on conducting an internal security audit for a fictional company called **Botium Toys**, a small U.S.-based business selling toys both in-store and online. As the company grows internationally, especially in the E.U. market, its IT infrastructure faces increased security and compliance risks.

The goal of this audit was to review the company’s current security posture, identify gaps in controls and compliance, and recommend improvements using the **NIST Cybersecurity Framework (CSF)**.

This activity was completed as part of the **Google Cybersecurity Certificate**, with an emphasis on practical, real-world security auditing.

---

## Audit Scope and Goals

**Scope:**  
The audit covered Botium Toys’ entire security program, including:
- IT-managed assets
- Internal systems and networks
- Security controls
- Compliance with regulations such as PCI DSS and GDPR

**Goals:**
- Identify missing or weak security controls  
- Assess compliance risks  
- Reduce the likelihood of data breaches and regulatory fines  
- Improve overall security posture

---

## Assets Reviewed
Some of the key assets assessed during the audit included:
- Employee devices (laptops, desktops, smartphones)
- Internal network and internet access
- Databases storing customer and payment data
- E-commerce and inventory systems
- Legacy systems requiring manual monitoring
- Physical location (office, storefront, warehouse)

---

## Key Findings (Risk Assessment Summary)

The overall risk level was rated **high (8/10)** due to multiple gaps in security controls and compliance practices.

### Major issues identified:
- All employees had access to sensitive customer and payment data
- No encryption was used for stored or processed credit card information
- No disaster recovery plans or data backups were in place
- Weak password policies and no password management system
- No intrusion detection system (IDS)
- Legacy systems were monitored inconsistently
- Compliance risks related to **PCI DSS**, **GDPR**, and **SOC controls**

Some positive findings included:
- Firewall rules were properly configured
- Antivirus software was installed and monitored
- Physical security (locks, CCTV, fire systems) was in place
- GDPR breach notification procedures existed

---

## Controls Assessment

I evaluated administrative, technical, and physical controls to determine whether they were currently implemented.

### Missing or Weak Controls:
- Least Privilege
- Separation of Duties
- Strong Password Policies
- Disaster Recovery Plans
- Data Backups
- Encryption
- Intrusion Detection System (IDS)
- Centralized Password Management
- Formal legacy system maintenance schedule

### Existing Controls:
- Firewall
- Antivirus software
- Physical locks
- CCTV surveillance
- Fire detection and prevention systems

---

## Compliance Assessment

### PCI DSS (Payment Card Industry Data Security Standard)
- ❌ Unauthorized access to cardholder data
- ❌ No encryption for payment data
- ❌ Weak password practices

### GDPR (General Data Protection Regulation)
- ❌ Customer data not fully secured
- ✅ 72-hour breach notification plan in place
- ❌ Assets not properly classified

### SOC Controls
- ❌ User access policies not enforced
- ❌ Sensitive data not confidential
- ✅ Data integrity maintained
- ❌ Data availability not restricted to authorized users

---

## Recommendations

To reduce risk and improve compliance, the following actions are recommended:
- Implement **Least Privilege** and **Separation of Duties**
- Encrypt all sensitive customer and payment data
- Deploy an **Intrusion Detection System (IDS)**
- Establish **disaster recovery plans** and regular **data backups**
- Enforce stronger password policies with a **password management system**
- Classify and inventory assets properly
- Create a structured maintenance schedule for legacy systems

---

## What I Learned

Through this project, I learned how to:
- Conduct a structured internal security audit
- Identify security risks using the NIST CSF
- Map security controls to real-world vulnerabilities
- Understand compliance requirements like PCI DSS and GDPR
- Communicate security findings clearly and simply

This project helped strengthen my understanding of how cybersecurity principles are applied in real business environments.
