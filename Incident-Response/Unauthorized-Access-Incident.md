# Unauthorized Access Incident

## 📌 Summary
This incident documents unauthorized access attempts against a workstation within the environment. The goal is to determine whether access was successful, identify the attack vector, and recommend containment and remediation steps.

---

## 🚨 Incident Details
- **Incident Type:** Unauthorized Access Attempt  
- **Detection Source:** EDR / SIEM  
- **Severity:** High  
- **Date/Time:** <insert>  
- **Affected Host:** <insert>  
- **User Involved:** <insert>  

---

## 🧪 Evidence Collected
### Host Artifacts
- Security Event Logs (4624/4625)
- Process creation logs (4688)
- EDR alerts
- Browser history (if relevant)
- Scheduled tasks / startup items

### Network Artifacts
- Outbound connections
- Suspicious IPs or domains
- Lateral movement attempts

---

## 🧠 Analysis
- Failed and successful logon attempts were reviewed  
- Suspicious processes were identified and correlated with login timestamps  
- No persistence mechanisms were found / persistence was identified  
- No data exfiltration observed / exfil indicators present  

---

## 🛡 Containment Actions
- Isolated host from network  
- Forced password reset  
- Terminated malicious processes  
- Blocked malicious IPs/domains  

---

## 🔧 Remediation
- Patch vulnerable software  
- Harden RDP / disable if unnecessary  
- Review user permissions  
- Improve logging coverage  

---

## 📚 MITRE ATT&CK Mapping
- **Initial Access:** T1078 – Valid Accounts  
- **Execution:** T1059 – Command Execution  
- **Persistence:** T1053 – Scheduled Task (if applicable)  

---

## 📝 Conclusion
Unauthorized access attempts were detected and contained. No confirmed compromise was identified, but hardening steps are recommended to reduce future risk.