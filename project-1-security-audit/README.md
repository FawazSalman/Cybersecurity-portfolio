# Conduct a Security Audit

## Project Overview
This portfolio activity is from the Google Cybersecurity Professional Certificate, specifically the course "Play It Safe: Manage Security Risks." The task involved conducting an internal security audit for a fictional company, Botium Toys, to assess their security posture, identify gaps in controls, and ensure compliance with standards like PCI DSS, GDPR, and SOC. Audits like this are crucial for monitoring threats, risks, and vulnerabilities that could impact business continuity and critical assets.

The scenario describes Botium Toys as a small U.S.-based toy developer with a growing online presence. The IT manager initiates an audit using the NIST Cybersecurity Framework (CSF) to evaluate assets, risks, and compliance, focusing on securing infrastructure, mitigating threats, and adhering to regulations for payment processing and E.U. business.

## Objectives
- Review the provided scope, goals, and risk assessment report.
- Evaluate controls across administrative, technical, and physical categories.
- Complete a controls and compliance checklist to identify implementation gaps.
- Provide recommendations to improve security and reduce risks.

## Approach
1. **Reviewed Supporting Materials**:
   - Botium Toys: Scope, goals, and risk assessment report – This outlined the audit scope (entire security program), goals (assess assets and controls), current assets (e.g., on-premises equipment, employee devices, networks, data storage), and risk assessment (inadequate asset management, lack of controls, high risk score of 8/10).
   - Control Categories – This document categorized controls into administrative/managerial, technical, and physical/operational, with types like preventative, corrective, detective, and deterrent. It provided examples and purposes for each.
   
2. **Conducted the Audit**:
   - Analyzed the risk assessment's "Additional comments" for specific issues (e.g., universal employee access to data, no encryption for credit cards, missing IDS, no disaster recovery plans).
   - Filled out the Controls and Compliance Checklist by marking "Yes" or "No" for each control/best practice, with explanations based on the report.
   - Focused on NIST CSF's "Identify" function to classify assets and assess impacts.

3. **Tools and Resources Used**:
   - Google Docs/Word for reviewing and completing the checklist (based on provided templates).
   - NIST CSF guidelines for structuring the audit.
   - No specialized software; this was a document-based analysis emphasizing analytical skills.

## Key Findings
The audit revealed significant gaps in Botium Toys' security controls and compliance. Below are the completed checklists reproduced as tables for clarity.

### Controls Assessment Checklist

| Yes | No | Control | Explanation |
|-----|----|---------|-------------|
|     | X  | Least Privilege | Currently, all employees have access to customer data; privileges need to be limited to reduce the risk of a breach. |
|     | X  | Disaster recovery plans | There are no disaster recovery plans in place. These need to be implemented to ensure business continuity. |
|     | X  | Password policies | Employee password requirements are minimal, which could allow a threat actor to more easily access secure data/other assets via employee work equipment/the internal network. |
|     | X  | Separation of duties | Needs to be implemented to reduce the possibility of fraud/access to critical data, since the company CEO currently runs day-to-day operations and manages the payroll. |
| X   |    | Firewall | The existing firewall blocks traffic based on an appropriately defined set of security rules. |
|     | X  | Intrusion detection system (IDS) | The IT department needs an IDS in place to help identify possible intrusions by threat actors. |
|     | X  | Backups | The IT department needs to have backups of critical data, in the case of a breach, to ensure business continuity. |
| X   |    | Antivirus software | Antivirus software is installed and monitored regularly by the IT department. |
|     | X  | Manual monitoring, maintenance, and intervention for legacy systems | The list of assets notes the use of legacy systems. The risk assessment indicates that these systems are monitored and maintained, but there is not a regular schedule in place for this task and procedures/policies related to intervention are unclear, which could place these systems at risk of a breach. |
|     | X  | Encryption | Encryption is not currently used; implementing it would provide greater confidentiality of sensitive information. |
|     | X  | Password management system | There is no password management system currently in place; implementing this control would improve IT department/other employee productivity in the case of password issues. |
| X   |    | Locks (offices, storefront, warehouse) | The store’s physical location, which includes the company’s main offices, store front, and warehouse of products, has sufficient locks. |
| X   |    | Closed-circuit television (CCTV) surveillance | CCTV is installed/functioning at the store’s physical location. |
| X   |    | Fire detection/prevention (fire alarm, sprinkler system, etc.) | Botium Toys’ physical location has a functioning fire detection and prevention system. |

