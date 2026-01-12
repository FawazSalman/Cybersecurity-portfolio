# Incident Response Analysis = DoS Attack (NIST CSF)

## Project Overview
This project analyzes a **Denial-of-Service (DoS) attack** that impacted a multimedia company’s internal network. The attack caused a two-hour network outage due to a flood of ICMP packets overwhelming network resources.

The goal of this analysis was to evaluate the incident and create a structured security improvement plan using the **National Institute of Standards and Technology Cybersecurity Framework (NIST CSF)**.

This project was completed as part of the **Google Cybersecurity Certificate**, with a focus on real-world incident response and security strategy.

---

## Security Event Summary
The organization experienced a network outage when all internal network services became unresponsive. Investigation revealed that a malicious actor exploited an **unconfigured firewall**, sending a high volume of ICMP packets into the network.

### Key details:
- **Attack type:** Denial-of-Service (ICMP flood)
- **Attack vector:** External network via firewall misconfiguration
- **Impact:** Internal network unavailable for approximately two hours
- **Affected systems:** Internal network services and resources

The incident response team blocked incoming ICMP traffic, shut down non-critical services, and restored critical systems.

---

## Identify (NIST CSF)
The cybersecurity team identified the root cause of the incident as a firewall configuration weakness that allowed unrestricted ICMP traffic.

### Findings:
- No ICMP rate limiting was configured
- Firewall lacked source IP verification
- Entire internal network was affected
- Network monitoring capabilities were limited prior to the incident

---

## Protect (NIST CSF)
To prevent similar incidents, the organization implemented several protective measures.

### Improvements made:
- Firewall rules to **limit ICMP packet rates**
- Source IP verification to detect **spoofed IP addresses**
- Deployment of an **IDS/IPS system**
- Review of firewall configuration standards and procedures

These changes reduce the likelihood of future DoS attacks impacting network availability.

---

## Detect (NIST CSF)
The organization improved its detection capabilities to identify abnormal traffic patterns earlier.

### Detection enhancements:
- Network monitoring software for traffic analysis
- Firewall logging for ICMP activity
- IDS/IPS rules to detect suspicious ICMP traffic
- Alerts for abnormal traffic spikes

These controls help identify attacks faster and reduce response time.

---

## Respond (NIST CSF)
A response plan was developed to handle future cybersecurity incidents more effectively.

### Response actions:
- Isolate affected systems to limit impact
- Block malicious traffic at the firewall
- Prioritize restoration of critical services
- Analyze logs to determine attack patterns
- Report incidents to management and stakeholders

---

## Recover (NIST CSF)
Recovery efforts focused on restoring network services safely and efficiently.

### Recovery steps:
- Restore critical network services first
- Keep non-essential services offline until traffic stabilizes
- Monitor network performance after restoration
- Review and update recovery procedures based on lessons learned

---

## What I Learned
Through this project, I gained practical experience in:
- Analyzing DoS attacks and their impact on networks
- Applying the NIST CSF to real incident scenarios
- Designing detection, response, and recovery strategies
- Understanding how firewall misconfigurations create security risks
- Communicating incident findings clearly and professionally

This project strengthened my understanding of incident response and network security fundamentals.
