
# Botium Toys – Security Risk Assessment and Controls Evaluation

## 1. Project Overview

This project involves a simulated security risk assessment of Botium Toys, a fictional retail company.

The assessment was completed as part of the Google Cybersecurity Professional Certificate. It focuses on evaluating organizational assets, identifying security control gaps, reviewing compliance practices, and recommending improvements to strengthen the company's security posture.

**Project Type:** Security Risk Assessment / Governance, Risk, and Compliance (GRC)

**Framework Reference:** NIST Cybersecurity Framework (NIST CSF)

## 2. Scope and Objectives

The assessment covered Botium Toys' overall security program, including:

- Employee devices and equipment
- Internal network and systems
- Business applications and databases
- Data storage and retention
- Physical security controls
- Legacy system maintenance

The primary objective was to identify weaknesses in existing security controls and determine which improvements were necessary to reduce organizational risk.

## 3. Identified Security Risks

The assessment identified several weaknesses:

| Security Area | Identified Weakness |
|---|---|
| Access Control | All employees had access to internally stored data. |
| Data Encryption | Sensitive customer information was not encrypted. |
| Business Continuity | No disaster recovery plan was established. |
| Data Backup | Critical data backups were not maintained. |
| Intrusion Detection | No Intrusion Detection System (IDS) was installed. |
| Password Management | Password requirements were minimal, with no centralized password management system. |
| Asset Management | Assets were inventoried but not properly classified. |
| Legacy Systems | No regular maintenance schedule or clear intervention procedures existed. |

## 4. Controls and Compliance Evaluation

The assessment reviewed security controls and compliance practices related to:

- Least Privilege
- Separation of Duties
- Password Policies
- Firewall Protection
- Intrusion Detection
- Data Encryption
- Disaster Recovery
- Data Backups
- Physical Security

Compliance areas evaluated included:

- Payment Card Industry Data Security Standard (PCI DSS)
- General Data Protection Regulation (GDPR)
- System and Organization Controls (SOC)

## 5. Recommended Security Improvements

Based on the assessment, the following improvements were recommended:

1. Implement the Principle of Least Privilege to restrict access to sensitive information.
2. Introduce encryption for sensitive information at rest and in transit.
3. Establish regular data backup procedures and a disaster recovery plan.
4. Implement an Intrusion Detection System to identify potential security threats.
5. Strengthen password policies and introduce centralized password management.
6. Classify organizational assets according to their sensitivity and business importance.
7. Establish regular monitoring and maintenance procedures for legacy systems.

## 6. Independent Security Analysis

### Greatest Risk: Lack of Encryption for Sensitive Customer Information

I consider the lack of encryption for sensitive customer information to be one of the greatest security risks identified in this assessment.

Botium Toys handles sensitive information, including customer credit card data and personally identifiable information (PII). Without proper encryption, this information may be exposed and readable if unauthorized individuals gain access to the company's systems or databases.

This could result in data breaches, financial losses, reputational damage, and potential compliance issues.

I recommend implementing encryption for sensitive data at rest and in transit, alongside stronger access controls.

### Additional Observation: Unrestricted Employee Access

Encryption alone would not be sufficient to establish a strong security posture.

Even if sensitive information is encrypted, access should still be restricted to authorized personnel whose job responsibilities require it.

Implementing the Principle of Least Privilege would reduce unnecessary exposure and minimize the potential impact of compromised employee accounts.

## 7. Key Takeaways

Through this assessment, I developed a better understanding of:

- Identifying and evaluating organizational security risks.
- Recognizing weaknesses in existing security controls.
- Understanding the importance of encryption and access management.
- Evaluating security practices against compliance requirements.
- Developing recommendations to improve an organization's security posture.

This exercise strengthened my understanding of how security analysts assess risks and recommend appropriate security controls.

## 8. Supporting Documents

The following documents contain the detailed assessment and findings:

- Scope, Goals, and Risk Assessment Report
- Controls and Compliance Checklist

---

**Disclaimer:** This is an educational, simulated assessment based on the Botium Toys case study provided through the Google Cybersecurity Professional Certificate. It is not an actual security audit of a real organization.
