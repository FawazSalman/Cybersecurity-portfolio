# Project 2: Use the NIST Cybersecurity Framework to Respond to a Security Incident

## Project Overview
This portfolio activity is from the Google Cybersecurity Professional Certificate, Course: **Connect and Protect: Networks and Network Security**.  

The task was to analyze a real-world Denial of Service (DoS) incident — specifically an **ICMP flood attack** — and create an incident report using the **NIST Cybersecurity Framework (CSF)**. The NIST CSF's five core functions (Identify, Protect, Detect, Respond, Recover) guide organizations in managing cybersecurity risks proactively and reactively.

Here are the 5 core functions of the NIST CSF visualized:

<grok-card data-id="200596" data-type="image_card"  data-arg-size="LARGE" ></grok-card>



<grok-card data-id="8a222e" data-type="image_card"  data-arg-size="LARGE" ></grok-card>


## Scenario Summary
A multimedia company offering web/graphic design and social media services experienced a **DoS attack** via an **ICMP flood** (ping flood) through an unconfigured firewall.  

This overwhelmed the network with excessive ICMP packets, causing all internal network services to become unresponsive for two hours. Normal traffic could not reach critical resources.  

The incident team responded by blocking incoming ICMP, taking non-critical services offline, and restoring critical ones.  

Post-incident, the team implemented:
- Rate-limiting for incoming ICMP packets
- Source IP verification to detect spoofing
- Network monitoring software for abnormal patterns
- IDS/IPS to filter suspicious ICMP traffic

The attack type: **ICMP flood DoS** (a classic volumetric attack that floods the target with ping requests to exhaust bandwidth/resources).  

Visual example of an ICMP flood / ping flood attack:

<grok-card data-id="f32a90" data-type="image_card"  data-arg-size="LARGE" ></grok-card>


## Incident Report Using NIST CSF

### Identify
The incident involved a malicious actor exploiting an unconfigured firewall to send a massive flood of ICMP packets, targeting the entire internal network.  
Affected systems: Firewall, all network resources (servers, internal services, employee access).  
Impact: Complete denial of service for 2 hours, disrupting business operations.  
Key gaps identified: Lack of ICMP rate-limiting, no source IP verification, insufficient traffic monitoring.

### Protect
To prevent recurrence and strengthen defenses:
- Implement strict firewall rules to limit ICMP packet rates from external sources.
- Enable source IP address verification to block spoofed packets.
- Deploy protective technologies like an Intrusion Prevention System (IPS).
- Update access controls and firewall configurations.
- Conduct employee awareness training on network security basics.

### Detect
Improve monitoring to identify similar threats faster:
- Configure network monitoring software to detect abnormal traffic spikes (e.g., sudden ICMP floods).
- Implement an Intrusion Detection System (IDS) for signature-based and anomaly-based detection.
- Enable firewall logging for incoming ICMP and spoofed IP attempts.
- Set up continuous monitoring of network traffic patterns and alerts for deviations.

### Respond
For future incidents:
- Immediately isolate affected network segments (e.g., block offending IPs at the firewall).
- Contain the incident by rate-limiting or dropping ICMP traffic.
- Analyze logs (firewall, IDS, network traffic) to trace the attack source.
- Communicate internally (notify management) and externally if required.
- Document lessons learned and update response playbooks.

### Recover
Restore normal operations:
- Bring critical services back online first after the flood subsides.
- Verify system integrity and data (no data loss in this DoS case, but always check).
- Restore non-critical services gradually.
- Improve recovery processes: Regular backups of configurations, automated failover for critical services.
- Conduct post-incident review to refine recovery procedures.

## Skills Gained & Key Learnings
- Applied the NIST CSF to structure incident analysis and planning.
- Understood DoS/ICMP flood mechanics and network-layer attack vectors.
- Gained experience in recommending layered defenses (firewall rules, IDS/IPS, monitoring).
- Improved ability to translate technical incidents into actionable security improvements.
- Recognized the importance of proactive monitoring and quick containment in network security.

**Challenges**: Differentiating between detection and response actions; learned to prioritize containment first.

This activity strengthened my understanding of how network concepts (protocols like ICMP, firewalls, traffic analysis) tie directly into broader cybersecurity frameworks.

Feel free to explore the full NIST CSF documentation for more details!
