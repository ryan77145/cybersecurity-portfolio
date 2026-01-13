# Failed RDP Brute Force Investigation

## 📌 Summary
This investigation analyzes a series of failed Remote Desktop Protocol (RDP) login attempts originating from a suspicious external IP address. The goal is to determine whether the activity represents a brute-force attack and identify recommended response actions.

---

## 🔍 Alert Details
- **Alert Type:** Multiple Failed RDP Logins  
- **Source:** SIEM (generic)  
- **Severity:** Medium  
- **Date/Time:** <Insert date/time>  
- **Detection Logic:** Excessive failed logins from a single external IP within a short time window  

---

## 🧪 Evidence Collected
### Event Logs Reviewed
- Windows Security Log (Event ID 4625 – Failed Logon)
- Network firewall logs (if available)

### Key Fields Observed
- **Target Username:** <insert>  
- **Source IP:** <insert>  
- **Failure Reason:** Unknown username / bad password  
- **Logon Type:** 10 (RemoteInteractive)  

---

## 🧠 Analysis
- The source IP attempted multiple logins in rapid succession.  
- Username attempts appear to be common/default accounts.  
- No successful logins were observed.  
- Behavior is consistent with automated brute-force activity.  

---

## 🛡 Recommended Response
- Block the source IP at the firewall  
- Enforce account lockout policies  
- Enable MFA for remote access  
- Review RDP exposure (consider VPN-only access)  

---

## 📚 MITRE ATT&CK Mapping
- **Technique:** T1110 – Brute Force  
- **Sub-technique:** T1110.001 – Password Guessing  

---

## 📝 Conclusion
The activity represents a brute-force attempt against exposed RDP services. No compromise was identified, but preventative hardening is recommended to reduce future risk.