# Phishing Email Investigation

## 📌 Summary
This investigation analyzes a suspicious email reported by a user. The goal is to determine whether the email is malicious, identify indicators of compromise, and recommend appropriate response actions.

---

## 📥 Email Overview
- **Sender:** <insert>  
- **Recipient:** <insert>  
- **Subject:** <insert>  
- **Date/Time Received:** <insert>  
- **User Report Reason:** <insert>  

---

## 🧪 Evidence Collected
### Email Header Analysis
- **Return-Path:** <insert>  
- **Received From:** <insert>  
- **SPF:** Pass / Fail  
- **DKIM:** Pass / Fail  
- **DMARC:** Pass / Fail  

### Body Analysis
- Suspicious links  
- Urgent language  
- Credential harvesting attempts  
- Attachments (if any)  

### URL / Link Inspection
- **Displayed URL:** <insert>  
- **Actual URL:** <insert>  
- **Reputation Check:** (VirusTotal / URLScan)  
- **Domain Age:** <insert>  

---

## 🧠 Analysis
- The sender domain does/does not match the organization  
- Authentication checks failed/passed  
- The link redirects to a suspicious login page  
- Language indicates social engineering (urgency, threats, rewards)  
- Indicators align with credential harvesting attempts  

---

## 🛡 Recommended Response
- Block sender domain  
- Block malicious URL  
- Reset affected user credentials (if clicked)  
- Notify users of similar phishing attempts  
- Update email filtering rules  

---

## 📚 MITRE ATT&CK Mapping
- **Technique:** T1566 – Phishing  
- **Sub-technique:** T1566.002 – Spearphishing Link  

---

## 📝 Conclusion
The email is confirmed to be malicious and designed to harvest credentials. No compromise was identified, but preventative measures and user awareness are recommended.