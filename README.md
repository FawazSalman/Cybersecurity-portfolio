# Fawaz Salman | Cybersecurity Portfolio

## 👋 About Me

I'm a third-year Bachelor of Engineering student in ICT – Robotics at Häme University of Applied Sciences (HAMK), Finland, with a growing focus on defensive cybersecurity.

My cybersecurity journey began with the Google Cybersecurity Professional Certificate, where I developed a foundation in security operations, incident response, risk assessment, Linux security, and network defense. Since then, I've expanded into independent projects involving Python-based security automation, threat detection, log analysis, and AI-assisted security investigations.

I'm particularly interested in understanding how security incidents are detected, investigated, and prevented, as well as how organizations manage access to critical systems and sensitive information.

This portfolio brings together my independent cybersecurity projects, hands-on technical work, and foundational security assessments, documenting both what I've built and how I approach security problems.

---

## 🎯 Career Objective

I'm seeking a **Summer 2027 cybersecurity internship**, particularly in:

- Security Operations Center (SOC) and Security Analysis
- Identity & Access Management (IAM)
- Cybersecurity Operations and Incident Response
- Vulnerability Management and Security Risk Assessment
- Other entry-level defensive cybersecurity roles

My goal is to contribute to a security team while developing practical experience with enterprise security tools, detection and investigation workflows, access management, and risk reduction.

I'm open to opportunities where I can combine technical problem-solving, analytical thinking, and continuous learning.

---

## 🛠️ Technical Skills

### Security Operations & Threat Detection
- Security log analysis and authentication event investigation
- Rule-based threat detection and alert correlation
- Brute-force and password-spraying detection
- Incident response fundamentals and investigation documentation
- MITRE ATT&CK mapping and NIST Cybersecurity Framework (CSF)
- SIEM fundamentals: Splunk and Google Chronicle (introductory)

### Identity, Access & System Security
- Identity and access management (IAM) fundamentals
- Least privilege, role-based access control (RBAC), and access reviews
- Linux file permissions and system authorization
- Access control automation using Python
- Authentication security and account-related threat analysis

### Risk Assessment & Security Governance
- Security audits and control gap assessments
- Vulnerability assessment and qualitative risk scoring
- NIST SP 800-30 risk assessment methodology
- PCI DSS and GDPR compliance fundamentals
- Security remediation planning and documentation

### Programming, Automation & AI
- Python for security automation, log processing, and analysis
- SQL for security investigations and data filtering
- AI/LLM integration for security investigation assistance
- Evidence-grounded AI reporting and reliability evaluation
- Automated testing and Git/GitHub version control

### Systems, Networking & Tools
- Linux and Windows fundamentals
- TCP/IP, DNS, HTTP/HTTPS, and network security fundamentals
- Wireshark for packet inspection
- Streamlit for interactive security dashboards
- OpenRouter API and LLM-assisted analysis

---

## 📂 Cybersecurity Projects

My portfolio includes independent security engineering projects and practical cybersecurity assessments completed during the Google Cybersecurity Professional Certificate.

### 🚀 Independent Cybersecurity Projects

These projects focus on building security tools, applying defensive techniques, and testing security analysis workflows.

#### 1. [SentinelAI — AI-Augmented SOC](https://github.com/FawazSalman/SentinelAI-AI-Augmented-SOC)

**Python | SOC | Log Analysis | Threat Detection | MITRE ATT&CK | Streamlit | AI**

Developed an AI-augmented SOC prototype combining rule-based authentication threat detection, log correlation, and LLM-assisted security investigation reporting.

- Processed 10,000 OpenSSH log lines, extracting 2,755 structured authentication events.
- Implemented detection logic for brute-force attacks, password spraying, and suspicious authentication activity.
- Achieved 100% precision and recall across 10 labeled synthetic evaluation scenarios.
- Built an interactive Streamlit dashboard for alert investigation, evidence inspection, and AI-assisted reporting.
- Passed 22 automated tests and evaluated LLM-generated reports for evidence-grounding and unsupported findings.

