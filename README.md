# vunerability-scan-report
i have run the vunerability scan 
# 🔍 Vulnerability Review Summary

**Tool Used:** Nessus Essentials  
**Scan Type:** Host Discovery Scan  
**Report:** `My Host Discovery Scan_6j4ror.html`

## 🧾 Overview
The host discovery scan identified active hosts and potential open ports. No critical exploitable vulnerabilities were detected, but several configuration weaknesses and exposure points were noted.

## ⚠️ Detected Vulnerabilities
| Vulnerability | Severity | Description | Recommended Fix |
|----------------|-----------|--------------|-----------------|
| **Ping/ICMP Response Enabled** | Low | Host responded to ICMP echo requests, revealing presence to attackers. | Disable ICMP response in firewall settings or restrict to trusted networks. |
| **Open TCP Port(s) Detected** | Medium | Unused or unprotected ports can allow unauthorized access or fingerprinting. | Review and close unnecessary ports. Implement firewall rules and access control. |
| **No SSL/TLS Detected (on some services)** | Medium | Some services run without encryption, exposing credentials/data. | Enable HTTPS or TLS-based communication where possible. |
| **Default or Generic Hostnames** | Low | Default hostnames can help attackers identify systems or OS versions. | Change to unique identifiers. |
| **Unidentified Operating System Fingerprint** | Info | Host OS was guessed via network fingerprinting. | Consider using OS obfuscation or segmentation. |

## 🧩 Severity Summary
| Level | Count | Description |
|-------|--------|-------------|
| **Critical** | 0 | Immediate exploitation possible |
| **High** | 0 | Significant risk, needs patching |
| **Medium** | 2 | Potential exposure, needs configuration fix |
| **Low** | 2 | Minor information disclosure |
| **Informational** | 1 | For awareness and improvement |

## 🛠️ Mitigations
- **Patch management:** Regularly update all OS and services.
- **Firewall hardening:** Restrict inbound traffic to necessary ports only.
- **Network segmentation:** Limit broadcast and scanning reach.
- **TLS Enforcement:** Use HTTPS or encrypted protocols across all hosts.
- **Monitoring:** Enable IDS/IPS to detect further scanning or probing activity.

## 📄 Notes
This report serves as an initial **network exposure assessment**, not a full vulnerability audit.  
A follow-up **credentialed scan** is recommended for detailed security posture evaluation.
<img width="338" height="437" alt="Screenshot 2025-06-16 111937" src="https://github.com/user-attachments/assets/5266640f-c8c3-4d3f-9ba9-2ea8935948f9" />
<img width="645" height="662" alt="Screenshot 2025-06-16 111952" src="https://github.com/user-attachments/assets/09f68267-0294-4d18-8a40-929370360ed6" />
<img width="629" height="510" alt="Screenshot 2025-06-16 111924" src="https://github.com/user-attachments/assets/d33434ab-3263-4a44-93c3-c9b62bf2eee1" />
<img width="477" height="93" alt="Screenshot 2025-06-16 111914" src="https://github.com/user-attachments/assets/0bc9f5e2-e9bd-4262-8bd1-c05638b19e9b" />
<img width="477" height="93" alt="Screenshot 2025-06-16 111914" src="https://github.com/user-attachments/assets/d8235f26-2b37-401f-a39f-4491e2a94680" />
<img width="1918" height="1079" alt="Screenshot 2025-10-25 193446" src="https://github.com/user-attachments/assets/9636a3ac-c035-4490-8e41-b4d63d49ec81" />
