**Security Hardening Assessment & Incident Analysis**

**NIST Cybersecurity Framework (CSF) | MITRE ATT&CK | Microsoft Defender | Microsoft 365**

**Overview**

Security controls are often evaluated only after an organization experiences a security incident. In reality, effective cybersecurity requires understanding how existing controls perform before an attack occurs and identifying weaknesses before they become business problems.

This project simulates a security assessment conducted for a fictional logistics company, **SwiftCart Logistics Ltd**, using the NIST Cybersecurity Framework (CSF) as the primary assessment methodology.

Rather than approaching security purely from a compliance perspective, the assessment is driven by realistic threat scenarios that organizations commonly face. Two incidents were analysed in depth:

- Business Email Compromise (BEC)
- Malware Infection via Unauthorized USB Device

Each incident was investigated from the perspective of a Security Analyst, including attack analysis, impact assessment, MITRE ATT&CK mapping, root cause analysis, containment planning, recovery actions, and long-term hardening recommendations.

The goal was not simply to identify weaknesses, but to understand how those weaknesses could be exploited and what practical controls would reduce organizational risk.

**Why This Project Matters**

Organizations are not compromised because they lack security tools, they are compromised because security controls fail to prevent, detect, or respond to attacks effectively.

This project examines those failures through the lens of realistic incidents, using the NIST Cybersecurity Framework to assess security posture and the MITRE ATT&CK framework to understand attacker behaviour. By connecting business risk, technical investigation, and security hardening recommendations, the project demonstrates the practical skills required to assess, investigate, and improve an organization's security maturity.

**Project Objectives**

The objectives of this project were to:

- Assess the security posture of a simulated enterprise environment using the NIST Cybersecurity Framework.
- Evaluate how existing security controls perform against common real-world attack scenarios.
- Identify gaps in preventive, detective, and responsive security capabilities.
- Develop risk-based recommendations to improve organizational resilience.
- Demonstrate incident investigation and security assessment methodologies commonly used by Security Operations Centre (SOC) analysts and security teams.

**Organization Profile**

**SwiftCart Logistics Ltd**

SwiftCart Logistics Ltd is a fictional mid-sized logistics and transportation company operating across East Africa.

The organization relies heavily on digital systems to manage:

- Inventory operations
- Shipment tracking
- Customer communications
- Financial transactions
- Internal collaboration

Its technology environment includes:

- Microsoft 365
- Active Directory
- Windows 11 Endpoints
- Microsoft Defender
- VPN Access
- Cloud-Based Business Applications

Because email, endpoint devices, and user accounts are critical to daily operations, they represent attractive targets for cyber attackers.

**Assessment Methodology**

The assessment was conducted using the five core functions of the NIST Cybersecurity Framework:

| **Function** | **Purpose**                                                                              |
| ------------ | ---------------------------------------------------------------------------------------- |
| Identify     | Understand assets, business processes, risks, and dependencies.                          |
| Protect      | Evaluate safeguards designed to reduce the likelihood of compromise.                     |
| Detect       | Assess monitoring and alerting capabilities used to identify malicious activity.         |
| Respond      | Review procedures used to contain and manage security incidents.                         |
| Recover      | Evaluate the organization's ability to restore operations and implement lessons learned. |

Rather than treating these functions as a checklist exercise, each recommendation was tied directly to observed weaknesses within the incident scenarios.

**Incident Scenarios**

**Incident 1: Business Email Compromise (BEC)**

A finance employee received a phishing email impersonating Microsoft Support and unknowingly submitted corporate credentials to a fraudulent login page.

The attacker successfully authenticated to Microsoft 365, established persistence through mailbox rule manipulation, and gained visibility into sensitive business communications.

Key areas analysed:

- Phishing attack lifecycle
- Credential theft
- Unauthorized account access
- Mailbox rule abuse
- Business impact assessment
- Identity security improvements

**Incident 2: Malware Infection via Unauthorized USB Device**

A warehouse employee connected a personal USB storage device containing malware to a corporate workstation.

After executing a malicious file disguised as a legitimate business application, the workstation became compromised and attempted communication with external attacker infrastructure.

Key areas analysed:

