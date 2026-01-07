# AWS Cloud Security & Compliance Lab

## Project Overview
This is a self-directed cloud security lab built in AWS to simulate **SOC 2 Type II** and **PCI DSS** compliance requirements.  
The lab demonstrates audit logging, compliance monitoring, threat detection, and incident response for cloud resources.

---

## Objectives
- Implement AWS security controls aligned with SOC 2 and PCI DSS
- Enable centralized logging, monitoring, and detection
- Simulate and remediate a security incident
- Document incident response workflow

---

## Tools & Services Used
| AWS Service       | Purpose |
|------------------|---------|
| IAM               | Access control, MFA enforcement |
| CloudTrail        | Audit logging, event tracking |
| AWS Config        | Compliance rules and configuration monitoring |
| Security Hub      | Centralized security findings |
| GuardDuty         | Threat detection and anomaly alerts |
| S3                | Test environment for incident response |

---

## Lab Steps

1. **Secure Account**
   - Enabled MFA on root account
   - Created IAM roles: `SecurityAdmin`, `ReadOnlyAudit`

2. **Enable CloudTrail**
   - Created trail `security-audit-trail`
   - Enabled management events and log file validation
   - Logs stored in an encrypted S3 bucket

3. **Enable AWS Config**
   - Added rules:
     - `root-account-mfa-enabled`
     - `iam-user-mfa-enabled`
     - `s3-bucket-public-read-prohibited`

4. **Enable Security Hub**
   - Enabled AWS Foundational Security Best Practices

5. **Enable GuardDuty**
   - Default detectors enabled

6. **Test Incident**
   - Created S3 bucket
   - Made it public (violating compliance)
   - AWS Config flagged it as noncompliant
   - Security Hub also generated a finding

7. **Remediate Incident**
   - Blocked public access on the S3 bucket
   - Verified AWS Config rule turned compliant

---

## Incident Response Workflow

**Incident:** Public S3 Bucket Exposure  
**Detection:** AWS Config & Security Hub  
**Impact:** Potential data exposure  
**Containment:** Blocked public access  
**Recovery:** Verified compliance  
**Lessons Learned:** Implement preventive controls, monitor logs continuously

---

## Screenshots (Optional)
- 01_MFA_Enabled.png  
- 02_CloudTrail_Logging.png  
- 03_AWSConfig_Rules.png  
- 04_SecurityHub_Findings.png  
- 05_GuardDuty_Enabled.png  
- 06_S3_Public_Test.png  
- 07_S3_Public_Fixed.png  

---

## Outcome
- Gained hands-on experience with AWS security tools
- Mapped compliance requirements to cloud services
- Successfully detected and remediated a cloud security incident
- Created documentation suitable for audit or interview discussions

---

