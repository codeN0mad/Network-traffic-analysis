

# 🕵️‍♀️ Network Traffic Analysis

*A project by Uneeq Interns*

## 📌 Project Overview

This project focuses on **capturing and analyzing network traffic** to study connectivity, protocol behavior, and communication patterns. Using **Wireshark** and **Linux command-line tools** (e.g., `tcpdump`, `dig`, `netcat`), we investigated both **normal** and **suspicious** traffic, providing insights for **network performance monitoring** and **security hardening**.

---

## 🎯 Objectives

* Capture and analyze live network traffic.
* Check connectivity and detect issues.
* Study protocol behavior and functions.
* Identify anomalies and potential threats.

---

## ⚙️ Tools & Techniques

* **Traffic Capture:** `tcpdump`
* **Traffic Generation:** ICMP requests, DNS lookups, TCP connectivity tests
* **Traffic Analysis:** Wireshark filters (`http`, `icmp`, `dns`, `tcp.port==8080`, `tcp.flags.syn==1 && tcp.flags.ack==0`)
* **Protocols Studied:** TCP, HTTP, ICMP, DNS

---

## 🔎 Key Findings

* **Unusual TCP SYN Traffic:** Multiple SYN packets on port 8080 from unknown IPs → possible scanning/probing.
* **Suspicious HTTP Requests:** Requests to unrecognized hostnames → potential phishing/malware activity.
* **Repeated ICMP Requests:** Excessive pings from a single external IP → possible reconnaissance attempt.

---

## 🛡️ Recommendations

* Block unused/non-essential ports (e.g., unsolicited SYN packets).
* Enable **DNS filtering** to block suspicious domain resolution.
* Restrict **ICMP traffic** to trusted sources only.
* Regularly monitor traffic with **tcpdump/Wireshark**.
* Keep **IDS/IPS rules updated** for better detection.

---

## ✅ Conclusion

This analysis successfully distinguished between **normal** and **potentially malicious** traffic patterns. Proactive monitoring and implementing the recommended security measures can significantly improve **network resilience** and **threat protection**.

---



Would you like me to also make this **GitHub-ready with badges** (e.g., Wireshark, Linux, Security tags) and maybe add a **"How to Reproduce" section** with commands so others can replicate your analysis?

