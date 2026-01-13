# AWS Misconfiguration Review

## 📌 Summary
This assessment reviews an AWS environment for common security misconfigurations, focusing on IAM, S3, EC2, and logging. The goal is to identify weaknesses and recommend corrective actions.

---

## ☁️ Scope
- IAM Users, Roles, and Policies  
- S3 Bucket Permissions  
- EC2 Security Groups  
- CloudTrail Logging  
- Public Exposure Checks  

---

## 🧪 Findings

### 1. IAM Misconfigurations
- Overly permissive policies (e.g., `AdministratorAccess`)  
- Unused access keys  
- MFA disabled for console users  

### 2. S3 Bucket Issues
- Public read/write access  
- Missing encryption  
- No bucket policy restrictions  

### 3. EC2 Security Group Risks
- Open ports (0.0.0.0/0)  
- SSH/RDP exposed  
- Missing network segmentation  

### 4. Logging & Monitoring Gaps
- CloudTrail disabled / partially enabled  
- No log file validation  
- No GuardDuty enabled  

---

## 🧠 Analysis
- Misconfigurations increase the risk of unauthorized access  
- Lack of MFA and key rotation weakens IAM security  
- Public S3 buckets expose sensitive data  
- Missing logging reduces detection capability  

---

## 🛡 Recommended Remediation
- Enforce MFA for all IAM users  
- Apply least‑privilege policies  
- Restrict S3 buckets to private access  
- Enable CloudTrail in all regions  
- Enable GuardDuty  
- Harden security groups (remove 0.0.0.0/0)  

---

## 📚 MITRE ATT&CK Mapping
- **Initial Access:** T1078 – Valid Accounts  
- **Discovery:** T1087 – Account Discovery  
- **Collection:** T1530 – Data from Cloud Storage  

---

## 📝 Conclusion
The AWS environment contains several high‑risk misconfigurations that should be addressed immediately. Implementing the recommended controls will significantly improve cloud security posture.