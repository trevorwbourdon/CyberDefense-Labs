# Wireshark Lab

## Objective
Analyze packet captures to detect malicious activity and understand attack patterns.

---

## Findings

### 1. Suspicious Network Traffic
- **Observation:** Malicious IP connection detected.  
- **Tool:** Wireshark (pcap analysis)  
- **Details:** Identified communication with suspicious external IP addresses, consistent with command-and-control (C2) traffic.  

---

### 2. Exploit Detection
- **Observation:** Packet payloads suggested an **exploit attempt**.  
- **Tool:** Wireshark (deep packet inspection)  
- **Details:** Detected abnormal payload size and suspicious shellcode-like data.

---

### 3. Indicators of Compromise (IOCs)
- **IP Addresses:** [example IPs you found]  
- **Ports:** 4444 / 5555 (commonly used for Metasploit reverse shells)  
- **Protocol:** TCP  

---

## Conclusion
Wireshark analysis revealed network-based malicious activity, including suspicious port usage (4444/5555) tied to Metasploit exploitation.  
This lab demonstrated how packet captures can be leveraged to detect early signs of compromise.