- Malware execution
- Endpoint compromise
- Persistence mechanisms
- Command and control activity
- Endpoint detection and response
- Device control and endpoint hardening

**MITRE ATT&CK Analysis**

To better understand attacker behaviour, both incidents were mapped to the MITRE ATT&CK framework.

This provided visibility into:

- Initial Access techniques
- Execution methods
- Persistence mechanisms
- Discovery activities
- Command and Control communications
- Potential attacker objectives

Using ATT&CK mapping allowed defensive recommendations to be tied directly to adversary behaviours rather than generic security best practices.

**Security Gaps Identified**

The assessment highlighted several recurring themes.

**Identity Security**

- Multi-factor authentication was not consistently enforced.
- Risk-based authentication controls were limited.
- Account monitoring could be improved.

**Endpoint Security**

- Unauthorized USB devices were permitted.
- Application execution controls were insufficient.
- Endpoint visibility required strengthening.

**Monitoring & Detection**

- Limited monitoring of high-risk account activity.
- Insufficient visibility into persistence mechanisms.
- Opportunities to improve security event correlation.

**User Awareness**

- Employees remained vulnerable to phishing and social engineering.
- Security awareness initiatives required greater emphasis on real-world attack techniques.

**Security Hardening Recommendations**

Recommendations were prioritized according to risk and potential impact.

**High Priority**

- Enforce Multi-Factor Authentication (MFA)
- Disable legacy authentication protocols
- Implement USB device control policies
- Deploy application allowlisting
- Strengthen endpoint detection and response capabilities

**Medium Priority**

- Implement conditional access policies
- Increase PowerShell logging and monitoring
- Conduct quarterly phishing simulations
- Improve security event monitoring and alerting

**Low Priority**

- Conduct periodic security audits
- Establish security metrics and reporting
- Perform regular incident response exercises

**Skills Demonstrated**

This project demonstrates practical experience in:

**Security Assessment**

- Security posture evaluation
- Gap analysis
- Risk assessment
- Security hardening

**Incident Response**

- Incident investigation
- Root cause analysis
- Containment planning
- Recovery planning

**Threat Analysis**

- MITRE ATT&CK mapping
- Attack chain analysis
- Adversary behaviour analysis
- Threat-informed defense

**Governance & Frameworks**

- NIST Cybersecurity Framework (CSF)
- Risk-based decision making
- Security control evaluation
- Security documentation

**Project Structure**

├── README.md

├── NIST-CSF-Assessment.pdf

├── Incident-01-Business-Email-Compromise.pdf

├── Incident-02-Malware-Infection.pdf

├── Risk-Register.xlsx

├── Security-Hardening-Roadmap.pdf

└── Supporting-Evidence/

**Files**

| **File**                                  | **Description**                                                       |
| ----------------------------------------- | --------------------------------------------------------------------- |
| NIST-CSF-Assessment.pdf                   | Full security posture assessment and framework analysis.              |
| Incident-01-Business-Email-Compromise.pdf | Detailed Business Email Compromise investigation and recommendations. |
| Incident-02-Malware-Infection.pdf         | Detailed malware incident investigation and recommendations.          |
| Risk-Register.xlsx                        | Identified risks, impact ratings, and prioritization.                 |
| Security-Hardening-Roadmap.pdf            | Recommended remediation and improvement plan.                         |

**Key Takeaways**

One of the most valuable lessons from this project was recognizing that security controls are most meaningful when evaluated against realistic attack scenarios.

Frameworks such as NIST CSF provide structure, but effective security assessment requires understanding how attackers operate, how incidents unfold, and how defensive controls perform under pressure.

By combining framework-based assessment with incident analysis and ATT&CK mapping, this project focuses on security from both a governance and operational perspective.

**Future Improvements**

Future iterations of this project may include:

- SIEM detection use cases
- Sample security alerts
- Simulated log analysis
- Incident response playbooks
- MITRE D3FEND defensive mappings
- Threat hunting scenarios
- Security metrics and KPI dashboards

**Disclaimer**

This project was developed for educational and portfolio purposes. All organizations, users, systems, incidents, and data referenced within this repository are fictional and were created to demonstrate cybersecurity assessment and incident response concepts.