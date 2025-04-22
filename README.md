# Cybersecurity Reports - MASA's Current Cyber Threats

## Table of Contents

1. [Introduction](#introduction)
2. [Importance of Risk Assessment](#importance-of-risk-assessment)
3. [Critical Asset Identification](#critical-asset-identification)
4. [Risk Management for MASA’s Information Assets](#risk-management-for-masas-information-assets)
5. [Threat Identification](#threat-identification)
6. [Threat Assessment](#threat-assessment)
7. [References](#references)

---

## Introduction

Michigan Aeronautical Science Association (MASA) is a space-based engineering team associated with the University of Michigan. Their focus is on rocketry, and they have many customers around the world. As the world advances with increasingly sophisticated technologies, adversaries have also developed more complex techniques to exploit vulnerabilities. This report identifies some cyber risks MASA may face.

---

## Importance of Risk Assessment

Cyber risk assessment is a critical step for any organization interacting with the cyber world. According to CCOHS (2020), risk assessment identifies factors related to the likelihood of loss, helping organizations take precautionary measures. Through risk assessment, MASA can identify relevant threats and vulnerabilities, maintaining strong security policies to prevent loss.

Managing risks helps preserve organizational functions. Frameworks like qualitative risk assessment, using Likelihood and Consequences Ratings, are crucial for mitigating attacks. The approach is suitable as it helps avoid estimation errors.

---

## Critical Asset Identification

The aim of protecting MASA’s information assets is to prevent loss. Critical information assets for MASA have been identified as follows:

1. **Software** - Space-related programs such as HAL/S.
2. **Cloud Storage** - Private cloud storage hosted in Sydney.
3. **Satellites** - Expensive and irreplaceable.
4. **Desktops/Laptops** - Critical for project work.
5. **Networks** - Vital for communication between MASA's global offices.

These assets are crucial for MASA’s operations, and their loss could significantly impact the organization.

---

## Risk Management for MASA’s Information Assets

### Risk Assessment Table

| Asset            | Vulnerability & Threat                             | Likelihood | Risk (Impact) | Controls (Safeguards)                                        |
|------------------|----------------------------------------------------|------------|---------------|-------------------------------------------------------------|
| **Software**      | Human error, weak access control                   | Likely     | Major         | Proper privilege scheme (RBAC), disabling default admin user |
| **Cloud Storage** | Insider threats, weak passwords, lack of security | Possible   | High          | Multi-factor authentication, encryption                      |
| **Satellites**    | Malware, remote access                           | Unlikely   | Critical      | Anti-malware software, secure access protocols               |
| **Desktops/Laptops** | Ransomware, phishing                          | Likely     | High          | Anti-virus software, phishing awareness training             |
| **Network**       | Malware attacks, weak firewalls                   | Possible   | High          | Strong firewalls, regular vulnerability scans                 |

---

## Threat Identification

Key threats facing MASA include:

1. **Ransomware** - Malware encrypts data, demanding a ransom to restore access.
2. **DNS Hijacking** - Redirects users to malicious sites.
3. **Social Engineering** - Tricking individuals to break security protocols.
4. **Remote Access Trojan (RAT)** - Hackers gain remote control over systems.
5. **Phishing** - Fraudulent attempts to steal login credentials.

---

## Threat Assessment

MASA’s website is a critical asset vulnerable to **DNS hijacking**. Hackers could modify the site, damaging its integrity and causing organizational harm. Another key threat is **cross-site scripting (XSS)**, which allows attackers to modify website content. The impact on MASA could be severe, including reputational damage and loss of customer trust.

Risk levels for assets:

- **Software**: High
- **Satellites**: Low
- **Cloud Storage**: High
- **Network**: High
- **Website**: Very High
- **Desktops/Laptops**: Very High

---

## References

- Australian Cyber Security Centre (2017)
- CCOHS (2020)
- Wikipedia, "HAL/S"
- Brown & Harris (2020)

---
