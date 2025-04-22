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






# Security Consultation Report - Southern Cross University

## Table of Contents

1. [Introduction](#introduction)
2. [Risk Assessment](#risk-assessment)
3. [Authentication Schemes](#authentication-schemes)
    1. [Password-Based Authentication](#password-based-authentication)
    2. [Certificate-Based Authentication](#certificate-based-authentication)
4. [Spamming](#spamming)
    1. [Email Spam](#email-spam)
    2. [Spam Comments](#spam-comments)
    3. [Spam Text](#spam-text)
5. [References](#references)

---

## Introduction

The report aims to evaluate some of the risks which are associated with the top 3 critical assets of Southern Cross University. Furthermore, two authentication schemes are discussed and compared, and the use of electronic messaging systems to send unsolicited bulk messages for advertising purposes or spreading malware is examined.

Southern Cross University is an Australian public university with campuses in several countries around the world (Wikipedia, 2020). It is ranked among the top 100 young universities globally and offers many different types of courses. The table below shows the top 3 critical assets of Southern Cross University with some of their associated threats. A semi-quantitative risk analysis was used to define the levels of risk each threat possesses.

---

## Risk Assessment

| Asset                      | Vulnerabilities and Threats                                              | Impact | Likelihood | Risk   | Controls                                                                 |
|----------------------------|-------------------------------------------------------------------------|--------|------------|--------|--------------------------------------------------------------------------|
| **Webserver**               | 1. Poor security configuration in servers can result in a DDoS Attack     | 5      | 3          | 15     | Deploy anti-DDoS hardware and software modules, continuously monitor traffic, robust firewalls, data backup |
|                            | 2. Vulnerable web application tolerates Cross-Site Scripting (XSS)       | 4      | 3          | 12     | Regular scanning, traffic filtering, use proper escaping/encoding        |
|                            | 3. Unauthorized access can affect the CIA                               | 4      | 5          | 20     | Implement RBAC, proper authentication schemes                           |
| **Student Information DB** | 1. Weakly coded web application allowing SQL Injection attack            | 4      | 2          | 8      | Run automated SQL Injection Tools, patching flaws                       |
|                            | 2. Insider threats (no proper access control)                           | 5      | 4          | 20     | Use proper cryptographic tools, I-AAA, passwords, RBAC, confidential model |
|                            | 3. Unorganized data causing accidental exposure and data theft          | 2      | 3          | 6      | Use proper inventory, backup data                                        |
| **AI Lab**                  | 1. Lack of proper access control allows malicious humans to affect the CIA | 5      | 4          | 20     | Implement I-AAA, Bell-LaPadula model, proper physical security           |
|                            | 2. Network flaws provide opportunities for attackers                    | 4      | 4          | 16     | Hardware redundancy, regular scanning for vulnerabilities, robust network firewalls |
|                            | 3. Weak firewalls and outdated malware protections result in attacks    | 3      | 3          | 9      | Cybersecurity training, update malware scanners                          |

---

## Authentication Schemes

### Password-Based Authentication

Password-Based Authentication is an authentication scheme that uses passwords to validate a user's identity before granting access to a resource. Initially, the user creates a password and shares it securely with the server. The server converts the password into an unreadable form using cryptography before storing it. Later, when the user wants to access the server, they provide the same password, which is hashed and compared with the stored value. If they match, authentication is successful, otherwise, access is denied.

Password-Based Authentication is costless and easy to implement but has many vulnerabilities. Passwords can be guessed or stolen through various techniques, such as brute-force attacks, phishing, or keylogging.

### Certificate-Based Authentication

Certificate-Based Authentication uses digital certificates to verify the identity of the user or device. A digital certificate is an electronic file containing the user’s identity and their public key. The certificate is signed by a trusted Certificate Authority (CA). This form of authentication provides higher security as it does not rely on passwords.

The client sends a request to the server, and the server returns a certificate containing its public key. The client then encrypts a message with its private key, which can only be decrypted by the server’s private key, establishing mutual trust and secure communication.

This method is more secure than password-based authentication because it prevents phishing and other attacks targeting passwords. However, it can be costly and difficult to install for some users.

---

## Spamming

### Email Spam

Email spam is an unsolicited message sent in bulk using email systems. Typical characteristics of spam include:

- Containing links and attachments
- Often an urgent message
- Missing sender’s ID
- No specific recipient
- Spelling errors
- Contains login requests or gift offers

#### Handling Spam Emails
- Avoid clicking on links or attachments
- Use spam filters
- Be familiar with spam characteristics
- Unsubscribe from mailing lists

### Spam Comments

Spam comments are messages posted by automated bots on websites, blogs, or other online platforms with high traffic. These comments are often irrelevant to the content and include links to other websites.

#### Recognizing Spam Comments
- The commenter does not use a real name
- The comment includes irrelevant links
- The comment is unrelated to the content

#### Handling Spam Comments
- Decrease the number of links in posts
- Blacklist undesirable keywords
- Use comment moderation
- Utilize anti-spam plugins

### Spam Text

Spam text messages are unsolicited messages sent via text. These messages may contain offers, urgent alerts, or links to malicious sites.

#### Handling Spam Texts
- Delete spam texts immediately
- Report spam
- Avoid clicking on links
- Recognize the features of spam texts

While spamming can sometimes be used legitimately, sending messages to a large number of people without their permission is against the law.

---

## References

- CISCO, Email Spam, viewed 2020, [http://www.sico.com](http://www.sico.com)
- Hughes, J, 2020, Preventing spam comments, viewed 2020, [http://www.themeisis.com](http://www.themeisis.com)
- NR, (2018), Digital Certificates, viewed 2020, [http://www.nr.com](http://www.nr.com)
- NSS, Certificate-Based Authentication, viewed 2020, [http://www.nss.com](http://www.nss.com)
- Paul Villanueva, (2016), X.509 Certificates, viewed 2020, [http://www.blog.keyfactor.com](http://www.blog.keyfactor.com)
- Rouse, M, Authentication, viewed 2020, [http://www.searchsecurity.techtarget.com](http://www.searchsecurity.techtarget.com)
- Wikipedia, SPAM, viewed 2020, [http://www.wikipedia.com](http://www.wikipedia.com)