### Compliance Checklist

#### Payment Card Industry Data Security Standard (PCI DSS)

| Yes | No | Best Practice | Explanation |
|-----|----|---------------|-------------|
|     | X  | Only authorized users have access to customers’ credit card information. | Currently, all employees have access to the company’s internal data. |
|     | X  | Credit card information is accepted, processed, transmitted, and stored internally, in a secure environment. | Credit card information is not encrypted and all employees currently have access to internal data, including customers’ credit card information. |
|     | X  | Implement data encryption procedures to better secure credit card transaction touchpoints and data. | The company does not currently use encryption to better ensure the confidentiality of customers’ financial information. |
|     | X  | Adopt secure password management policies. | Password policies are nominal and no password management system is currently in place. |

#### General Data Protection Regulation (GDPR)

| Yes | No | Best Practice | Explanation |
|-----|----|---------------|-------------|
|     | X  | E.U. customers’ data is kept private/secured. | The company does not currently use encryption to better ensure the confidentiality of customers’ financial information. |
| X   |    | There is a plan in place to notify E.U. customers within 72 hours if their data is compromised/there is a breach. | There is a plan to notify E.U. customers within 72 hours of a data breach. |
|     | X  | Ensure data is properly classified and inventoried. | Current assets have been inventoried/listed, but not classified. |
| X   |    | Enforce privacy policies, procedures, and processes to properly document and maintain data. | Privacy policies, procedures, and processes have been developed and enforced among IT team members and other employees, as needed. |

#### System and Organizations Controls (SOC type 1, SOC type 2)

| Yes | No | Best Practice | Explanation |
|-----|----|---------------|-------------|
|     | X  | User access policies are established. | Controls of Least Privilege and separation of duties are not currently in place; all employees have access to internally stored data. |
|     | X  | Sensitive data (PII/SPII) is confidential/private. | Encryption is not currently used to better ensure the confidentiality of PII/SPII. |
| X   |    | Data integrity ensures the data is consistent, complete, accurate, and has been validated. | Data integrity is in place. |
|     | X  | Data is available to individuals authorized to access it. | While data is available to all employees, authorization needs to be limited to only the individuals who need access to it to do their jobs. |

## Recommendations
To strengthen Botium Toys' security posture:
- Implement Least Privilege and Separation of Duties to limit access and reduce insider threats.
- Develop disaster recovery plans and regular backups for business continuity.
- Enhance password policies and deploy a password management system.
- Install an IDS for better threat detection.
- Apply encryption for sensitive data (e.g., credit cards, PII).
- Schedule regular maintenance for legacy systems and classify all assets.
- These changes will address compliance gaps in PCI DSS, GDPR, and SOC, potentially reducing the risk score from 8/10 and avoiding fines.

## Skills Gained and Learnings
- **Skills**: Risk assessment, controls evaluation (administrative, technical, physical), compliance auditing (PCI DSS, GDPR, SOC), NIST CSF application.
- **Learnings**: Understood the importance of layered defenses (defense in depth) and how incomplete controls lead to high risks. Gained experience in analyzing reports to identify vulnerabilities and recommend prioritized fixes. This activity highlighted the balance between security and business operations in a growing company.
- **Challenges Overcome**: As a beginner, interpreting control categories and mapping them to the scenario was tricky, but cross-referencing documents helped build confidence in audit processes.

## Notes on GitHub Implementation
To add this to your GitHub repo professionally:
- Create a subfolder named `project-1-security-audit` in your main repository.
- Add this content as `README.md` inside that folder (copy-paste the Markdown above).
- No screenshots are needed here— the activity is text-based (reports and checklists), and rendering tables in Markdown keeps it clean, accessible, and professional. Screenshots could make it look cluttered or less searchable; recruiters prefer readable text.
- If you want to include originals, upload the attached .docx files to an `assets/` subfolder within the project folder, and link them in the README (e.g., `[Download Original Checklist](assets/Controls-and-compliance-checklist-exemplar.docx)`). This adds authenticity without overwhelming the page.
- Update your main repo README to link here: `- [Project 1: Conduct a Security Audit](./project-1-security-audit/README.md) (Course: Play It Safe: Manage Security Risks)`.

This format showcases your work effectively—concise, structured, and focused on outcomes. Great job on completing this; it demonstrates strong foundational cybersecurity skills! If you share more activities, I can template those too.
