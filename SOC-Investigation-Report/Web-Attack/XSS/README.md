# 🔍 SOC Investigation: XSS Attack Attempt

## 📖 Overview
This project documents a real-world SOC investigation involving a suspected Cross-Site Scripting (XSS) attack detected through a SIEM alert.

The analysis was performed using LetsDefend, focusing on log analysis, HTTP traffic inspection, and attack validation.

---

## 🚨 Alert Details
- Event ID: 116
- Rule: JavaScript Code Detected in Requested URL
- Severity: Medium
- Category: Web Attack (XSS)

---

## 🌐 Key Findings
- External IP attempted multiple XSS payload injections
- Traffic direction: Internet → Internal Network
- Payloads included script injection, SVG, and event-based execution
- Server responded with HTTP 302 and no content for malicious requests
- No evidence of payload execution or compromise

---

## ✅ Conclusion
The alert was validated as a **True Positive**, representing an **unsuccessful XSS attack attempt**.

---

## 📂 Report
The full investigation report is available here:

👉 [View PDF Report](XSS_Attack_Investigation_Report.pdf)

---

## 🛠️ Skills Demonstrated
- Log Analysis
- Web Attack Detection (XSS)
- HTTP Traffic Analysis
- Incident Classification
- SOC Decision-Making

---

## 📌 Notes
This case highlights the importance of distinguishing between attack attempts and successful exploitation using HTTP response analysis.
