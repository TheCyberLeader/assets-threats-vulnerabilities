# Assets, Threats, and Vulnerabilities 🛡️

![Status](https://img.shields.io/badge/Status-Complete-success)
![Projects](https://img.shields.io/badge/Projects-6-blue)
![Skills](https://img.shields.io/badge/Skills-Risk%20Assessment%20%7C%20Threat%20Modeling%20%7C%20Vulnerability%20Management-informational)

## Table of Contents
- [Overview](#overview)
- [Portfolio Quick Reference](#-portfolio-quick-reference)
- [Skills Demonstrated](#skills-demonstrated)
- [Project 1: Database Server Vulnerability Assessment](#-project-1-database-server-vulnerability-assessment)
- [Project 2: Bank Risk Register & Risk Matrix](#-project-2-bank-risk-register--risk-matrix)
- [Project 3: Data Leak Incident Response](#-project-3-data-leak-incident-response)
- [Project 4: Home Network Asset Inventory](#-project-4-home-network-asset-inventory)
- [Project 5: PASTA Threat Modeling Framework](#-project-5-pasta-threat-modeling-framework)
- [Project 6: Security Event Log Analysis](#-project-6-security-event-log-analysis)
- [Skills & Tools Demonstrated](#-skills--tools-demonstrated)
- [Technical Competencies](#technical-competencies)
- [Key Learning Outcomes](#key-learning-outcomes)

---

## Overview
**Note: These projects are educational examples. All scenarios are simulated for learning purposes and demonstrate the practical application of industry-standard frameworks.**

This portfolio demonstrates hands-on technical skills in identifying, analyzing, and managing the three foundational elements of cybersecurity risk: **Assets, Threats, and Vulnerabilities**. Each project showcases both the technical execution and the strategic rationale that connects tactical security work to business priorities and risk management.

**Key Question Addressed**: How do we systematically identify what we're protecting, what we're protecting it from, and where our weaknesses lie, then translate that into actionable governance decisions?

---

## 📊 Portfolio Quick Reference
| Metric | Value |
|--------|-------|
| **Total Projects** | 6 |
| **Primary Frameworks** | NIST SP 800-30, PASTA, NIST CSF |
| **Key Skills** | Risk Assessment, Threat Modeling, Vulnerability Analysis, Access Control, Incident Response |
| **Focus Areas** | Asset Management, Risk Quantification, Security Controls, Compliance |

---

## Skills Demonstrated
- Asset inventory and classification using sensitivity levels
- NIST SP 800-30 Rev. 1 vulnerability assessment methodology
- Risk quantification using Likelihood × Severity matrices
- PASTA (Process for Attack Simulation and Threat Analysis) framework
- Attack tree methodology for threat path analysis
- Data flow diagram development for attack surface mapping
- Access control design aligned with least privilege (NIST SP 800-53: AC-6)
- Incident response and root cause analysis
- Security event log parsing and investigation
- Risk register development and maintenance
- Remediation strategy development with technical controls
- Security control mapping to compliance requirements

---

## 🔐 Project 1: Database Server Vulnerability Assessment
**Note: This is an educational simulation designed to demonstrate NIST-compliant vulnerability assessment skills**

### Project Description
Marketing operations at the organization depend on a centralized MySQL database storing customer and campaign data. The existing access controls did not reflect appropriate authorization levels, creating regulatory and operational risk. I conducted a comprehensive vulnerability assessment following NIST SP 800-30 Rev. 1 guidelines to identify security gaps and develop a remediation roadmap aligned with compliance requirements.

---

### System Description

**Infrastructure Details:**
- **Hardware**: Powerful CPU processor with 128GB memory
- **Operating System**: Latest version of Linux
- **Database**: MySQL database management system
- **Network**: IPv4 addressing with SSL/TLS encrypted connections
- **Purpose**: Stores customer data, campaign data, and analytics for marketing operations

---

### Assessment Scope

**Evaluation Parameters:**
- **Focus Area**: Current access controls of the system
- **Time Period**: Three months (June 20XX to August 20XX)
- **Framework**: NIST SP 800-30 Rev. 1 - Guide for Conducting Risk Assessments
- **Critical Assets**: Customer data, campaign data, marketing analytics

---

### Risk Assessment Approach

The assessment considered data storage and management procedures, evaluating:

1. **Threat Sources**: Potential adversaries with motivation to access customer data
2. **Likelihood Analysis**: Probability of exploitation given open access permissions
3. **Severity Analysis**: Impact weighed against day-to-day operational needs
4. **Risk Scoring**: Likelihood × Impact = Priority

---

### Key Findings

**Critical Security Gap Identified:**
- **Issue**: Open access permissions to database server
- **Risk Level**: High
- **Impact**: Unauthorized access to sensitive customer and campaign data
- **Compliance Concern**: Failure to meet data protection requirements

---

### Remediation Strategy

**Technical Controls Implemented:**

1. **Authentication & Authorization**
   - Strong password policies
   - Role-based access controls (RBAC)
   - Multi-factor authentication (MFA)
   - Limited user privileges to minimum required

2. **Encryption**
   - Migration from SSL to TLS for data in motion
   - Stronger encryption protocols for sensitive data

3. **Network Security**
   - IP allow-listing restricted to corporate offices
   - Prevention of random internet connections to database

**Governance Alignment:**
- Recommendations mapped to compliance requirements
- Controls support business continuity needs
- Risk-based approach to resource allocation

---

### Summary: Vulnerability Assessment

I successfully conducted a NIST SP 800-30 compliant vulnerability assessment that identified critical access control deficiencies and provided a comprehensive remediation roadmap. The assessment process included:

1. **System Documentation** - Detailed infrastructure and purpose analysis
2. **Scope Definition** - Clear parameters for evaluation period and focus areas
3. **Risk Analysis** - Systematic evaluation of threats, likelihood, and impact
4. **Control Design** - Technical solutions aligned with compliance and business needs

This demonstrates the ability to translate technical vulnerabilities into business risk language and develop actionable security controls that protect organizational assets.

[🔝 Back to Top](#table-of-contents)

---

## 📊 Project 2: Bank Risk Register & Risk Matrix
**Note: This is an educational simulation designed to demonstrate risk quantification and prioritization skills**

### Project Description

A coastal bank serving 2,000 individual accounts and 200 commercial accounts required systematic risk assessment to balance operational availability with data protection and regulatory compliance. I developed a comprehensive risk register using quantified scoring to enable rational resource allocation and prioritization of security investments.

---

### Operational Environment

**Organization Profile:**
- **Location**: Coastal area with low crime rates
- **Workforce**: 100 on-premise employees, 20 remote employees
- **Customer Base**: 2,000 individual accounts, 200 commercial accounts
- **Business Partnerships**: Professional sports team, 10 local businesses
- **Regulatory Requirements**: Federal Reserve cash availability mandates, financial data security

---

### Risk Assessment Methodology

**Scoring Framework:**
- **Likelihood Scale**: 1 (Rare) to 3 (Certain)
- **Severity Scale**: 1 (Low Impact) to 3 (Catastrophic)
- **Priority Formula**: Likelihood × Severity = Risk Score
- **Priority Range**: 1-9 (higher scores require immediate action)

---

### Risk Assessment Results

| Asset | Risk/Threat | Description | Likelihood | Severity | Priority |
|-------|-------------|-------------|------------|----------|----------|
| **Financial records** | **Publicly accessible backup server** | Database server of backed up data is publicly accessible | **3** | **3** | **9 (Critical)** |
| Funds | Compromised user database | Customer data is poorly encrypted | 2 | 3 | 6 |
| Funds | Business email compromise | Employee tricked into sharing confidential information | 2 | 2 | 4 |
| Funds | Physical theft | Bank's safe is left unlocked | 1 | 3 | 3 |
| Operations | Supply chain disruption | Delivery delays due to natural disasters | 1 | 2 | 2 |

---

### Risk Matrix Visualization

|  | **Low (1)** | **Moderate (2)** | **Catastrophic (3)** |
|---|---|---|---|
| **Certain (3)** | 3 | 6 | 9 |
| **Likely (2)** | 2 | 4 | 6 |
| **Rare (1)** | 1 | 2 | 3 |

---

### Governance Insights

**Strategic Observations:**
- The Priority 9 finding (exposed backup server) justified immediate remediation budget despite competing priorities
- Business partnerships increase data compromise risk through additional exposure vectors
- Physical theft rated low priority due to location in low-crime area
- Risk quantification transforms subjective concerns into objective decision criteria

**Resource Allocation Guidance:**
- **Priority 9**: Immediate action required (publicly accessible backup)
- **Priority 6**: Schedule within current quarter (database encryption)
- **Priority 2-4**: Address in routine maintenance cycles

---

### Summary: Risk Register

I successfully developed a quantified risk register that enables data-driven security decision-making. The methodology demonstrates:

1. **Systematic Risk Identification** - Comprehensive threat cataloging across asset categories
2. **Quantified Scoring** - Likelihood × Severity formula for objective prioritization
3. **Strategic Context** - Business environment considerations in risk evaluation
4. **Actionable Priorities** - Clear guidance for resource allocation

This risk-based approach supports informed governance decisions and justifies security investments with measurable business impact.

[🔝 Back to Top](#table-of-contents)

---

## 🔍 Project 3: Data Leak Incident Response
**Note: This is an educational simulation designed to demonstrate incident analysis and NIST framework application skills**

### Project Description

A sales team member accidentally shared an internal product folder containing unreleased product information with an external business partner, who subsequently posted promotional materials to social media. I conducted a root cause analysis using the NIST Cybersecurity Framework and NIST SP 800-53 control review to identify control gaps and develop remediation recommendations.

---

### Incident Summary

**Timeline of Events:**
1. Sales manager shares access to internal folder with team during meeting
2. Folder contains: new product files (not publicly announced), customer analytics, promotional materials
3. Manager warns team not to share outside the organization
4. During video call with business partner, sales representative forgets warning
5. Representative shares link to promotional materials for partner distribution
6. Representative accidentally shares entire folder link instead of specific materials
7. Business partner posts unreleased product information to social media

---

### Root Cause Analysis

**Primary Control Failures:**

1. **Inadequate Access Controls**
   - Internal folder access not limited to sales team
   - No role-based restrictions preventing external sharing

2. **Missing Authorization Boundaries**
   - Business partner granted sharing permissions beyond need-to-know
   - No technical controls preventing external distribution

3. **Insufficient Auditing**
   - No regular privilege audits
   - Missing activity logging for shared folder access

---

### NIST Cybersecurity Framework Control Review

**Framework Mapping:**
- **Function**: Protect (PR)
- **Category**: Data Security (PR.DS)
- **Subcategory**: PR.DS-5: Protections against data leaks
- **Reference**: NIST SP 800-53: AC-6 (Least Privilege)

---

### NIST SP 800-53: AC-6 Analysis

**Control Definition:**
Only the minimal access and authorization required to complete a task or function should be provided to users.

**Discussion:**
Processes, user accounts, and roles should be enforced as necessary to achieve least privilege. The intention is to prevent a user from operating at privilege levels higher than what is necessary to accomplish business objectives.

**Control Enhancements:**
1. Restrict access to sensitive resources based on user role
2. Automatically revoke access to information after a period of time
3. Keep activity logs of provisioned user accounts
4. Regularly audit user privileges

---

### Gap Analysis

**Identified Control Deficiencies:**

| Control Area | Current State | Gap Identified |
|-------------|---------------|----------------|
| Access Restrictions | Folder open to all users | Should be role-based (sales team only) |
| External Sharing | Permitted by default | Should require explicit approval |
| Privilege Auditing | No regular reviews | Quarterly audits needed |
| Activity Logging | Not enabled | Required for accountability |
| Access Revocation | Manual only | Automatic time-based revocation needed |

---

### Recommendations

**Technical Controls:**
1. **Restrict file access based on user role**
   - Implement role-based access control (RBAC)
   - Sales team access only for internal product folders

2. **Enable activity logging for provisioned accounts**
   - Track all file access and sharing activities
   - Create audit trail for investigation

**Process Controls:**
3. **Implement regular privilege audits**
   - Quarterly review of folder access permissions
   - Automated alerts for privilege escalation

4. **Deploy automatic access revocation policies**
   - Time-based access expiration for sensitive folders
   - Require re-authorization for continued access

**Awareness & Training:**
5. **Security awareness training**
   - Reinforce data handling procedures
   - Clarify sharing authorization boundaries

---

### Justification

Data leaks can be prevented if shared links to internal files are restricted to employees only. Requiring managers and security teams to regularly audit access to team files would help limit the exposure of sensitive information. Technical controls must be paired with process controls and awareness training to create defense-in-depth.

---

### Summary: Incident Response

I successfully conducted a comprehensive incident analysis using NIST frameworks to identify root causes and develop remediation strategies. The investigation process included:

1. **Incident Reconstruction** - Detailed timeline of events leading to data exposure
2. **Framework Application** - NIST CSF and SP 800-53 control mapping
3. **Gap Analysis** - Systematic identification of control deficiencies
4. **Remediation Strategy** - Multi-layered approach (technical, process, awareness)

This demonstrates the ability to translate security incidents into actionable control improvements aligned with industry standards.

[🔝 Back to Top](#table-of-contents)

---

## 🏠 Project 4: Home Network Asset Inventory
**Note: This is an educational simulation designed to demonstrate asset management and classification skills**

### Project Description

A small business operating from a home office required comprehensive asset management to identify protection priorities and implement appropriate security controls. I developed a systematic asset inventory with sensitivity classifications that enable risk-based security decisions.

---

### Asset Classification Framework

**Sensitivity Levels:**
- **Restricted**: Highest protection level; limited to specific authorized users
- **Confidential**: Limited to specific users; enhanced security controls required
- **Internal-only**: Organization members only; not for external sharing
- **Public**: No confidentiality requirements; can be freely shared

**Network Access Categories:**
- **Continuous**: Constant connection to network
- **Occasional**: Intermittent network connectivity

**Location Tracking:**
- **On-premises**: Physical presence at home office
- **On and off-premises**: Mobile devices that travel

---

### Complete Asset Inventory

| # | Asset | Network Access | Owner | Location | Sensitivity | Security Notes |
|---|-------|----------------|-------|----------|-------------|----------------|
| 1 | **Network router** | Continuous | ISP | On-premises | Confidential | 2.4 GHz and 5 GHz dual-band; all devices connect to 5 GHz |
| 2 | **Desktop computer** | Occasional | Homeowner | On-premises | Restricted | Contains private photos and personal information |
| 3 | **Guest smartphone** | Occasional | Friend | On/off-premises | Internal-only | Friend's device with temporary network access |
| 4 | **External hard drive** | Occasional | Homeowner | On-premises | Confidential | Personal media storage (music and movies) |
| 5 | **Streaming media player** | Continuous | Homeowner | On-premises | Internal-only | Payment card information stored for rentals |
| 6 | **Portable game console** | Occasional | Friend | On/off-premises | Internal-only | Has camera and microphone capabilities |

---

### Asset Analysis by Sensitivity

**Restricted Assets (1):**
- Desktop computer - Private photos require strongest protection
- **Controls Needed**: Full disk encryption, strong authentication, MFA

**Confidential Assets (2):**
- Network router - Gateway to all network traffic
- External hard drive - Personal media collection
- **Controls Needed**: Strong passwords, encryption, limited physical access

**Internal-only Assets (3):**
- Guest smartphone - Temporary access device
- Streaming media player - Contains payment data
- Game console - Has recording capabilities
- **Controls Needed**: Network segmentation, time-based access, activity monitoring

---

### Governance Application

**Risk-Based Control Mapping:**

| Sensitivity Level | Required Controls | Justification |
|------------------|-------------------|---------------|
| **Restricted** | Encryption (AES-256)<br>MFA<br>Strong passwords<br>Access logging | Contains most sensitive personal data |
| **Confidential** | Encryption<br>Strong passwords<br>Physical security | Protects valuable personal assets and network access |
| **Internal-only** | Network segmentation<br>Time-based access<br>Basic passwords | Prevents unauthorized external access |

**Network Architecture Recommendations:**
1. **Primary Network**: Restricted and Confidential assets only
2. **Guest Network**: Internal-only devices (friends' devices)
3. **IoT Network**: Streaming player and game console isolation

---

### Summary: Asset Inventory

I successfully developed a comprehensive asset inventory with risk-based classification that enables informed security control decisions. The methodology demonstrates:

1. **Systematic Cataloging** - Complete enumeration of network-connected assets
2. **Multi-Dimensional Classification** - Sensitivity, access patterns, location tracking
3. **Risk-Based Controls** - Protection levels matched to asset value
4. **Network Segmentation Strategy** - Isolation recommendations based on trust levels

This asset management approach supports the principle of least privilege and enables efficient resource allocation for security controls.

[🔝 Back to Top](#table-of-contents)

---

## 🎯 Project 5: PASTA Threat Modeling Framework
**Note: This is an educational simulation designed to demonstrate systematic threat modeling skills**

### Project Description

Organizations require systematic methods to identify and analyze potential threats to their systems and data. I applied the PASTA (Process for Attack Simulation and Threat Analysis) framework to develop comprehensive threat models that bridge technical threat identification with business risk context, enabling informed security control investments.

---

### PASTA Framework Overview

PASTA is a seven-stage risk-centric threat modeling methodology that aligns technical requirements with business objectives.

**Framework Stages:**

1. **Define Security Objectives**
   - Identify business requirements and compliance needs
   - Establish security goals aligned with organizational priorities

2. **Define Technical Scope**
   - Map the attack surface and technical boundaries
   - Identify all components requiring protection

3. **Application Decomposition**
   - Break down system architecture into components
   - Analyze data flows and trust boundaries

4. **Threat Analysis**
   - Identify potential threat actors and their capabilities
   - Develop threat scenarios based on business context

5. **Vulnerability Analysis**
   - Identify weaknesses that could be exploited
   - Map vulnerabilities to potential threats

6. **Attack Modeling**
   - Create attack trees showing threat progression paths
   - Analyze likelihood of successful attacks

7. **Risk and Impact Analysis**
   - Quantify business impact of successful attacks
   - Prioritize risks for remediation

---

### Data Flow Diagram Development

**Purpose**: Visual representation of how data moves through a system, identifying:
- Data sources and destinations
- Processing components
- Trust boundaries
- Potential attack vectors

**Key Elements Mapped:**
- External entities (users, systems, services)
- Processes (applications, services, functions)
- Data stores (databases, file systems)
- Data flows (connections between components)

**Security Insights:**
- Trust boundaries where data crosses security zones
- High-value targets for attackers
- Points requiring additional security controls

---

### Attack Tree Methodology

**Purpose**: Hierarchical analysis showing how an attacker might achieve their objectives.

**Tree Structure:**
- **Root**: Attacker's ultimate goal
- **Branches**: Different attack paths to achieve the goal
- **Leaves**: Specific techniques or vulnerabilities exploited

**Analysis Benefits:**
- Visualizes multiple attack scenarios
- Identifies critical nodes requiring protection
- Supports risk prioritization decisions
- Enables proactive control design

**Example Attack Paths Analyzed:**
1. External network attack → Exploit web vulnerability → Access database
2. Social engineering → Credential theft → Privilege escalation
3. Physical access → USB malware → System compromise

---

### Threat Scenario Development

**Threat Actor Categories:**
- External attackers (hackers, organized crime)
- Malicious insiders (employees, contractors)
- Nation-state actors
- Automated threats (malware, botnets)

**Scenario Components:**
- Threat actor motivation
- Capability assessment
- Target assets
- Attack vectors
- Expected impact

---

### Risk and Impact Analysis

**Business Impact Mapping:**

| Threat Scenario | Confidentiality Impact | Integrity Impact | Availability Impact | Overall Business Risk |
|----------------|----------------------|------------------|--------------------|--------------------|
| Data breach | High | Medium | Low | High |
| Ransomware | Medium | High | High | Critical |
| Insider threat | High | High | Medium | High |
| DDoS attack | Low | Low | High | Medium |

**Risk Prioritization:**
- Critical risks require immediate investment
- High risks scheduled for current planning cycle
- Medium risks addressed in routine operations
- Low risks monitored for changes

---

### Strategic Value of PASTA

**Business Benefits:**
1. **Informed Investment Decisions**
   - Security spending justified by quantified business risk
   - Resources allocated to highest-impact threats

2. **Proactive Security Posture**
   - Threats identified before exploitation
   - Controls designed based on attack path analysis

3. **Stakeholder Communication**
   - Technical threats translated to business language
   - Executive leadership understands security priorities

4. **Compliance Support**
   - Demonstrates due diligence in risk management
   - Documents threat analysis for auditors

---

### Summary: PASTA Threat Modeling

I successfully applied the PASTA framework to develop comprehensive threat models that support strategic security decision-making. The methodology demonstrates:

1. **Systematic Analysis** - Seven-stage structured approach to threat identification
2. **Visual Communication** - Data flow diagrams and attack trees for stakeholder understanding
3. **Risk Quantification** - Business impact assessment for prioritization
4. **Strategic Alignment** - Threat modeling connected to organizational objectives

This threat modeling capability enables proactive control design rather than reactive incident response.

[🔝 Back to Top](#table-of-contents)

---

## 📝 Project 6: Security Event Log Analysis
**Note: This is an educational simulation designed to demonstrate log analysis and investigation skills**

### Project Description

Security event logs provide critical audit trails for detecting unauthorized activities and supporting forensic investigations. I analyzed accounting system event logs to verify user activities, validate authorization levels, and ensure compliance with access control policies.

---

### Event Log Details

**Raw Event Data:**
```
Event Type: Information
Event Source: AdsmEmployeeService
Event Category: None
Event ID: 1227
Date: 10/03/2023
Time: 8:29:57 AM
User: Legal\Administrator
Computer: Up2-NoGud
IP: 152.207.255.255
Description: Payroll event added. FAUX_BANK
```

---

### Investigative Process

**1. Event Log Parsing**
- Extracted structured data from raw log entries
- Identified key fields: timestamp, user, system, action

**2. Timestamp Correlation**
- Verified event occurred during business hours (8:29:57 AM)
- Confirmed date consistency (10/03/2023)
- Cross-referenced with authorized change windows

**3. User Activity Pattern Analysis**
- **User Identified**: Legal\Administrator account
- **Action Performed**: Payroll event modification
- **System Accessed**: Up2-NoGud (accounting system)
- **Event Type**: Payroll event added for FAUX_BANK

**4. Privilege Verification**
- Confirmed administrator-level access used
- Validated whether Legal department authorized for payroll modifications
- Assessed whether least privilege principle applied

**5. IP Address Validation**
- **IP Address**: 152.207.255.255
- Verified against known corporate IP ranges
- Checked for geographic consistency with user location
- Identified potential anomalies (suspicious external access)

**6. Payroll Event Verification**
- Cross-referenced with authorized change management system
- Verified approval documentation exists
- Confirmed FAUX_BANK entity is legitimate
- Checked for unusual patterns (time of day, frequency)

---

### Security Concerns Identified

**Potential Red Flags:**
1. **Cross-Department Access**: Legal\Administrator modifying payroll records
2. **Privilege Level**: Administrator account for routine payroll task
3. **System Naming**: "Up2-NoGud" suggests non-standard naming convention
4. **Entity Name**: "FAUX_BANK" requires verification of legitimacy

**Investigation Questions:**
- Does Legal department require payroll modification access?
- Should payroll events use standard user accounts instead of administrator?
- Is the IP address consistent with Legal department's network segment?
- Has FAUX_BANK been verified as a legitimate entity?

---

### Governance Application

**Audit Trail Importance:**
- Event logs provide accountability for all system actions
- Enable detection of unauthorized activities
- Support forensic investigations after incidents
- Demonstrate compliance with regulatory requirements

**Best Practices Demonstrated:**
- Regular log review schedule
- Correlation of multiple log fields
- Privilege escalation monitoring
- Cross-reference with authorization systems

**Recommendations:**
1. Implement automated alerts for cross-department access
2. Review administrator account usage for routine operations
3. Standardize system naming conventions
4. Require approval documentation linkage in log entries

---

### Summary: Event Log Analysis

I successfully conducted systematic security event log analysis to identify potential authorization issues and verify user activities. The investigation process demonstrates:

1. **Structured Analysis** - Methodical examination of all log fields
2. **Contextual Evaluation** - Assessment within business and security context
3. **Anomaly Detection** - Identification of potential security concerns
4. **Governance Integration** - Connection to accountability and compliance

This log analysis capability supports continuous monitoring and detection of unauthorized activities before they escalate to security incidents.

[🔝 Back to Top](#table-of-contents)

---

## 🎯 Skills & Tools Demonstrated

### Risk Management Frameworks
![NIST SP 800-30](https://img.shields.io/badge/NIST_SP_800--30-0066CC?style=flat)
![NIST SP 800-53](https://img.shields.io/badge/NIST_SP_800--53-0066CC?style=flat)
![NIST CSF](https://img.shields.io/badge/NIST_CSF-4479A1?style=flat)
![PASTA](https://img.shields.io/badge/PASTA-FF6B6B?style=flat)

### Security Analysis Tools
![Risk Assessment](https://img.shields.io/badge/Risk_Assessment-95E1D3?style=flat)
![Threat Modeling](https://img.shields.io/badge/Threat_Modeling-4ECDC4?style=flat)
![Vulnerability Analysis](https://img.shields.io/badge/Vulnerability_Analysis-FCC624?style=flat)

### Documentation & Reporting
![Technical Writing](https://img.shields.io/badge/Technical_Writing-4EAA25?style=flat)
![Security Reports](https://img.shields.io/badge/Security_Reports-003545?style=flat)
![Compliance](https://img.shields.io/badge/Compliance-FF6B6B?style=flat)

---

## Technical Competencies

| Competency Area | Specific Skills |
|-----------------|----------------|
| **Risk Assessment** | NIST SP 800-30 methodology, risk scoring matrices (Likelihood × Severity), quantified risk prioritization, risk register development, remediation strategy design |
| **Threat Modeling** | PASTA framework application, data flow diagram development, attack tree analysis, threat scenario development, threat actor profiling |
| **Vulnerability Management** | Systematic vulnerability identification, control gap analysis, remediation roadmapping, compliance mapping, control effectiveness assessment |
| **Asset Management** | Asset inventory development, sensitivity classification, risk-based control mapping, network segmentation strategy, asset lifecycle tracking |
| **Access Control** | RBAC design, least privilege implementation, privilege auditing, access revocation policies, NIST SP 800-53 AC-6 application |
| **Incident Response** | Root cause analysis, NIST CSF application, control deficiency identification, remediation recommendations, lessons learned documentation |
| **Security Auditing** | Event log analysis, user activity monitoring, privilege verification, anomaly detection, audit trail correlation |
| **Governance Integration** | Risk-to-business translation, compliance alignment, executive communication, security metrics development, policy enforcement |

---

## Key Learning Outcomes

**Risk Management Excellence:**
- Applied industry-standard frameworks (NIST SP 800-30, PASTA, CSF) to real-world scenarios
- Demonstrated ability to quantify risk using objective scoring methodologies
- Translated technical vulnerabilities into business impact language for governance decisions
- Developed comprehensive remediation strategies aligned with compliance and business needs

**Strategic Security Thinking:**
- Connected tactical security controls to organizational priorities and regulatory requirements
- Applied principle of least privilege across multiple domains (access control, asset management)
- Demonstrated risk-based approach to resource allocation and investment prioritization
- Bridged technical execution with strategic leadership through governance integration

**Practical Application:**
- Created actionable deliverables (risk registers, vulnerability reports, threat models, asset inventories)
- Applied systematic methodologies to complex security challenges
- Developed documentation meeting professional security standards
- Demonstrated both technical proficiency and strategic business acumen

**Professional Readiness:**
This portfolio showcases competencies essential for cybersecurity leadership roles requiring both technical depth and governance perspective. The projects demonstrate the ability to conduct comprehensive security assessments, apply industry frameworks, quantify risk for decision-making, and communicate technical findings to business stakeholders. These skills directly support enterprise security program development, risk management, compliance, and strategic security planning.

---
## 🔗 Navigation
[⬅️ Back to Portfolio Home](https://github.com/TheCyberLeader) | [📧 Contact](mailto:m@riegrc.com) | [💼 LinkedIn](https://linkedin.com/in/mariezw)

---

[![](https://visitcount.itsvg.in/api?id=TheCyberLeader-linux-command-line-mastery&icon=0&color=0)](https://visitcount.itsvg.in)
