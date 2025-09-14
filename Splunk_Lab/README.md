# Snort Lab

## Objective
Use Snort IDS rules to detect and alert on malicious activity within packet captures.

---

## Findings

### 1. Exploit Attempt
- **Observation:** Snort alert triggered for suspicious traffic matching exploit patterns.  
- **Tool:** Snort (rule-based detection on pcap)  
- **Details:** Detected payload activity resembling **buffer overflow / shellcode injection**.  

---

### 2. Weaponization
- **Observation:** Custom Snort rule matched exploit payloads in traffic.  
- **Rule Example:**  
  ```snort
  alert ip any any -> any any (msg:"Suspicious IP ID"; id:35369; sid:100001;)