**[View Project Repository](https://github.com/FawazSalman/SentinelAI-AI-Augmented-SOC)**

#### 2. [PhishLens AI — Explainable Phishing Detection & Email Investigation](https://github.com/FawazSalman/PhishLens-AI)

**Python | Machine Learning | Email Security | TF-IDF | Logistic Regression | LLM | Threat Analysis**

Developed a local phishing investigation application combining machine learning, rule-based security indicators, and optional LLM-assisted evidence analysis.

- Built a phishing classifier using TF-IDF and logistic regression, achieving **99.47% F1 on 8,103 held-out samples** and **66.64% F1 on 5,684 external samples**, identifying limitations in cross-dataset generalization.
- Implemented email header, URL, attachment metadata, and MIME analysis to identify suspicious indicators without executing potentially malicious content.
- Integrated optional local LLM-assisted evidence prioritization, keeping detection scores independent of AI-generated output.
- Developed a local investigation dashboard supporting `.eml` analysis, explainable detection results, SHA-256 evidence hashes, and JSON/text report exports.
- Validated functionality through automated tests and evaluated detection behavior using 12 synthetic AI-generated challenge emails.

**[View Project Repository](https://github.com/FawazSalman/PhishLens-AI)**

### 🔐 Google Cybersecurity Certificate Projects

The following projects demonstrate foundational security skills through simulated business scenarios, technical exercises, and documented security assessments.

#### 3. [Internal Security Audit & Risk Assessment](./project-1-security-audit/README.md)

**NIST CSF | Security Auditing | GRC | PCI DSS | GDPR**

Conducted a simulated internal security audit of an e-commerce business, identifying control deficiencies, compliance gaps, and a high overall risk rating of 8/10. Evaluated access controls, encryption, disaster recovery, and security monitoring, proposing risk-based remediation measures.

#### 4. [Incident Response Analysis — DoS Attack](./project-2-nist-incident-response/README.md)

**NIST CSF | Incident Response | Network Security | IDS/IPS**

Analyzed a simulated ICMP flood attack that caused approximately two hours of network downtime. Identified firewall configuration weaknesses and developed detection, mitigation, response, and recovery recommendations using the NIST CSF.

#### 5. [Security Investigation Using SQL Filters](./project-3-sql-filters/README.md)

**SQL | Security Investigation | Database Queries**

Used SQL queries with `AND`, `OR`, `NOT`, and `LIKE` operators to investigate suspicious login activity, filter security records, and identify employee machines requiring attention.

#### 6. [Managing File Permissions in Linux](./project-4-linux-file-permissions/README.md)

**Linux | chmod | Access Control | Least Privilege**

Audited Linux file and directory permissions using `ls -la` and applied targeted `chmod` commands to remove unauthorized write access, secure archived files, and restrict directory access. Verified the resulting permissions through terminal inspection.

#### 7. [Vulnerability Assessment & Risk Analysis](./project-5-vulnerability-assessment/README.md)

**NIST SP 800-30 | Risk Assessment | Vulnerability Management**

Assessed security risks associated with a publicly accessible database server, evaluating three threat scenarios with risk scores of 9, 6, and 3. Recommended RBAC, MFA, TLS encryption, IP allow-listing, and defense-in-depth controls.

#### 8. [Python Automation for Access Control](./project-6-python-allow-list-update/README.md)

**Python | Security Automation | Access Management**

Developed a Python algorithm to automate IP allow-list maintenance, removing unauthorized addresses from approved access records to support consistent access control enforcement.

---

## 📜 Certifications & Learning

- **Google Cybersecurity Professional Certificate**
- **CCNA: Introduction to Networks** — HAMK / Cisco
- **Wireshark for Beginners: Capture Packets**

---

## 📫 Connect With Me

- **LinkedIn:** [linkedin.com/in/fawaz-salman](https://www.linkedin.com/in/fawaz-salman)
- **Email:** [fawazsalman25@gmail.com](mailto:fawazsalman25@gmail.com)

I'm interested in connecting with cybersecurity professionals, learning from security teams, and exploring Summer 2027 internship opportunities.

Thank you for visiting my portfolio!
