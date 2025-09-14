# Phishing Analysis (Greenholt Case Study)

## Category  
📂 Defensive Security → Email Security  

## Objective  
Analyze a phishing campaign to identify indicators, understand attacker methods, and determine mitigation strategies.  

## Tools/Skills Practiced  
- Email header analysis  
- Identifying phishing URLs and payloads  
- VirusTotal / Urlscan.io for file and URL analysis  
- Mapping phishing TTPs to MITRE ATT&CK  

## Process (Steps Taken)  
1. Opened phishing email in Thunderbird Mail.  
2. Extracted subject, sender, and attachment details.  
3. Analyzed email headers (Return-Path, Reply-To, originating IP).  
4. Used OSINT tools (VirusTotal, MXToolbox, WHOIS) to validate indicators.  
5. Traced campaign TTPs back to MITRE ATT&CK (T1566 - Phishing).  

## Key Findings  
- Subject line included suspicious reference number (`09674321`).  
- Spoofed sender: *Mr. James Jackson* (`info@mutawamarine.com`).  
- Reply-To resolved to malicious IP (`192.119.71.157` → Hostwinds LLC).  
- Attachment: `SWT_#09674321____PDF__.CAB` (actual extension = RAR).  
- File hash (SHA256): `2e91c533615a9bb8929ac4bb76707b2444597ce063d84a4b33525e25074fff3f`.  
- File size: `400.26 KB`.  

## Screenshots (recommended)  
*(Insert screenshots of Thunderbird email, header source, and VirusTotal analysis here)*  

## Outcome / What I Learned  
- Improved ability to analyze phishing attempts and extract IoCs.  
- Learned how to verify suspicious email headers and attachments.  
- Practiced applying threat intel tools to real phishing campaigns.  
