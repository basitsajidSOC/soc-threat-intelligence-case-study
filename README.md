# soc-threat-intelligence-case-study
A hands-on SOC case study case study documenting multi-tool URL and file hash triage using MalwareBazaar ,Virus Total and Cisco Talos Intelligence.
#Project #2: Multi-Tool Threat Intelligence & Artifact Triage
1. Objective
To perform manual threat intelligence and reputation analysis on unknown or suspicious digital artifacts (URLs and sample hashes) using industry-standard security tools, simulating a real-world SOC triage workflow.
2. Artifact Details
Source Platform: MalwareBazaar (Abuse.ch)  
Target Sample/URL: [https://bazaar.abuse.ch/sample/48c44475627d37aa1d2057df21bb6e32f5abe09249ac43ff52f42b9e481aa1a/](https://bazaar.abuse.ch/sample/48c44475627d37aa1d2057df21bb6e32f5abe09249ac43ff52f42b9e481aa1a/)  
Artifact Type: Malware Sample Repository Link / SHA256 Hash Lookup
3. Investigation Steps & Tool Analysis
Step 1: Domain & Web Reputation Check (Cisco Talos Intelligence)
Action: Queried the hosting domain (bazaar.abuse.ch) on Cisco Talos to evaluate infrastructure safety.  
Findings: The web reputation was rated as Favorable, and it was not listed on the Talos Security Intelligence Block List. It was correctly categorized under "Computer Security" as a legitimate research portal.  
Step 2: Multi-Vendor Cross-Reference (VirusTotal URL Analysis)
Action: Scanned the sample URL through VirusTotal's scanning engine.  
Findings: Cross-referenced with global security vendors and community indicators to verify that the sample link points to a known threat intelligence repository context without active malicious web injections on the landing page.  
4. Conclusion & Analyst Verdict
Verdict: The target URL belongs to a trusted open-source threat intelligence database (Abuse.ch MalwareBazaar) utilized by security analysts for malware research. While the underlying file hash points to a malicious sample, the hosting infrastructure itself is verified as a legitimate security resource.
