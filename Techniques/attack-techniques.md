---
ATT&CK Version: v18.1
Total Techniques: 691 (216 parent, 475 sub-techniques)
Author: jasonlayton.com
---

# MITRE ATT&CK Enterprise — Technique Reference

## Table of Contents

1. [Summary Statistics](#summary-statistics)
2. [Master Technique Table](#master-technique-table)
3. [Techniques by Tactic](#techniques-by-tactic)

---

## Summary Statistics

| Tactic | Technique Count |
|--------|----------------:|
| Defense Evasion | 215 |
| Persistence | 126 |
| Privilege Escalation | 109 |
| Credential Access | 67 |
| Discovery | 49 |
| Resource Development | 47 |
| Execution | 46 |
| Command And Control | 45 |
| Reconnaissance | 45 |
| Collection | 41 |
| Impact | 33 |
| Lateral Movement | 23 |
| Initial Access | 22 |
| Exfiltration | 19 |

> **Note:** Techniques can map to multiple tactics, so the sum of tactic counts will exceed the total unique technique count.

---

## Master Technique Table

| T-Code | Name | Tactics | Platforms |
|--------|------|---------|-----------|
| [T1001](https://attack.mitre.org/techniques/T1001) | Data Obfuscation | Command And Control | ESXi, Linux, macOS, Windows |
| [T1001.001](https://attack.mitre.org/techniques/T1001/001) | Junk Data | Command And Control | ESXi, Linux, macOS, Windows |
| [T1001.002](https://attack.mitre.org/techniques/T1001/002) | Steganography | Command And Control | Linux, macOS, Windows, ESXi |
| [T1001.003](https://attack.mitre.org/techniques/T1001/003) | Protocol or Service Impersonation | Command And Control | ESXi, Linux, macOS, Windows |
| [T1003](https://attack.mitre.org/techniques/T1003) | OS Credential Dumping | Credential Access | Linux, macOS, Windows |
| [T1003.001](https://attack.mitre.org/techniques/T1003/001) | LSASS Memory | Credential Access | Windows |
| [T1003.002](https://attack.mitre.org/techniques/T1003/002) | Security Account Manager | Credential Access | Windows |
| [T1003.003](https://attack.mitre.org/techniques/T1003/003) | NTDS | Credential Access | Windows |
| [T1003.004](https://attack.mitre.org/techniques/T1003/004) | LSA Secrets | Credential Access | Windows |
| [T1003.005](https://attack.mitre.org/techniques/T1003/005) | Cached Domain Credentials | Credential Access | Windows, Linux |
| [T1003.006](https://attack.mitre.org/techniques/T1003/006) | DCSync | Credential Access | Windows |
| [T1003.007](https://attack.mitre.org/techniques/T1003/007) | Proc Filesystem | Credential Access | Linux |
| [T1003.008](https://attack.mitre.org/techniques/T1003/008) | /etc/passwd and /etc/shadow | Credential Access | Linux |
| [T1005](https://attack.mitre.org/techniques/T1005) | Data from Local System | Collection | ESXi, Linux, macOS, Network Devices, Windows |
| [T1006](https://attack.mitre.org/techniques/T1006) | Direct Volume Access | Defense Evasion | Network Devices, Windows |
| [T1007](https://attack.mitre.org/techniques/T1007) | System Service Discovery | Discovery | Linux, macOS, Windows |
| [T1008](https://attack.mitre.org/techniques/T1008) | Fallback Channels | Command And Control | Linux, Windows, macOS, ESXi |
| [T1010](https://attack.mitre.org/techniques/T1010) | Application Window Discovery | Discovery | Linux, Windows, macOS |
| [T1011](https://attack.mitre.org/techniques/T1011) | Exfiltration Over Other Network Medium | Exfiltration | Linux, macOS, Windows |
| [T1011.001](https://attack.mitre.org/techniques/T1011/001) | Exfiltration Over Bluetooth | Exfiltration | Linux, macOS, Windows |
| [T1012](https://attack.mitre.org/techniques/T1012) | Query Registry | Discovery | Windows |
| [T1014](https://attack.mitre.org/techniques/T1014) | Rootkit | Defense Evasion | Linux, macOS, Windows |
| [T1016](https://attack.mitre.org/techniques/T1016) | System Network Configuration Discovery | Discovery | ESXi, Linux, macOS, Network Devices, Windows |
| [T1016.001](https://attack.mitre.org/techniques/T1016/001) | Internet Connection Discovery | Discovery | Windows, Linux, macOS, ESXi |
| [T1016.002](https://attack.mitre.org/techniques/T1016/002) | Wi-Fi Discovery | Discovery | Linux, Windows, macOS |
| [T1018](https://attack.mitre.org/techniques/T1018) | Remote System Discovery | Discovery | ESXi, Linux, macOS, Network Devices, Windows |
| [T1020](https://attack.mitre.org/techniques/T1020) | Automated Exfiltration | Exfiltration | Linux, macOS, Network Devices, Windows |
| [T1020.001](https://attack.mitre.org/techniques/T1020/001) | Traffic Duplication | Exfiltration | Network Devices, IaaS |
| [T1021](https://attack.mitre.org/techniques/T1021) | Remote Services | Lateral Movement | Linux, macOS, Windows, IaaS, ESXi |
| [T1021.001](https://attack.mitre.org/techniques/T1021/001) | Remote Desktop Protocol | Lateral Movement | Windows |
| [T1021.002](https://attack.mitre.org/techniques/T1021/002) | SMB/Windows Admin Shares | Lateral Movement | Windows |
| [T1021.003](https://attack.mitre.org/techniques/T1021/003) | Distributed Component Object Model | Lateral Movement | Windows |
| [T1021.004](https://attack.mitre.org/techniques/T1021/004) | SSH | Lateral Movement | ESXi, Linux, macOS |
| [T1021.005](https://attack.mitre.org/techniques/T1021/005) | VNC | Lateral Movement | Linux, Windows, macOS |
| [T1021.006](https://attack.mitre.org/techniques/T1021/006) | Windows Remote Management | Lateral Movement | Windows |
| [T1021.007](https://attack.mitre.org/techniques/T1021/007) | Cloud Services | Lateral Movement | IaaS, Identity Provider, Office Suite, SaaS |
| [T1021.008](https://attack.mitre.org/techniques/T1021/008) | Direct Cloud VM Connections | Lateral Movement | IaaS |
| [T1025](https://attack.mitre.org/techniques/T1025) | Data from Removable Media | Collection | Linux, macOS, Windows |
| [T1027](https://attack.mitre.org/techniques/T1027) | Obfuscated Files or Information | Defense Evasion | ESXi, Linux, macOS, Network Devices, Windows |
| [T1027.001](https://attack.mitre.org/techniques/T1027/001) | Binary Padding | Defense Evasion | Linux, Windows, macOS |
| [T1027.002](https://attack.mitre.org/techniques/T1027/002) | Software Packing | Defense Evasion | Linux, macOS, Windows |
| [T1027.003](https://attack.mitre.org/techniques/T1027/003) | Steganography | Defense Evasion | Linux, macOS, Windows |
| [T1027.004](https://attack.mitre.org/techniques/T1027/004) | Compile After Delivery | Defense Evasion | Linux, macOS, Windows |
| [T1027.005](https://attack.mitre.org/techniques/T1027/005) | Indicator Removal from Tools | Defense Evasion | Linux, macOS, Windows |
| [T1027.006](https://attack.mitre.org/techniques/T1027/006) | HTML Smuggling | Defense Evasion | Windows, Linux, macOS |
| [T1027.007](https://attack.mitre.org/techniques/T1027/007) | Dynamic API Resolution | Defense Evasion | Windows |
| [T1027.008](https://attack.mitre.org/techniques/T1027/008) | Stripped Payloads | Defense Evasion | macOS, Linux, Windows, Network Devices |
| [T1027.009](https://attack.mitre.org/techniques/T1027/009) | Embedded Payloads | Defense Evasion | Linux, macOS, Windows |
| [T1027.010](https://attack.mitre.org/techniques/T1027/010) | Command Obfuscation | Defense Evasion | Linux, macOS, Windows |
| [T1027.011](https://attack.mitre.org/techniques/T1027/011) | Fileless Storage | Defense Evasion | Windows, Linux |
| [T1027.012](https://attack.mitre.org/techniques/T1027/012) | LNK Icon Smuggling | Defense Evasion | Windows |
| [T1027.013](https://attack.mitre.org/techniques/T1027/013) | Encrypted/Encoded File | Defense Evasion | Linux, macOS, Windows |
| [T1027.014](https://attack.mitre.org/techniques/T1027/014) | Polymorphic Code | Defense Evasion | Windows, macOS, Linux |
| [T1027.015](https://attack.mitre.org/techniques/T1027/015) | Compression | Defense Evasion | Linux, Windows, macOS |
| [T1027.016](https://attack.mitre.org/techniques/T1027/016) | Junk Code Insertion | Defense Evasion | Linux, macOS, Windows |
| [T1027.017](https://attack.mitre.org/techniques/T1027/017) | SVG Smuggling | Defense Evasion | Linux, macOS, Windows |
| [T1029](https://attack.mitre.org/techniques/T1029) | Scheduled Transfer | Exfiltration | Linux, macOS, Windows |
| [T1030](https://attack.mitre.org/techniques/T1030) | Data Transfer Size Limits | Exfiltration | Linux, macOS, Windows, ESXi |
| [T1033](https://attack.mitre.org/techniques/T1033) | System Owner/User Discovery | Discovery | Linux, macOS, Network Devices, Windows |
| [T1036](https://attack.mitre.org/techniques/T1036) | Masquerading | Defense Evasion | Containers, ESXi, Linux, macOS, Windows |
| [T1036.001](https://attack.mitre.org/techniques/T1036/001) | Invalid Code Signature | Defense Evasion | Windows, macOS |
| [T1036.002](https://attack.mitre.org/techniques/T1036/002) | Right-to-Left Override | Defense Evasion | Linux, macOS, Windows |
| [T1036.003](https://attack.mitre.org/techniques/T1036/003) | Rename Legitimate Utilities | Defense Evasion | Linux, macOS, Windows |
| [T1036.004](https://attack.mitre.org/techniques/T1036/004) | Masquerade Task or Service | Defense Evasion | Linux, macOS, Windows |
| [T1036.005](https://attack.mitre.org/techniques/T1036/005) | Match Legitimate Resource Name or Location | Defense Evasion | Containers, ESXi, Linux, macOS, Windows |
| [T1036.006](https://attack.mitre.org/techniques/T1036/006) | Space after Filename | Defense Evasion | Linux, macOS |
| [T1036.007](https://attack.mitre.org/techniques/T1036/007) | Double File Extension | Defense Evasion | Windows |
| [T1036.008](https://attack.mitre.org/techniques/T1036/008) | Masquerade File Type | Defense Evasion | Linux, macOS, Windows |
| [T1036.009](https://attack.mitre.org/techniques/T1036/009) | Break Process Trees | Defense Evasion | Linux, macOS |
| [T1036.010](https://attack.mitre.org/techniques/T1036/010) | Masquerade Account Name | Defense Evasion | Linux, macOS, Windows, SaaS, IaaS, Containers, Office Suite, Identity Provider |
| [T1036.011](https://attack.mitre.org/techniques/T1036/011) | Overwrite Process Arguments | Defense Evasion | Linux |
| [T1036.012](https://attack.mitre.org/techniques/T1036/012) | Browser Fingerprint | Defense Evasion | Linux, macOS, Windows |
| [T1037](https://attack.mitre.org/techniques/T1037) | Boot or Logon Initialization Scripts | Persistence, Privilege Escalation | macOS, Windows, Linux, Network Devices, ESXi |
| [T1037.001](https://attack.mitre.org/techniques/T1037/001) | Logon Script (Windows) | Persistence, Privilege Escalation | Windows |
| [T1037.002](https://attack.mitre.org/techniques/T1037/002) | Login Hook | Persistence, Privilege Escalation | macOS |
| [T1037.003](https://attack.mitre.org/techniques/T1037/003) | Network Logon Script | Persistence, Privilege Escalation | Windows |
| [T1037.004](https://attack.mitre.org/techniques/T1037/004) | RC Scripts | Persistence, Privilege Escalation | macOS, Linux, Network Devices, ESXi |
| [T1037.005](https://attack.mitre.org/techniques/T1037/005) | Startup Items | Persistence, Privilege Escalation | macOS |
| [T1039](https://attack.mitre.org/techniques/T1039) | Data from Network Shared Drive | Collection | Linux, macOS, Windows |
| [T1040](https://attack.mitre.org/techniques/T1040) | Network Sniffing | Credential Access, Discovery | Linux, macOS, Windows, Network Devices, IaaS |
| [T1041](https://attack.mitre.org/techniques/T1041) | Exfiltration Over C2 Channel | Exfiltration | ESXi, Linux, macOS, Windows |
| [T1046](https://attack.mitre.org/techniques/T1046) | Network Service Discovery | Discovery | Containers, IaaS, Linux, macOS, Network Devices, Windows |
| [T1047](https://attack.mitre.org/techniques/T1047) | Windows Management Instrumentation | Execution | Windows |
| [T1048](https://attack.mitre.org/techniques/T1048) | Exfiltration Over Alternative Protocol | Exfiltration | ESXi, IaaS, Linux, macOS, Network Devices, Office Suite, SaaS, Windows |
| [T1048.001](https://attack.mitre.org/techniques/T1048/001) | Exfiltration Over Symmetric Encrypted Non-C2 Protocol | Exfiltration | Linux, macOS, Windows, ESXi |
| [T1048.002](https://attack.mitre.org/techniques/T1048/002) | Exfiltration Over Asymmetric Encrypted Non-C2 Protocol | Exfiltration | Linux, macOS, Windows, ESXi |
| [T1048.003](https://attack.mitre.org/techniques/T1048/003) | Exfiltration Over Unencrypted Non-C2 Protocol | Exfiltration | ESXi, Linux, macOS, Network Devices, Windows |
| [T1049](https://attack.mitre.org/techniques/T1049) | System Network Connections Discovery | Discovery | Windows, IaaS, Linux, macOS, Network Devices, ESXi |
| [T1052](https://attack.mitre.org/techniques/T1052) | Exfiltration Over Physical Medium | Exfiltration | Linux, macOS, Windows |
| [T1052.001](https://attack.mitre.org/techniques/T1052/001) | Exfiltration over USB | Exfiltration | Linux, Windows, macOS |
| [T1053](https://attack.mitre.org/techniques/T1053) | Scheduled Task/Job | Execution, Persistence, Privilege Escalation | Windows, Linux, macOS, Containers, ESXi |
| [T1053.002](https://attack.mitre.org/techniques/T1053/002) | At | Execution, Persistence, Privilege Escalation | Windows, Linux, macOS |
| [T1053.003](https://attack.mitre.org/techniques/T1053/003) | Cron | Execution, Persistence, Privilege Escalation | Linux, macOS, ESXi |
| [T1053.005](https://attack.mitre.org/techniques/T1053/005) | Scheduled Task | Execution, Persistence, Privilege Escalation | Windows |
| [T1053.006](https://attack.mitre.org/techniques/T1053/006) | Systemd Timers | Execution, Persistence, Privilege Escalation | Linux |
| [T1053.007](https://attack.mitre.org/techniques/T1053/007) | Container Orchestration Job | Execution, Persistence, Privilege Escalation | Containers |
| [T1055](https://attack.mitre.org/techniques/T1055) | Process Injection | Defense Evasion, Privilege Escalation | Linux, macOS, Windows |
| [T1055.001](https://attack.mitre.org/techniques/T1055/001) | Dynamic-link Library Injection | Defense Evasion, Privilege Escalation | Windows |
| [T1055.002](https://attack.mitre.org/techniques/T1055/002) | Portable Executable Injection | Defense Evasion, Privilege Escalation | Windows |
| [T1055.003](https://attack.mitre.org/techniques/T1055/003) | Thread Execution Hijacking | Defense Evasion, Privilege Escalation | Windows |
| [T1055.004](https://attack.mitre.org/techniques/T1055/004) | Asynchronous Procedure Call | Defense Evasion, Privilege Escalation | Windows |
| [T1055.005](https://attack.mitre.org/techniques/T1055/005) | Thread Local Storage | Defense Evasion, Privilege Escalation | Windows |
| [T1055.008](https://attack.mitre.org/techniques/T1055/008) | Ptrace System Calls | Defense Evasion, Privilege Escalation | Linux |
| [T1055.009](https://attack.mitre.org/techniques/T1055/009) | Proc Memory | Defense Evasion, Privilege Escalation | Linux |
| [T1055.011](https://attack.mitre.org/techniques/T1055/011) | Extra Window Memory Injection | Defense Evasion, Privilege Escalation | Windows |
| [T1055.012](https://attack.mitre.org/techniques/T1055/012) | Process Hollowing | Defense Evasion, Privilege Escalation | Windows |
| [T1055.013](https://attack.mitre.org/techniques/T1055/013) | Process Doppelgänging | Defense Evasion, Privilege Escalation | Windows |
| [T1055.014](https://attack.mitre.org/techniques/T1055/014) | VDSO Hijacking | Defense Evasion, Privilege Escalation | Linux |
| [T1055.015](https://attack.mitre.org/techniques/T1055/015) | ListPlanting | Defense Evasion, Privilege Escalation | Windows |
| [T1056](https://attack.mitre.org/techniques/T1056) | Input Capture | Collection, Credential Access | Linux, macOS, Network Devices, Windows |
| [T1056.001](https://attack.mitre.org/techniques/T1056/001) | Keylogging | Collection, Credential Access | Linux, macOS, Network Devices, Windows |
| [T1056.002](https://attack.mitre.org/techniques/T1056/002) | GUI Input Capture | Collection, Credential Access | macOS, Windows, Linux |
| [T1056.003](https://attack.mitre.org/techniques/T1056/003) | Web Portal Capture | Collection, Credential Access | Linux, macOS, Windows |
| [T1056.004](https://attack.mitre.org/techniques/T1056/004) | Credential API Hooking | Collection, Credential Access | Windows, Linux, macOS |
| [T1057](https://attack.mitre.org/techniques/T1057) | Process Discovery | Discovery | ESXi, Linux, macOS, Network Devices, Windows |
| [T1059](https://attack.mitre.org/techniques/T1059) | Command and Scripting Interpreter | Execution | ESXi, IaaS, Identity Provider, Linux, macOS, Network Devices, Office Suite, Windows |
| [T1059.001](https://attack.mitre.org/techniques/T1059/001) | PowerShell | Execution | Windows |
| [T1059.002](https://attack.mitre.org/techniques/T1059/002) | AppleScript | Execution | macOS |
| [T1059.003](https://attack.mitre.org/techniques/T1059/003) | Windows Command Shell | Execution | Windows |
| [T1059.004](https://attack.mitre.org/techniques/T1059/004) | Unix Shell | Execution | ESXi, Linux, macOS, Network Devices |
| [T1059.005](https://attack.mitre.org/techniques/T1059/005) | Visual Basic | Execution | Linux, macOS, Windows |
| [T1059.006](https://attack.mitre.org/techniques/T1059/006) | Python | Execution | ESXi, Linux, macOS, Windows |
| [T1059.007](https://attack.mitre.org/techniques/T1059/007) | JavaScript | Execution | Linux, macOS, Windows |
| [T1059.008](https://attack.mitre.org/techniques/T1059/008) | Network Device CLI | Execution | Network Devices |
| [T1059.009](https://attack.mitre.org/techniques/T1059/009) | Cloud API | Execution | IaaS, Identity Provider, Office Suite, SaaS |
| [T1059.010](https://attack.mitre.org/techniques/T1059/010) | AutoHotKey & AutoIT | Execution | Windows |
| [T1059.011](https://attack.mitre.org/techniques/T1059/011) | Lua | Execution | Linux, Network Devices, Windows, macOS |
| [T1059.012](https://attack.mitre.org/techniques/T1059/012) | Hypervisor CLI | Execution | ESXi |
| [T1059.013](https://attack.mitre.org/techniques/T1059/013) | Container CLI/API | Execution | Containers |
| [T1068](https://attack.mitre.org/techniques/T1068) | Exploitation for Privilege Escalation | Privilege Escalation | Containers, Linux, macOS, Windows |
| [T1069](https://attack.mitre.org/techniques/T1069) | Permission Groups Discovery | Discovery | Containers, IaaS, Identity Provider, Linux, macOS, Office Suite, SaaS, Windows |
| [T1069.001](https://attack.mitre.org/techniques/T1069/001) | Local Groups | Discovery | Linux, macOS, Windows |
| [T1069.002](https://attack.mitre.org/techniques/T1069/002) | Domain Groups | Discovery | Linux, macOS, Windows |
| [T1069.003](https://attack.mitre.org/techniques/T1069/003) | Cloud Groups | Discovery | SaaS, IaaS, Office Suite, Identity Provider |
| [T1070](https://attack.mitre.org/techniques/T1070) | Indicator Removal | Defense Evasion | Containers, ESXi, Linux, macOS, Network Devices, Office Suite, Windows |
| [T1070.001](https://attack.mitre.org/techniques/T1070/001) | Clear Windows Event Logs | Defense Evasion | Windows |
| [T1070.002](https://attack.mitre.org/techniques/T1070/002) | Clear Linux or Mac System Logs | Defense Evasion | Linux, macOS |
| [T1070.003](https://attack.mitre.org/techniques/T1070/003) | Clear Command History | Defense Evasion | ESXi, Linux, macOS, Network Devices, Windows |
| [T1070.004](https://attack.mitre.org/techniques/T1070/004) | File Deletion | Defense Evasion | ESXi, Linux, macOS, Windows |
| [T1070.005](https://attack.mitre.org/techniques/T1070/005) | Network Share Connection Removal | Defense Evasion | Windows |
| [T1070.006](https://attack.mitre.org/techniques/T1070/006) | Timestomp | Defense Evasion | ESXi, Linux, macOS, Windows |
| [T1070.007](https://attack.mitre.org/techniques/T1070/007) | Clear Network Connection History and Configurations | Defense Evasion | Linux, macOS, Windows, Network Devices |
| [T1070.008](https://attack.mitre.org/techniques/T1070/008) | Clear Mailbox Data | Defense Evasion | Linux, macOS, Office Suite, Windows |
| [T1070.009](https://attack.mitre.org/techniques/T1070/009) | Clear Persistence | Defense Evasion | ESXi, Linux, Windows, macOS |
| [T1070.010](https://attack.mitre.org/techniques/T1070/010) | Relocate Malware | Defense Evasion | Linux, macOS, Windows, Network Devices |
| [T1071](https://attack.mitre.org/techniques/T1071) | Application Layer Protocol | Command And Control | Linux, macOS, Windows, Network Devices, ESXi |
| [T1071.001](https://attack.mitre.org/techniques/T1071/001) | Web Protocols | Command And Control | ESXi, Linux, macOS, Network Devices, Windows |
| [T1071.002](https://attack.mitre.org/techniques/T1071/002) | File Transfer Protocols | Command And Control | ESXi, Linux, macOS, Network Devices, Windows |
| [T1071.003](https://attack.mitre.org/techniques/T1071/003) | Mail Protocols | Command And Control | Linux, macOS, Network Devices, Windows |
| [T1071.004](https://attack.mitre.org/techniques/T1071/004) | DNS | Command And Control | Linux, macOS, Windows, Network Devices, ESXi |
| [T1071.005](https://attack.mitre.org/techniques/T1071/005) | Publish/Subscribe Protocols | Command And Control | macOS, Linux, Windows, Network Devices |
| [T1072](https://attack.mitre.org/techniques/T1072) | Software Deployment Tools | Execution, Lateral Movement | Linux, macOS, Network Devices, SaaS, Windows |
| [T1074](https://attack.mitre.org/techniques/T1074) | Data Staged | Collection | Windows, IaaS, Linux, macOS, ESXi |
| [T1074.001](https://attack.mitre.org/techniques/T1074/001) | Local Data Staging | Collection | ESXi, Linux, macOS, Windows |
| [T1074.002](https://attack.mitre.org/techniques/T1074/002) | Remote Data Staging | Collection | Windows, IaaS, Linux, macOS, ESXi |
| [T1078](https://attack.mitre.org/techniques/T1078) | Valid Accounts | Defense Evasion, Initial Access, Persistence, Privilege Escalation | Containers, ESXi, IaaS, Identity Provider, Linux, macOS, Network Devices, Office Suite, SaaS, Windows |
| [T1078.001](https://attack.mitre.org/techniques/T1078/001) | Default Accounts | Defense Evasion, Initial Access, Persistence, Privilege Escalation | Windows, SaaS, IaaS, Linux, macOS, Containers, Network Devices, Office Suite, Identity Provider, ESXi |
| [T1078.002](https://attack.mitre.org/techniques/T1078/002) | Domain Accounts | Defense Evasion, Initial Access, Persistence, Privilege Escalation | ESXi, Linux, macOS, Windows |
| [T1078.003](https://attack.mitre.org/techniques/T1078/003) | Local Accounts | Defense Evasion, Initial Access, Persistence, Privilege Escalation | Linux, macOS, Windows, Containers, Network Devices, ESXi |
| [T1078.004](https://attack.mitre.org/techniques/T1078/004) | Cloud Accounts | Defense Evasion, Initial Access, Persistence, Privilege Escalation | IaaS, Identity Provider, Office Suite, SaaS |
| [T1080](https://attack.mitre.org/techniques/T1080) | Taint Shared Content | Lateral Movement | Windows, SaaS, Linux, macOS, Office Suite |
| [T1082](https://attack.mitre.org/techniques/T1082) | System Information Discovery | Discovery | ESXi, IaaS, Linux, macOS, Network Devices, Windows |
| [T1083](https://attack.mitre.org/techniques/T1083) | File and Directory Discovery | Discovery | ESXi, Linux, macOS, Network Devices, Windows |
| [T1087](https://attack.mitre.org/techniques/T1087) | Account Discovery | Discovery | ESXi, IaaS, Identity Provider, Linux, macOS, Office Suite, SaaS, Windows |
| [T1087.001](https://attack.mitre.org/techniques/T1087/001) | Local Account | Discovery | ESXi, Linux, macOS, Windows |
| [T1087.002](https://attack.mitre.org/techniques/T1087/002) | Domain Account | Discovery | Linux, macOS, Windows |
| [T1087.003](https://attack.mitre.org/techniques/T1087/003) | Email Account | Discovery | Windows, Office Suite |
| [T1087.004](https://attack.mitre.org/techniques/T1087/004) | Cloud Account | Discovery | IaaS, Identity Provider, Office Suite, SaaS |
| [T1090](https://attack.mitre.org/techniques/T1090) | Proxy | Command And Control | ESXi, Linux, macOS, Network Devices, Windows |
| [T1090.001](https://attack.mitre.org/techniques/T1090/001) | Internal Proxy | Command And Control | Linux, Network Devices, Windows, macOS, ESXi |
| [T1090.002](https://attack.mitre.org/techniques/T1090/002) | External Proxy | Command And Control | ESXi, Linux, Network Devices, Windows, macOS |
| [T1090.003](https://attack.mitre.org/techniques/T1090/003) | Multi-hop Proxy | Command And Control | ESXi, Linux, macOS, Network Devices, Windows |
| [T1090.004](https://attack.mitre.org/techniques/T1090/004) | Domain Fronting | Command And Control | Linux, macOS, Windows, ESXi |
| [T1091](https://attack.mitre.org/techniques/T1091) | Replication Through Removable Media | Initial Access, Lateral Movement | Windows |
| [T1092](https://attack.mitre.org/techniques/T1092) | Communication Through Removable Media | Command And Control | Linux, macOS, Windows |
| [T1095](https://attack.mitre.org/techniques/T1095) | Non-Application Layer Protocol | Command And Control | ESXi, Linux, macOS, Network Devices, Windows |
| [T1098](https://attack.mitre.org/techniques/T1098) | Account Manipulation | Persistence, Privilege Escalation | Containers, ESXi, IaaS, Identity Provider, Linux, macOS, Network Devices, Office Suite, SaaS, Windows |
| [T1098.001](https://attack.mitre.org/techniques/T1098/001) | Additional Cloud Credentials | Persistence, Privilege Escalation | IaaS, Identity Provider, SaaS |
| [T1098.002](https://attack.mitre.org/techniques/T1098/002) | Additional Email Delegate Permissions | Persistence, Privilege Escalation | Windows, Office Suite |
| [T1098.003](https://attack.mitre.org/techniques/T1098/003) | Additional Cloud Roles | Persistence, Privilege Escalation | IaaS, Identity Provider, Office Suite, SaaS |
| [T1098.004](https://attack.mitre.org/techniques/T1098/004) | SSH Authorized Keys | Persistence, Privilege Escalation | Linux, macOS, IaaS, Network Devices, ESXi |
| [T1098.005](https://attack.mitre.org/techniques/T1098/005) | Device Registration | Persistence, Privilege Escalation | Windows, Identity Provider |
| [T1098.006](https://attack.mitre.org/techniques/T1098/006) | Additional Container Cluster Roles | Persistence, Privilege Escalation | Containers |
| [T1098.007](https://attack.mitre.org/techniques/T1098/007) | Additional Local or Domain Groups | Persistence, Privilege Escalation | Windows, macOS, Linux |
| [T1102](https://attack.mitre.org/techniques/T1102) | Web Service | Command And Control | ESXi, Linux, Windows, macOS |
| [T1102.001](https://attack.mitre.org/techniques/T1102/001) | Dead Drop Resolver | Command And Control | ESXi, Linux, macOS, Windows |
| [T1102.002](https://attack.mitre.org/techniques/T1102/002) | Bidirectional Communication | Command And Control | Linux, macOS, Windows, ESXi |
| [T1102.003](https://attack.mitre.org/techniques/T1102/003) | One-Way Communication | Command And Control | Linux, macOS, Windows, ESXi |
| [T1104](https://attack.mitre.org/techniques/T1104) | Multi-Stage Channels | Command And Control | Linux, macOS, Windows, ESXi |
| [T1105](https://attack.mitre.org/techniques/T1105) | Ingress Tool Transfer | Command And Control | ESXi, Linux, macOS, Network Devices, Windows |
| [T1106](https://attack.mitre.org/techniques/T1106) | Native API | Execution | Linux, macOS, Windows |
| [T1110](https://attack.mitre.org/techniques/T1110) | Brute Force | Credential Access | Containers, ESXi, IaaS, Identity Provider, Linux, macOS, Network Devices, Office Suite, SaaS, Windows |
| [T1110.001](https://attack.mitre.org/techniques/T1110/001) | Password Guessing | Credential Access | Windows, SaaS, IaaS, Linux, macOS, Containers, Network Devices, Office Suite, Identity Provider, ESXi |
| [T1110.002](https://attack.mitre.org/techniques/T1110/002) | Password Cracking | Credential Access | Linux, macOS, Windows, Network Devices, Office Suite, Identity Provider |
| [T1110.003](https://attack.mitre.org/techniques/T1110/003) | Password Spraying | Credential Access | Containers, ESXi, IaaS, Identity Provider, Linux, Network Devices, Office Suite, SaaS, Windows, macOS |
| [T1110.004](https://attack.mitre.org/techniques/T1110/004) | Credential Stuffing | Credential Access | Windows, SaaS, IaaS, Linux, macOS, Containers, Network Devices, Office Suite, Identity Provider, ESXi |
| [T1111](https://attack.mitre.org/techniques/T1111) | Multi-Factor Authentication Interception | Credential Access | Linux, Windows, macOS |
| [T1112](https://attack.mitre.org/techniques/T1112) | Modify Registry | Defense Evasion, Persistence | Windows |
| [T1113](https://attack.mitre.org/techniques/T1113) | Screen Capture | Collection | Linux, Windows, macOS |
| [T1114](https://attack.mitre.org/techniques/T1114) | Email Collection | Collection | Windows, macOS, Linux, Office Suite |
| [T1114.001](https://attack.mitre.org/techniques/T1114/001) | Local Email Collection | Collection | Windows |
| [T1114.002](https://attack.mitre.org/techniques/T1114/002) | Remote Email Collection | Collection | Windows, Office Suite |
| [T1114.003](https://attack.mitre.org/techniques/T1114/003) | Email Forwarding Rule | Collection | Linux, macOS, Office Suite, Windows |
| [T1115](https://attack.mitre.org/techniques/T1115) | Clipboard Data | Collection | Linux, macOS, Windows |
| [T1119](https://attack.mitre.org/techniques/T1119) | Automated Collection | Collection | IaaS, Linux, macOS, Office Suite, SaaS, Windows |
| [T1120](https://attack.mitre.org/techniques/T1120) | Peripheral Device Discovery | Discovery | Linux, Windows, macOS |
| [T1123](https://attack.mitre.org/techniques/T1123) | Audio Capture | Collection | Linux, macOS, Windows |
| [T1124](https://attack.mitre.org/techniques/T1124) | System Time Discovery | Discovery | ESXi, Linux, macOS, Network Devices, Windows |
| [T1125](https://attack.mitre.org/techniques/T1125) | Video Capture | Collection | Windows, macOS, Linux |
| [T1127](https://attack.mitre.org/techniques/T1127) | Trusted Developer Utilities Proxy Execution | Defense Evasion | Windows |
| [T1127.001](https://attack.mitre.org/techniques/T1127/001) | MSBuild | Defense Evasion | Windows |
| [T1127.002](https://attack.mitre.org/techniques/T1127/002) | ClickOnce | Defense Evasion | Windows |
| [T1127.003](https://attack.mitre.org/techniques/T1127/003) | JamPlus | Defense Evasion | Windows |
| [T1129](https://attack.mitre.org/techniques/T1129) | Shared Modules | Execution | Linux, macOS, Windows |
| [T1132](https://attack.mitre.org/techniques/T1132) | Data Encoding | Command And Control | Linux, macOS, Windows, ESXi |
| [T1132.001](https://attack.mitre.org/techniques/T1132/001) | Standard Encoding | Command And Control | ESXi, Linux, Windows, macOS |
| [T1132.002](https://attack.mitre.org/techniques/T1132/002) | Non-Standard Encoding | Command And Control | ESXi, Linux, macOS, Windows |
| [T1133](https://attack.mitre.org/techniques/T1133) | External Remote Services | Initial Access, Persistence | Containers, Linux, macOS, Windows |
| [T1134](https://attack.mitre.org/techniques/T1134) | Access Token Manipulation | Defense Evasion, Privilege Escalation | Windows |
| [T1134.001](https://attack.mitre.org/techniques/T1134/001) | Token Impersonation/Theft | Defense Evasion, Privilege Escalation | Windows |
| [T1134.002](https://attack.mitre.org/techniques/T1134/002) | Create Process with Token | Defense Evasion, Privilege Escalation | Windows |
| [T1134.003](https://attack.mitre.org/techniques/T1134/003) | Make and Impersonate Token | Defense Evasion, Privilege Escalation | Windows |
| [T1134.004](https://attack.mitre.org/techniques/T1134/004) | Parent PID Spoofing | Defense Evasion, Privilege Escalation | Windows |
| [T1134.005](https://attack.mitre.org/techniques/T1134/005) | SID-History Injection | Defense Evasion, Privilege Escalation | Windows |
| [T1135](https://attack.mitre.org/techniques/T1135) | Network Share Discovery | Discovery | Linux, macOS, Windows |
| [T1136](https://attack.mitre.org/techniques/T1136) | Create Account | Persistence | Windows, IaaS, Linux, macOS, Network Devices, Containers, SaaS, Office Suite, Identity Provider, ESXi |
| [T1136.001](https://attack.mitre.org/techniques/T1136/001) | Local Account | Persistence | Linux, macOS, Windows, Network Devices, Containers, ESXi |
| [T1136.002](https://attack.mitre.org/techniques/T1136/002) | Domain Account | Persistence | Linux, macOS, Windows |
| [T1136.003](https://attack.mitre.org/techniques/T1136/003) | Cloud Account | Persistence | IaaS, SaaS, Office Suite, Identity Provider |
| [T1137](https://attack.mitre.org/techniques/T1137) | Office Application Startup | Persistence | Windows, Office Suite |
| [T1137.001](https://attack.mitre.org/techniques/T1137/001) | Office Template Macros | Persistence | Windows, Office Suite |
| [T1137.002](https://attack.mitre.org/techniques/T1137/002) | Office Test | Persistence | Windows, Office Suite |
| [T1137.003](https://attack.mitre.org/techniques/T1137/003) | Outlook Forms | Persistence | Windows, Office Suite |
| [T1137.004](https://attack.mitre.org/techniques/T1137/004) | Outlook Home Page | Persistence | Windows, Office Suite |
| [T1137.005](https://attack.mitre.org/techniques/T1137/005) | Outlook Rules | Persistence | Windows, Office Suite |
| [T1137.006](https://attack.mitre.org/techniques/T1137/006) | Add-ins | Persistence | Windows, Office Suite |
| [T1140](https://attack.mitre.org/techniques/T1140) | Deobfuscate/Decode Files or Information | Defense Evasion | ESXi, Linux, macOS, Windows |
| [T1176](https://attack.mitre.org/techniques/T1176) | Software Extensions | Persistence | Linux, macOS, Windows |
| [T1176.001](https://attack.mitre.org/techniques/T1176/001) | Browser Extensions | Persistence | Linux, Windows, macOS |
| [T1176.002](https://attack.mitre.org/techniques/T1176/002) | IDE Extensions | Persistence | Linux, macOS, Windows |
| [T1185](https://attack.mitre.org/techniques/T1185) | Browser Session Hijacking | Collection | Windows |
| [T1187](https://attack.mitre.org/techniques/T1187) | Forced Authentication | Credential Access | Windows |
| [T1189](https://attack.mitre.org/techniques/T1189) | Drive-by Compromise | Initial Access | Identity Provider, Linux, macOS, Windows |
| [T1190](https://attack.mitre.org/techniques/T1190) | Exploit Public-Facing Application | Initial Access | Containers, ESXi, IaaS, Linux, macOS, Network Devices, Windows |
| [T1195](https://attack.mitre.org/techniques/T1195) | Supply Chain Compromise | Initial Access | Linux, Windows, macOS, SaaS |
| [T1195.001](https://attack.mitre.org/techniques/T1195/001) | Compromise Software Dependencies and Development Tools | Initial Access | Linux, macOS, Windows |
| [T1195.002](https://attack.mitre.org/techniques/T1195/002) | Compromise Software Supply Chain | Initial Access | Linux, Windows, macOS |
| [T1195.003](https://attack.mitre.org/techniques/T1195/003) | Compromise Hardware Supply Chain | Initial Access | Linux, macOS, Windows |
| [T1197](https://attack.mitre.org/techniques/T1197) | BITS Jobs | Defense Evasion, Persistence | Windows |
| [T1199](https://attack.mitre.org/techniques/T1199) | Trusted Relationship | Initial Access | Windows, SaaS, IaaS, Linux, macOS, Identity Provider, Office Suite |
| [T1200](https://attack.mitre.org/techniques/T1200) | Hardware Additions | Initial Access | Windows, Linux, macOS |
| [T1201](https://attack.mitre.org/techniques/T1201) | Password Policy Discovery | Discovery | Windows, Linux, macOS, IaaS, Network Devices, Identity Provider, SaaS, Office Suite |
| [T1202](https://attack.mitre.org/techniques/T1202) | Indirect Command Execution | Defense Evasion | Windows |
| [T1203](https://attack.mitre.org/techniques/T1203) | Exploitation for Client Execution | Execution | Linux, macOS, Windows |
| [T1204](https://attack.mitre.org/techniques/T1204) | User Execution | Execution | Linux, Windows, macOS, IaaS, Containers |
| [T1204.001](https://attack.mitre.org/techniques/T1204/001) | Malicious Link | Execution | Linux, macOS, Windows |
| [T1204.002](https://attack.mitre.org/techniques/T1204/002) | Malicious File | Execution | Linux, macOS, Windows |
| [T1204.003](https://attack.mitre.org/techniques/T1204/003) | Malicious Image | Execution | IaaS, Containers |
| [T1204.004](https://attack.mitre.org/techniques/T1204/004) | Malicious Copy and Paste | Execution | Linux, macOS, Windows |
| [T1204.005](https://attack.mitre.org/techniques/T1204/005) | Malicious Library | Execution | Linux, macOS, Windows |
| [T1205](https://attack.mitre.org/techniques/T1205) | Traffic Signaling | Command And Control, Defense Evasion, Persistence | Linux, macOS, Network Devices, Windows |
| [T1205.001](https://attack.mitre.org/techniques/T1205/001) | Port Knocking | Command And Control, Defense Evasion, Persistence | Linux, macOS, Windows, Network Devices |
| [T1205.002](https://attack.mitre.org/techniques/T1205/002) | Socket Filters | Command And Control, Defense Evasion, Persistence | Linux, macOS, Windows |
| [T1207](https://attack.mitre.org/techniques/T1207) | Rogue Domain Controller | Defense Evasion | Windows |
| [T1210](https://attack.mitre.org/techniques/T1210) | Exploitation of Remote Services | Lateral Movement | Linux, Windows, macOS, ESXi |
| [T1211](https://attack.mitre.org/techniques/T1211) | Exploitation for Defense Evasion | Defense Evasion | Linux, Windows, macOS, SaaS, IaaS |
| [T1212](https://attack.mitre.org/techniques/T1212) | Exploitation for Credential Access | Credential Access | Linux, Windows, macOS, Identity Provider |
| [T1213](https://attack.mitre.org/techniques/T1213) | Data from Information Repositories | Collection | Linux, Windows, macOS, SaaS, IaaS, Office Suite |
| [T1213.001](https://attack.mitre.org/techniques/T1213/001) | Confluence | Collection | SaaS |
| [T1213.002](https://attack.mitre.org/techniques/T1213/002) | Sharepoint | Collection | Windows, Office Suite |
| [T1213.003](https://attack.mitre.org/techniques/T1213/003) | Code Repositories | Collection | SaaS |
| [T1213.004](https://attack.mitre.org/techniques/T1213/004) | Customer Relationship Management Software | Collection | SaaS |
| [T1213.005](https://attack.mitre.org/techniques/T1213/005) | Messaging Applications | Collection | SaaS, Office Suite |
| [T1213.006](https://attack.mitre.org/techniques/T1213/006) | Databases | Collection | Linux, Windows, macOS, IaaS, SaaS |
| [T1216](https://attack.mitre.org/techniques/T1216) | System Script Proxy Execution | Defense Evasion | Windows |
| [T1216.001](https://attack.mitre.org/techniques/T1216/001) | PubPrn | Defense Evasion | Windows |
| [T1216.002](https://attack.mitre.org/techniques/T1216/002) | SyncAppvPublishingServer | Defense Evasion | Windows |
| [T1217](https://attack.mitre.org/techniques/T1217) | Browser Information Discovery | Discovery | Linux, macOS, Windows |
| [T1218](https://attack.mitre.org/techniques/T1218) | System Binary Proxy Execution | Defense Evasion | Windows, Linux, macOS |
| [T1218.001](https://attack.mitre.org/techniques/T1218/001) | Compiled HTML File | Defense Evasion | Windows |
| [T1218.002](https://attack.mitre.org/techniques/T1218/002) | Control Panel | Defense Evasion | Windows |
| [T1218.003](https://attack.mitre.org/techniques/T1218/003) | CMSTP | Defense Evasion | Windows |
| [T1218.004](https://attack.mitre.org/techniques/T1218/004) | InstallUtil | Defense Evasion | Windows |
| [T1218.005](https://attack.mitre.org/techniques/T1218/005) | Mshta | Defense Evasion | Windows |
| [T1218.007](https://attack.mitre.org/techniques/T1218/007) | Msiexec | Defense Evasion | Windows |
| [T1218.008](https://attack.mitre.org/techniques/T1218/008) | Odbcconf | Defense Evasion | Windows |
| [T1218.009](https://attack.mitre.org/techniques/T1218/009) | Regsvcs/Regasm | Defense Evasion | Windows |
| [T1218.010](https://attack.mitre.org/techniques/T1218/010) | Regsvr32 | Defense Evasion | Windows |
| [T1218.011](https://attack.mitre.org/techniques/T1218/011) | Rundll32 | Defense Evasion | Windows |
| [T1218.012](https://attack.mitre.org/techniques/T1218/012) | Verclsid | Defense Evasion | Windows |
| [T1218.013](https://attack.mitre.org/techniques/T1218/013) | Mavinject | Defense Evasion | Windows |
| [T1218.014](https://attack.mitre.org/techniques/T1218/014) | MMC | Defense Evasion | Windows |
| [T1218.015](https://attack.mitre.org/techniques/T1218/015) | Electron Applications | Defense Evasion | Linux, macOS, Windows |
| [T1219](https://attack.mitre.org/techniques/T1219) | Remote Access Tools | Command And Control | Linux, macOS, Windows |
| [T1219.001](https://attack.mitre.org/techniques/T1219/001) | IDE Tunneling | Command And Control | Linux, macOS, Windows |
| [T1219.002](https://attack.mitre.org/techniques/T1219/002) | Remote Desktop Software | Command And Control | Linux, macOS, Windows |
| [T1219.003](https://attack.mitre.org/techniques/T1219/003) | Remote Access Hardware | Command And Control | Linux, macOS, Windows |
| [T1220](https://attack.mitre.org/techniques/T1220) | XSL Script Processing | Defense Evasion | Windows |
| [T1221](https://attack.mitre.org/techniques/T1221) | Template Injection | Defense Evasion | Windows |
| [T1222](https://attack.mitre.org/techniques/T1222) | File and Directory Permissions Modification | Defense Evasion | ESXi, Linux, macOS, Windows |
| [T1222.001](https://attack.mitre.org/techniques/T1222/001) | Windows File and Directory Permissions Modification | Defense Evasion | Windows |
| [T1222.002](https://attack.mitre.org/techniques/T1222/002) | Linux and Mac File and Directory Permissions Modification | Defense Evasion | macOS, Linux |
| [T1480](https://attack.mitre.org/techniques/T1480) | Execution Guardrails | Defense Evasion | ESXi, Linux, macOS, Windows |
| [T1480.001](https://attack.mitre.org/techniques/T1480/001) | Environmental Keying | Defense Evasion | Linux, Windows, macOS |
| [T1480.002](https://attack.mitre.org/techniques/T1480/002) | Mutual Exclusion | Defense Evasion | Linux, macOS, Windows |
| [T1482](https://attack.mitre.org/techniques/T1482) | Domain Trust Discovery | Discovery | Windows |
| [T1484](https://attack.mitre.org/techniques/T1484) | Domain or Tenant Policy Modification | Defense Evasion, Privilege Escalation | Windows, Identity Provider |
| [T1484.001](https://attack.mitre.org/techniques/T1484/001) | Group Policy Modification | Defense Evasion, Privilege Escalation | Windows |
| [T1484.002](https://attack.mitre.org/techniques/T1484/002) | Trust Modification | Defense Evasion, Privilege Escalation | Identity Provider, Windows |
| [T1485](https://attack.mitre.org/techniques/T1485) | Data Destruction | Impact | Containers, ESXi, IaaS, Linux, macOS, Windows |
| [T1485.001](https://attack.mitre.org/techniques/T1485/001) | Lifecycle-Triggered Deletion | Impact | IaaS |
| [T1486](https://attack.mitre.org/techniques/T1486) | Data Encrypted for Impact | Impact | ESXi, IaaS, Linux, macOS, Windows |
| [T1489](https://attack.mitre.org/techniques/T1489) | Service Stop | Impact | ESXi, IaaS, Linux, macOS, Windows |
| [T1490](https://attack.mitre.org/techniques/T1490) | Inhibit System Recovery | Impact | Containers, ESXi, IaaS, Linux, macOS, Network Devices, Windows |
| [T1491](https://attack.mitre.org/techniques/T1491) | Defacement | Impact | Windows, IaaS, Linux, macOS, ESXi |
| [T1491.001](https://attack.mitre.org/techniques/T1491/001) | Internal Defacement | Impact | ESXi, Linux, macOS, Windows |
| [T1491.002](https://attack.mitre.org/techniques/T1491/002) | External Defacement | Impact | Windows, IaaS, Linux, macOS |
| [T1495](https://attack.mitre.org/techniques/T1495) | Firmware Corruption | Impact | Linux, macOS, Network Devices, Windows |
| [T1496](https://attack.mitre.org/techniques/T1496) | Resource Hijacking | Impact | Windows, IaaS, Linux, macOS, Containers, SaaS |
| [T1496.001](https://attack.mitre.org/techniques/T1496/001) | Compute Hijacking | Impact | Windows, IaaS, Linux, macOS, Containers |
| [T1496.002](https://attack.mitre.org/techniques/T1496/002) | Bandwidth Hijacking | Impact | Linux, Windows, macOS, IaaS, Containers |
| [T1496.003](https://attack.mitre.org/techniques/T1496/003) | SMS Pumping | Impact | SaaS |
| [T1496.004](https://attack.mitre.org/techniques/T1496/004) | Cloud Service Hijacking | Impact | SaaS |
| [T1497](https://attack.mitre.org/techniques/T1497) | Virtualization/Sandbox Evasion | Defense Evasion, Discovery | Linux, macOS, Windows |
| [T1497.001](https://attack.mitre.org/techniques/T1497/001) | System Checks | Defense Evasion, Discovery | Linux, macOS, Windows |
| [T1497.002](https://attack.mitre.org/techniques/T1497/002) | User Activity Based Checks | Defense Evasion, Discovery | Linux, Windows, macOS |
| [T1497.003](https://attack.mitre.org/techniques/T1497/003) | Time Based Checks | Defense Evasion, Discovery | Linux, macOS, Windows |
| [T1498](https://attack.mitre.org/techniques/T1498) | Network Denial of Service | Impact | Windows, IaaS, Linux, macOS, Containers |
| [T1498.001](https://attack.mitre.org/techniques/T1498/001) | Direct Network Flood | Impact | Windows, IaaS, Linux, macOS |
| [T1498.002](https://attack.mitre.org/techniques/T1498/002) | Reflection Amplification | Impact | Windows, IaaS, Linux, macOS |
| [T1499](https://attack.mitre.org/techniques/T1499) | Endpoint Denial of Service | Impact | Windows, Linux, macOS, Containers, IaaS |
| [T1499.001](https://attack.mitre.org/techniques/T1499/001) | OS Exhaustion Flood | Impact | Linux, macOS, Windows |
| [T1499.002](https://attack.mitre.org/techniques/T1499/002) | Service Exhaustion Flood | Impact | Windows, IaaS, Linux, macOS |
| [T1499.003](https://attack.mitre.org/techniques/T1499/003) | Application Exhaustion Flood | Impact | Windows, IaaS, Linux, macOS |
| [T1499.004](https://attack.mitre.org/techniques/T1499/004) | Application or System Exploitation | Impact | Windows, IaaS, Linux, macOS |
| [T1505](https://attack.mitre.org/techniques/T1505) | Server Software Component | Persistence | Windows, Linux, macOS, Network Devices, ESXi |
| [T1505.001](https://attack.mitre.org/techniques/T1505/001) | SQL Stored Procedures | Persistence | Windows, Linux |
| [T1505.002](https://attack.mitre.org/techniques/T1505/002) | Transport Agent | Persistence | Linux, Windows |
| [T1505.003](https://attack.mitre.org/techniques/T1505/003) | Web Shell | Persistence | Linux, macOS, Network Devices, Windows |
| [T1505.004](https://attack.mitre.org/techniques/T1505/004) | IIS Components | Persistence | Windows |
| [T1505.005](https://attack.mitre.org/techniques/T1505/005) | Terminal Services DLL | Persistence | Windows |
| [T1505.006](https://attack.mitre.org/techniques/T1505/006) | vSphere Installation Bundles | Persistence | ESXi |
| [T1518](https://attack.mitre.org/techniques/T1518) | Software Discovery | Discovery | ESXi, IaaS, Linux, macOS, Windows |
| [T1518.001](https://attack.mitre.org/techniques/T1518/001) | Security Software Discovery | Discovery | IaaS, Linux, macOS, Windows |
| [T1518.002](https://attack.mitre.org/techniques/T1518/002) | Backup Software Discovery | Discovery | Windows, macOS, Linux |
| [T1525](https://attack.mitre.org/techniques/T1525) | Implant Internal Image | Persistence | IaaS, Containers |
| [T1526](https://attack.mitre.org/techniques/T1526) | Cloud Service Discovery | Discovery | IaaS, Identity Provider, Office Suite, SaaS |
| [T1528](https://attack.mitre.org/techniques/T1528) | Steal Application Access Token | Credential Access | SaaS, Containers, IaaS, Office Suite, Identity Provider |
| [T1529](https://attack.mitre.org/techniques/T1529) | System Shutdown/Reboot | Impact | ESXi, Linux, macOS, Network Devices, Windows |
| [T1530](https://attack.mitre.org/techniques/T1530) | Data from Cloud Storage | Collection | IaaS, Office Suite, SaaS |
| [T1531](https://attack.mitre.org/techniques/T1531) | Account Access Removal | Impact | Linux, macOS, Windows, SaaS, IaaS, Office Suite, ESXi |
| [T1534](https://attack.mitre.org/techniques/T1534) | Internal Spearphishing | Lateral Movement | Windows, macOS, Linux, SaaS, Office Suite |
| [T1535](https://attack.mitre.org/techniques/T1535) | Unused/Unsupported Cloud Regions | Defense Evasion | IaaS |
| [T1537](https://attack.mitre.org/techniques/T1537) | Transfer Data to Cloud Account | Exfiltration | IaaS, Office Suite, SaaS |
| [T1538](https://attack.mitre.org/techniques/T1538) | Cloud Service Dashboard | Discovery | IaaS, SaaS, Office Suite, Identity Provider |
| [T1539](https://attack.mitre.org/techniques/T1539) | Steal Web Session Cookie | Credential Access | Linux, Office Suite, SaaS, Windows, macOS |
| [T1542](https://attack.mitre.org/techniques/T1542) | Pre-OS Boot | Defense Evasion, Persistence | Linux, Network Devices, Windows, macOS |
| [T1542.001](https://attack.mitre.org/techniques/T1542/001) | System Firmware | Defense Evasion, Persistence | Windows, Network Devices |
| [T1542.002](https://attack.mitre.org/techniques/T1542/002) | Component Firmware | Defense Evasion, Persistence | Windows, Linux, macOS |
| [T1542.003](https://attack.mitre.org/techniques/T1542/003) | Bootkit | Defense Evasion, Persistence | Linux, Windows |
| [T1542.004](https://attack.mitre.org/techniques/T1542/004) | ROMMONkit | Defense Evasion, Persistence | Network Devices |
| [T1542.005](https://attack.mitre.org/techniques/T1542/005) | TFTP Boot | Defense Evasion, Persistence | Network Devices |
| [T1543](https://attack.mitre.org/techniques/T1543) | Create or Modify System Process | Persistence, Privilege Escalation | Windows, macOS, Linux, Containers |
| [T1543.001](https://attack.mitre.org/techniques/T1543/001) | Launch Agent | Persistence, Privilege Escalation | macOS |
| [T1543.002](https://attack.mitre.org/techniques/T1543/002) | Systemd Service | Persistence, Privilege Escalation | Linux |
| [T1543.003](https://attack.mitre.org/techniques/T1543/003) | Windows Service | Persistence, Privilege Escalation | Windows |
| [T1543.004](https://attack.mitre.org/techniques/T1543/004) | Launch Daemon | Persistence, Privilege Escalation | macOS |
| [T1543.005](https://attack.mitre.org/techniques/T1543/005) | Container Service | Persistence, Privilege Escalation | Containers |
| [T1546](https://attack.mitre.org/techniques/T1546) | Event Triggered Execution | Persistence, Privilege Escalation | Linux, macOS, Windows, SaaS, IaaS, Office Suite |
| [T1546.001](https://attack.mitre.org/techniques/T1546/001) | Change Default File Association | Persistence, Privilege Escalation | Windows |
| [T1546.002](https://attack.mitre.org/techniques/T1546/002) | Screensaver | Persistence, Privilege Escalation | Windows |
| [T1546.003](https://attack.mitre.org/techniques/T1546/003) | Windows Management Instrumentation Event Subscription | Persistence, Privilege Escalation | Windows |
| [T1546.004](https://attack.mitre.org/techniques/T1546/004) | Unix Shell Configuration Modification | Persistence, Privilege Escalation | Linux, macOS |
| [T1546.005](https://attack.mitre.org/techniques/T1546/005) | Trap | Persistence, Privilege Escalation | macOS, Linux |
| [T1546.006](https://attack.mitre.org/techniques/T1546/006) | LC_LOAD_DYLIB Addition | Persistence, Privilege Escalation | macOS |
| [T1546.007](https://attack.mitre.org/techniques/T1546/007) | Netsh Helper DLL | Persistence, Privilege Escalation | Windows |
| [T1546.008](https://attack.mitre.org/techniques/T1546/008) | Accessibility Features | Persistence, Privilege Escalation | Windows |
| [T1546.009](https://attack.mitre.org/techniques/T1546/009) | AppCert DLLs | Persistence, Privilege Escalation | Windows |
| [T1546.010](https://attack.mitre.org/techniques/T1546/010) | AppInit DLLs | Persistence, Privilege Escalation | Windows |
| [T1546.011](https://attack.mitre.org/techniques/T1546/011) | Application Shimming | Persistence, Privilege Escalation | Windows |
| [T1546.012](https://attack.mitre.org/techniques/T1546/012) | Image File Execution Options Injection | Persistence, Privilege Escalation | Windows |
| [T1546.013](https://attack.mitre.org/techniques/T1546/013) | PowerShell Profile | Persistence, Privilege Escalation | Windows |
| [T1546.014](https://attack.mitre.org/techniques/T1546/014) | Emond | Persistence, Privilege Escalation | macOS |
| [T1546.015](https://attack.mitre.org/techniques/T1546/015) | Component Object Model Hijacking | Persistence, Privilege Escalation | Windows |
| [T1546.016](https://attack.mitre.org/techniques/T1546/016) | Installer Packages | Persistence, Privilege Escalation | Linux, Windows, macOS |
| [T1546.017](https://attack.mitre.org/techniques/T1546/017) | Udev Rules | Persistence, Privilege Escalation | Linux |
| [T1546.018](https://attack.mitre.org/techniques/T1546/018) | Python Startup Hooks | Persistence, Privilege Escalation | Linux, macOS, Windows |
| [T1547](https://attack.mitre.org/techniques/T1547) | Boot or Logon Autostart Execution | Persistence, Privilege Escalation | Linux, macOS, Windows, Network Devices |
| [T1547.001](https://attack.mitre.org/techniques/T1547/001) | Registry Run Keys / Startup Folder | Persistence, Privilege Escalation | Windows |
| [T1547.002](https://attack.mitre.org/techniques/T1547/002) | Authentication Package | Persistence, Privilege Escalation | Windows |
| [T1547.003](https://attack.mitre.org/techniques/T1547/003) | Time Providers | Persistence, Privilege Escalation | Windows |
| [T1547.004](https://attack.mitre.org/techniques/T1547/004) | Winlogon Helper DLL | Persistence, Privilege Escalation | Windows |
| [T1547.005](https://attack.mitre.org/techniques/T1547/005) | Security Support Provider | Persistence, Privilege Escalation | Windows |
| [T1547.006](https://attack.mitre.org/techniques/T1547/006) | Kernel Modules and Extensions | Persistence, Privilege Escalation | macOS, Linux |
| [T1547.007](https://attack.mitre.org/techniques/T1547/007) | Re-opened Applications | Persistence, Privilege Escalation | macOS |
| [T1547.008](https://attack.mitre.org/techniques/T1547/008) | LSASS Driver | Persistence, Privilege Escalation | Windows |
| [T1547.009](https://attack.mitre.org/techniques/T1547/009) | Shortcut Modification | Persistence, Privilege Escalation | Windows |
| [T1547.010](https://attack.mitre.org/techniques/T1547/010) | Port Monitors | Persistence, Privilege Escalation | Windows |
| [T1547.012](https://attack.mitre.org/techniques/T1547/012) | Print Processors | Persistence, Privilege Escalation | Windows |
| [T1547.013](https://attack.mitre.org/techniques/T1547/013) | XDG Autostart Entries | Persistence, Privilege Escalation | Linux |
| [T1547.014](https://attack.mitre.org/techniques/T1547/014) | Active Setup | Persistence, Privilege Escalation | Windows |
| [T1547.015](https://attack.mitre.org/techniques/T1547/015) | Login Items | Persistence, Privilege Escalation | macOS |
| [T1548](https://attack.mitre.org/techniques/T1548) | Abuse Elevation Control Mechanism | Defense Evasion, Privilege Escalation | Linux, macOS, Windows, IaaS, Office Suite, Identity Provider |
| [T1548.001](https://attack.mitre.org/techniques/T1548/001) | Setuid and Setgid | Defense Evasion, Privilege Escalation | Linux, macOS |
| [T1548.002](https://attack.mitre.org/techniques/T1548/002) | Bypass User Account Control | Defense Evasion, Privilege Escalation | Windows |
| [T1548.003](https://attack.mitre.org/techniques/T1548/003) | Sudo and Sudo Caching | Defense Evasion, Privilege Escalation | Linux, macOS |
| [T1548.004](https://attack.mitre.org/techniques/T1548/004) | Elevated Execution with Prompt | Defense Evasion, Privilege Escalation | macOS |
| [T1548.005](https://attack.mitre.org/techniques/T1548/005) | Temporary Elevated Cloud Access | Defense Evasion, Privilege Escalation | IaaS, Office Suite, Identity Provider |
| [T1548.006](https://attack.mitre.org/techniques/T1548/006) | TCC Manipulation | Defense Evasion, Privilege Escalation | macOS |
| [T1550](https://attack.mitre.org/techniques/T1550) | Use Alternate Authentication Material | Defense Evasion, Lateral Movement | Windows, SaaS, IaaS, Containers, Identity Provider, Office Suite, Linux |
| [T1550.001](https://attack.mitre.org/techniques/T1550/001) | Application Access Token | Defense Evasion, Lateral Movement | SaaS, Containers, IaaS, Office Suite, Identity Provider |
| [T1550.002](https://attack.mitre.org/techniques/T1550/002) | Pass the Hash | Defense Evasion, Lateral Movement | Windows |
| [T1550.003](https://attack.mitre.org/techniques/T1550/003) | Pass the Ticket | Defense Evasion, Lateral Movement | Windows |
| [T1550.004](https://attack.mitre.org/techniques/T1550/004) | Web Session Cookie | Defense Evasion, Lateral Movement | SaaS, IaaS, Office Suite |
| [T1552](https://attack.mitre.org/techniques/T1552) | Unsecured Credentials | Credential Access | Windows, SaaS, IaaS, Linux, macOS, Containers, Network Devices, Office Suite, Identity Provider |
| [T1552.001](https://attack.mitre.org/techniques/T1552/001) | Credentials In Files | Credential Access | Containers, IaaS, Linux, macOS, Windows |
| [T1552.002](https://attack.mitre.org/techniques/T1552/002) | Credentials in Registry | Credential Access | Windows |
| [T1552.003](https://attack.mitre.org/techniques/T1552/003) | Shell History | Credential Access | Linux, macOS, Windows |
| [T1552.004](https://attack.mitre.org/techniques/T1552/004) | Private Keys | Credential Access | Linux, macOS, Network Devices, Windows |
| [T1552.005](https://attack.mitre.org/techniques/T1552/005) | Cloud Instance Metadata API | Credential Access | IaaS |
| [T1552.006](https://attack.mitre.org/techniques/T1552/006) | Group Policy Preferences | Credential Access | Windows |
| [T1552.007](https://attack.mitre.org/techniques/T1552/007) | Container API | Credential Access | Containers |
| [T1552.008](https://attack.mitre.org/techniques/T1552/008) | Chat Messages | Credential Access | SaaS, Office Suite |
| [T1553](https://attack.mitre.org/techniques/T1553) | Subvert Trust Controls | Defense Evasion | Windows, macOS, Linux |
| [T1553.001](https://attack.mitre.org/techniques/T1553/001) | Gatekeeper Bypass | Defense Evasion | macOS |
| [T1553.002](https://attack.mitre.org/techniques/T1553/002) | Code Signing | Defense Evasion | macOS, Windows |
| [T1553.003](https://attack.mitre.org/techniques/T1553/003) | SIP and Trust Provider Hijacking | Defense Evasion | Windows |
| [T1553.004](https://attack.mitre.org/techniques/T1553/004) | Install Root Certificate | Defense Evasion | Linux, macOS, Windows |
| [T1553.005](https://attack.mitre.org/techniques/T1553/005) | Mark-of-the-Web Bypass | Defense Evasion | Windows |
| [T1553.006](https://attack.mitre.org/techniques/T1553/006) | Code Signing Policy Modification | Defense Evasion | Windows, macOS |
| [T1554](https://attack.mitre.org/techniques/T1554) | Compromise Host Software Binary | Persistence | Linux, macOS, Windows, ESXi |
| [T1555](https://attack.mitre.org/techniques/T1555) | Credentials from Password Stores | Credential Access | IaaS, Linux, macOS, Windows |
| [T1555.001](https://attack.mitre.org/techniques/T1555/001) | Keychain | Credential Access | macOS |
| [T1555.002](https://attack.mitre.org/techniques/T1555/002) | Securityd Memory | Credential Access | Linux, macOS |
| [T1555.003](https://attack.mitre.org/techniques/T1555/003) | Credentials from Web Browsers | Credential Access | Linux, macOS, Windows |
| [T1555.004](https://attack.mitre.org/techniques/T1555/004) | Windows Credential Manager | Credential Access | Windows |
| [T1555.005](https://attack.mitre.org/techniques/T1555/005) | Password Managers | Credential Access | Linux, macOS, Windows |
| [T1555.006](https://attack.mitre.org/techniques/T1555/006) | Cloud Secrets Management Stores | Credential Access | IaaS |
| [T1556](https://attack.mitre.org/techniques/T1556) | Modify Authentication Process | Credential Access, Defense Evasion, Persistence | Windows, Linux, macOS, Network Devices, IaaS, SaaS, Office Suite, Identity Provider |
| [T1556.001](https://attack.mitre.org/techniques/T1556/001) | Domain Controller Authentication | Credential Access, Defense Evasion, Persistence | Windows |
| [T1556.002](https://attack.mitre.org/techniques/T1556/002) | Password Filter DLL | Credential Access, Defense Evasion, Persistence | Windows |
| [T1556.003](https://attack.mitre.org/techniques/T1556/003) | Pluggable Authentication Modules | Credential Access, Defense Evasion, Persistence | Linux, macOS |
| [T1556.004](https://attack.mitre.org/techniques/T1556/004) | Network Device Authentication | Credential Access, Defense Evasion, Persistence | Network Devices |
| [T1556.005](https://attack.mitre.org/techniques/T1556/005) | Reversible Encryption | Credential Access, Defense Evasion, Persistence | Windows |
| [T1556.006](https://attack.mitre.org/techniques/T1556/006) | Multi-Factor Authentication | Credential Access, Defense Evasion, Persistence | Windows, SaaS, IaaS, Linux, macOS, Office Suite, Identity Provider |
| [T1556.007](https://attack.mitre.org/techniques/T1556/007) | Hybrid Identity | Credential Access, Defense Evasion, Persistence | Windows, SaaS, IaaS, Office Suite, Identity Provider |
| [T1556.008](https://attack.mitre.org/techniques/T1556/008) | Network Provider DLL | Credential Access, Defense Evasion, Persistence | Windows |
| [T1556.009](https://attack.mitre.org/techniques/T1556/009) | Conditional Access Policies | Credential Access, Defense Evasion, Persistence | IaaS, Identity Provider |
| [T1557](https://attack.mitre.org/techniques/T1557) | Adversary-in-the-Middle | Collection, Credential Access | Linux, macOS, Network Devices, Windows |
| [T1557.001](https://attack.mitre.org/techniques/T1557/001) | LLMNR/NBT-NS Poisoning and SMB Relay | Collection, Credential Access | Windows |
| [T1557.002](https://attack.mitre.org/techniques/T1557/002) | ARP Cache Poisoning | Collection, Credential Access | Linux, Windows, macOS |
| [T1557.003](https://attack.mitre.org/techniques/T1557/003) | DHCP Spoofing | Collection, Credential Access | Linux, Windows, macOS |
| [T1557.004](https://attack.mitre.org/techniques/T1557/004) | Evil Twin | Collection, Credential Access | Network Devices |
| [T1558](https://attack.mitre.org/techniques/T1558) | Steal or Forge Kerberos Tickets | Credential Access | Windows, Linux, macOS |
| [T1558.001](https://attack.mitre.org/techniques/T1558/001) | Golden Ticket | Credential Access | Windows |
| [T1558.002](https://attack.mitre.org/techniques/T1558/002) | Silver Ticket | Credential Access | Windows |
| [T1558.003](https://attack.mitre.org/techniques/T1558/003) | Kerberoasting | Credential Access | Windows |
| [T1558.004](https://attack.mitre.org/techniques/T1558/004) | AS-REP Roasting | Credential Access | Windows |
| [T1558.005](https://attack.mitre.org/techniques/T1558/005) | Ccache Files | Credential Access | Linux, macOS |
| [T1559](https://attack.mitre.org/techniques/T1559) | Inter-Process Communication | Execution | Linux, macOS, Windows |
| [T1559.001](https://attack.mitre.org/techniques/T1559/001) | Component Object Model | Execution | Windows |
| [T1559.002](https://attack.mitre.org/techniques/T1559/002) | Dynamic Data Exchange | Execution | Windows |
| [T1559.003](https://attack.mitre.org/techniques/T1559/003) | XPC Services | Execution | macOS |
| [T1560](https://attack.mitre.org/techniques/T1560) | Archive Collected Data | Collection | Linux, macOS, Windows |
| [T1560.001](https://attack.mitre.org/techniques/T1560/001) | Archive via Utility | Collection | Linux, macOS, Windows |
| [T1560.002](https://attack.mitre.org/techniques/T1560/002) | Archive via Library | Collection | Linux, macOS, Windows |
| [T1560.003](https://attack.mitre.org/techniques/T1560/003) | Archive via Custom Method | Collection | Linux, macOS, Windows |
| [T1561](https://attack.mitre.org/techniques/T1561) | Disk Wipe | Impact | Linux, macOS, Windows, Network Devices |
| [T1561.001](https://attack.mitre.org/techniques/T1561/001) | Disk Content Wipe | Impact | Linux, Network Devices, Windows, macOS |
| [T1561.002](https://attack.mitre.org/techniques/T1561/002) | Disk Structure Wipe | Impact | Linux, macOS, Windows, Network Devices |
| [T1562](https://attack.mitre.org/techniques/T1562) | Impair Defenses | Defense Evasion | Windows, IaaS, Linux, macOS, Containers, Network Devices, Identity Provider, Office Suite, ESXi |
| [T1562.001](https://attack.mitre.org/techniques/T1562/001) | Disable or Modify Tools | Defense Evasion | Containers, IaaS, Linux, macOS, Network Devices, Windows |
| [T1562.002](https://attack.mitre.org/techniques/T1562/002) | Disable Windows Event Logging | Defense Evasion | Windows |
| [T1562.003](https://attack.mitre.org/techniques/T1562/003) | Impair Command History Logging | Defense Evasion | ESXi, Linux, macOS, Network Devices, Windows |
| [T1562.004](https://attack.mitre.org/techniques/T1562/004) | Disable or Modify System Firewall | Defense Evasion | ESXi, Linux, macOS, Network Devices, Windows |
| [T1562.006](https://attack.mitre.org/techniques/T1562/006) | Indicator Blocking | Defense Evasion | Windows, macOS, Linux, ESXi |
| [T1562.007](https://attack.mitre.org/techniques/T1562/007) | Disable or Modify Cloud Firewall | Defense Evasion | IaaS |
| [T1562.008](https://attack.mitre.org/techniques/T1562/008) | Disable or Modify Cloud Logs | Defense Evasion | IaaS, SaaS, Office Suite, Identity Provider |
| [T1562.009](https://attack.mitre.org/techniques/T1562/009) | Safe Mode Boot | Defense Evasion | Windows |
| [T1562.010](https://attack.mitre.org/techniques/T1562/010) | Downgrade Attack | Defense Evasion | Windows, Linux, macOS |
| [T1562.011](https://attack.mitre.org/techniques/T1562/011) | Spoof Security Alerting | Defense Evasion | Windows, macOS, Linux |
| [T1562.012](https://attack.mitre.org/techniques/T1562/012) | Disable or Modify Linux Audit System | Defense Evasion | Linux |
| [T1562.013](https://attack.mitre.org/techniques/T1562/013) | Disable or Modify Network Device Firewall | Defense Evasion | Network Devices |
| [T1563](https://attack.mitre.org/techniques/T1563) | Remote Service Session Hijacking | Lateral Movement | Linux, macOS, Windows |
| [T1563.001](https://attack.mitre.org/techniques/T1563/001) | SSH Hijacking | Lateral Movement | Linux, macOS |
| [T1563.002](https://attack.mitre.org/techniques/T1563/002) | RDP Hijacking | Lateral Movement | Windows |
| [T1564](https://attack.mitre.org/techniques/T1564) | Hide Artifacts | Defense Evasion | Linux, Office Suite, Windows, macOS, ESXi |
| [T1564.001](https://attack.mitre.org/techniques/T1564/001) | Hidden Files and Directories | Defense Evasion | Linux, Windows, macOS |
| [T1564.002](https://attack.mitre.org/techniques/T1564/002) | Hidden Users | Defense Evasion | macOS, Windows, Linux |
| [T1564.003](https://attack.mitre.org/techniques/T1564/003) | Hidden Window | Defense Evasion | Linux, macOS, Windows |
| [T1564.004](https://attack.mitre.org/techniques/T1564/004) | NTFS File Attributes | Defense Evasion | Windows |
| [T1564.005](https://attack.mitre.org/techniques/T1564/005) | Hidden File System | Defense Evasion | Linux, macOS, Windows |
| [T1564.006](https://attack.mitre.org/techniques/T1564/006) | Run Virtual Instance | Defense Evasion | Linux, macOS, Windows, ESXi |
| [T1564.007](https://attack.mitre.org/techniques/T1564/007) | VBA Stomping | Defense Evasion | Linux, Windows, macOS |
| [T1564.008](https://attack.mitre.org/techniques/T1564/008) | Email Hiding Rules | Defense Evasion | Windows, Linux, macOS, Office Suite |
| [T1564.009](https://attack.mitre.org/techniques/T1564/009) | Resource Forking | Defense Evasion | macOS |
| [T1564.010](https://attack.mitre.org/techniques/T1564/010) | Process Argument Spoofing | Defense Evasion | Windows |
| [T1564.011](https://attack.mitre.org/techniques/T1564/011) | Ignore Process Interrupts | Defense Evasion | Linux, macOS, Windows |
| [T1564.012](https://attack.mitre.org/techniques/T1564/012) | File/Path Exclusions | Defense Evasion | Linux, macOS, Windows |
| [T1564.013](https://attack.mitre.org/techniques/T1564/013) | Bind Mounts | Defense Evasion | Linux |
| [T1564.014](https://attack.mitre.org/techniques/T1564/014) | Extended Attributes | Defense Evasion | Linux, macOS |
| [T1565](https://attack.mitre.org/techniques/T1565) | Data Manipulation | Impact | Linux, macOS, Windows |
| [T1565.001](https://attack.mitre.org/techniques/T1565/001) | Stored Data Manipulation | Impact | Linux, macOS, Windows |
| [T1565.002](https://attack.mitre.org/techniques/T1565/002) | Transmitted Data Manipulation | Impact | Linux, macOS, Windows |
| [T1565.003](https://attack.mitre.org/techniques/T1565/003) | Runtime Data Manipulation | Impact | Linux, macOS, Windows |
| [T1566](https://attack.mitre.org/techniques/T1566) | Phishing | Initial Access | Identity Provider, Linux, macOS, Office Suite, SaaS, Windows |
| [T1566.001](https://attack.mitre.org/techniques/T1566/001) | Spearphishing Attachment | Initial Access | Linux, macOS, Windows |
| [T1566.002](https://attack.mitre.org/techniques/T1566/002) | Spearphishing Link | Initial Access | Identity Provider, Linux, macOS, Office Suite, SaaS, Windows |
| [T1566.003](https://attack.mitre.org/techniques/T1566/003) | Spearphishing via Service | Initial Access | Linux, macOS, Windows |
| [T1566.004](https://attack.mitre.org/techniques/T1566/004) | Spearphishing Voice | Initial Access | Linux, macOS, Windows, Identity Provider |
| [T1567](https://attack.mitre.org/techniques/T1567) | Exfiltration Over Web Service | Exfiltration | ESXi, Linux, macOS, Office Suite, SaaS, Windows |
| [T1567.001](https://attack.mitre.org/techniques/T1567/001) | Exfiltration to Code Repository | Exfiltration | Linux, macOS, Windows, ESXi |
| [T1567.002](https://attack.mitre.org/techniques/T1567/002) | Exfiltration to Cloud Storage | Exfiltration | ESXi, Linux, macOS, Windows |
| [T1567.003](https://attack.mitre.org/techniques/T1567/003) | Exfiltration to Text Storage Sites | Exfiltration | Linux, macOS, Windows, ESXi |
| [T1567.004](https://attack.mitre.org/techniques/T1567/004) | Exfiltration Over Webhook | Exfiltration | Windows, macOS, Linux, SaaS, Office Suite, ESXi |
| [T1568](https://attack.mitre.org/techniques/T1568) | Dynamic Resolution | Command And Control | Linux, macOS, Windows, ESXi |
| [T1568.001](https://attack.mitre.org/techniques/T1568/001) | Fast Flux DNS | Command And Control | Linux, macOS, Windows, ESXi |
| [T1568.002](https://attack.mitre.org/techniques/T1568/002) | Domain Generation Algorithms | Command And Control | Linux, macOS, Windows, ESXi |
| [T1568.003](https://attack.mitre.org/techniques/T1568/003) | DNS Calculation | Command And Control | Linux, macOS, Windows, ESXi |
| [T1569](https://attack.mitre.org/techniques/T1569) | System Services | Execution | Windows, macOS, Linux |
| [T1569.001](https://attack.mitre.org/techniques/T1569/001) | Launchctl | Execution | macOS |
| [T1569.002](https://attack.mitre.org/techniques/T1569/002) | Service Execution | Execution | Windows |
| [T1569.003](https://attack.mitre.org/techniques/T1569/003) | Systemctl | Execution | Linux |
| [T1570](https://attack.mitre.org/techniques/T1570) | Lateral Tool Transfer | Lateral Movement | ESXi, Linux, macOS, Windows |
| [T1571](https://attack.mitre.org/techniques/T1571) | Non-Standard Port | Command And Control | ESXi, Linux, macOS, Windows |
| [T1572](https://attack.mitre.org/techniques/T1572) | Protocol Tunneling | Command And Control | ESXi, Linux, macOS, Windows |
| [T1573](https://attack.mitre.org/techniques/T1573) | Encrypted Channel | Command And Control | ESXi, Linux, macOS, Network Devices, Windows |
| [T1573.001](https://attack.mitre.org/techniques/T1573/001) | Symmetric Cryptography | Command And Control | ESXi, Linux, macOS, Network Devices, Windows |
| [T1573.002](https://attack.mitre.org/techniques/T1573/002) | Asymmetric Cryptography | Command And Control | ESXi, Linux, macOS, Network Devices, Windows |
| [T1574](https://attack.mitre.org/techniques/T1574) | Hijack Execution Flow | Defense Evasion, Persistence, Privilege Escalation | Linux, macOS, Windows |
| [T1574.001](https://attack.mitre.org/techniques/T1574/001) | DLL | Defense Evasion, Persistence, Privilege Escalation | Windows |
| [T1574.004](https://attack.mitre.org/techniques/T1574/004) | Dylib Hijacking | Defense Evasion, Persistence, Privilege Escalation | macOS |
| [T1574.005](https://attack.mitre.org/techniques/T1574/005) | Executable Installer File Permissions Weakness | Defense Evasion, Persistence, Privilege Escalation | Windows |
| [T1574.006](https://attack.mitre.org/techniques/T1574/006) | Dynamic Linker Hijacking | Defense Evasion, Persistence, Privilege Escalation | Linux, macOS |
| [T1574.007](https://attack.mitre.org/techniques/T1574/007) | Path Interception by PATH Environment Variable | Defense Evasion, Persistence, Privilege Escalation | Windows, macOS, Linux |
| [T1574.008](https://attack.mitre.org/techniques/T1574/008) | Path Interception by Search Order Hijacking | Defense Evasion, Persistence, Privilege Escalation | Windows |
| [T1574.009](https://attack.mitre.org/techniques/T1574/009) | Path Interception by Unquoted Path | Defense Evasion, Persistence, Privilege Escalation | Windows |
| [T1574.010](https://attack.mitre.org/techniques/T1574/010) | Services File Permissions Weakness | Defense Evasion, Persistence, Privilege Escalation | Windows |
| [T1574.011](https://attack.mitre.org/techniques/T1574/011) | Services Registry Permissions Weakness | Defense Evasion, Persistence, Privilege Escalation | Windows |
| [T1574.012](https://attack.mitre.org/techniques/T1574/012) | COR_PROFILER | Defense Evasion, Persistence, Privilege Escalation | Windows |
| [T1574.013](https://attack.mitre.org/techniques/T1574/013) | KernelCallbackTable | Defense Evasion, Persistence, Privilege Escalation | Windows |
| [T1574.014](https://attack.mitre.org/techniques/T1574/014) | AppDomainManager | Defense Evasion, Persistence, Privilege Escalation | Windows |
| [T1578](https://attack.mitre.org/techniques/T1578) | Modify Cloud Compute Infrastructure | Defense Evasion | IaaS |
| [T1578.001](https://attack.mitre.org/techniques/T1578/001) | Create Snapshot | Defense Evasion | IaaS |
| [T1578.002](https://attack.mitre.org/techniques/T1578/002) | Create Cloud Instance | Defense Evasion | IaaS |
| [T1578.003](https://attack.mitre.org/techniques/T1578/003) | Delete Cloud Instance | Defense Evasion | IaaS |
| [T1578.004](https://attack.mitre.org/techniques/T1578/004) | Revert Cloud Instance | Defense Evasion | IaaS |
| [T1578.005](https://attack.mitre.org/techniques/T1578/005) | Modify Cloud Compute Configurations | Defense Evasion | IaaS |
| [T1580](https://attack.mitre.org/techniques/T1580) | Cloud Infrastructure Discovery | Discovery | IaaS |
| [T1583](https://attack.mitre.org/techniques/T1583) | Acquire Infrastructure | Resource Development | PRE |
| [T1583.001](https://attack.mitre.org/techniques/T1583/001) | Domains | Resource Development | PRE |
| [T1583.002](https://attack.mitre.org/techniques/T1583/002) | DNS Server | Resource Development | PRE |
| [T1583.003](https://attack.mitre.org/techniques/T1583/003) | Virtual Private Server | Resource Development | PRE |
| [T1583.004](https://attack.mitre.org/techniques/T1583/004) | Server | Resource Development | PRE |
| [T1583.005](https://attack.mitre.org/techniques/T1583/005) | Botnet | Resource Development | PRE |
| [T1583.006](https://attack.mitre.org/techniques/T1583/006) | Web Services | Resource Development | PRE |
| [T1583.007](https://attack.mitre.org/techniques/T1583/007) | Serverless | Resource Development | PRE |
| [T1583.008](https://attack.mitre.org/techniques/T1583/008) | Malvertising | Resource Development | PRE |
| [T1584](https://attack.mitre.org/techniques/T1584) | Compromise Infrastructure | Resource Development | PRE |
| [T1584.001](https://attack.mitre.org/techniques/T1584/001) | Domains | Resource Development | PRE |
| [T1584.002](https://attack.mitre.org/techniques/T1584/002) | DNS Server | Resource Development | PRE |
| [T1584.003](https://attack.mitre.org/techniques/T1584/003) | Virtual Private Server | Resource Development | PRE |
| [T1584.004](https://attack.mitre.org/techniques/T1584/004) | Server | Resource Development | PRE |
| [T1584.005](https://attack.mitre.org/techniques/T1584/005) | Botnet | Resource Development | PRE |
| [T1584.006](https://attack.mitre.org/techniques/T1584/006) | Web Services | Resource Development | PRE |
| [T1584.007](https://attack.mitre.org/techniques/T1584/007) | Serverless | Resource Development | PRE |
| [T1584.008](https://attack.mitre.org/techniques/T1584/008) | Network Devices | Resource Development | PRE |
| [T1585](https://attack.mitre.org/techniques/T1585) | Establish Accounts | Resource Development | PRE |
| [T1585.001](https://attack.mitre.org/techniques/T1585/001) | Social Media Accounts | Resource Development | PRE |
| [T1585.002](https://attack.mitre.org/techniques/T1585/002) | Email Accounts | Resource Development | PRE |
| [T1585.003](https://attack.mitre.org/techniques/T1585/003) | Cloud Accounts | Resource Development | PRE |
| [T1586](https://attack.mitre.org/techniques/T1586) | Compromise Accounts | Resource Development | PRE |
| [T1586.001](https://attack.mitre.org/techniques/T1586/001) | Social Media Accounts | Resource Development | PRE |
| [T1586.002](https://attack.mitre.org/techniques/T1586/002) | Email Accounts | Resource Development | PRE |
| [T1586.003](https://attack.mitre.org/techniques/T1586/003) | Cloud Accounts | Resource Development | PRE |
| [T1587](https://attack.mitre.org/techniques/T1587) | Develop Capabilities | Resource Development | PRE |
| [T1587.001](https://attack.mitre.org/techniques/T1587/001) | Malware | Resource Development | PRE |
| [T1587.002](https://attack.mitre.org/techniques/T1587/002) | Code Signing Certificates | Resource Development | PRE |
| [T1587.003](https://attack.mitre.org/techniques/T1587/003) | Digital Certificates | Resource Development | PRE |
| [T1587.004](https://attack.mitre.org/techniques/T1587/004) | Exploits | Resource Development | PRE |
| [T1588](https://attack.mitre.org/techniques/T1588) | Obtain Capabilities | Resource Development | PRE |
| [T1588.001](https://attack.mitre.org/techniques/T1588/001) | Malware | Resource Development | PRE |
| [T1588.002](https://attack.mitre.org/techniques/T1588/002) | Tool | Resource Development | PRE |
| [T1588.003](https://attack.mitre.org/techniques/T1588/003) | Code Signing Certificates | Resource Development | PRE |
| [T1588.004](https://attack.mitre.org/techniques/T1588/004) | Digital Certificates | Resource Development | PRE |
| [T1588.005](https://attack.mitre.org/techniques/T1588/005) | Exploits | Resource Development | PRE |
| [T1588.006](https://attack.mitre.org/techniques/T1588/006) | Vulnerabilities | Resource Development | PRE |
| [T1588.007](https://attack.mitre.org/techniques/T1588/007) | Artificial Intelligence | Resource Development | PRE |
| [T1589](https://attack.mitre.org/techniques/T1589) | Gather Victim Identity Information | Reconnaissance | PRE |
| [T1589.001](https://attack.mitre.org/techniques/T1589/001) | Credentials | Reconnaissance | PRE |
| [T1589.002](https://attack.mitre.org/techniques/T1589/002) | Email Addresses | Reconnaissance | PRE |
| [T1589.003](https://attack.mitre.org/techniques/T1589/003) | Employee Names | Reconnaissance | PRE |
| [T1590](https://attack.mitre.org/techniques/T1590) | Gather Victim Network Information | Reconnaissance | PRE |
| [T1590.001](https://attack.mitre.org/techniques/T1590/001) | Domain Properties | Reconnaissance | PRE |
| [T1590.002](https://attack.mitre.org/techniques/T1590/002) | DNS | Reconnaissance | PRE |
| [T1590.003](https://attack.mitre.org/techniques/T1590/003) | Network Trust Dependencies | Reconnaissance | PRE |
| [T1590.004](https://attack.mitre.org/techniques/T1590/004) | Network Topology | Reconnaissance | PRE |
| [T1590.005](https://attack.mitre.org/techniques/T1590/005) | IP Addresses | Reconnaissance | PRE |
| [T1590.006](https://attack.mitre.org/techniques/T1590/006) | Network Security Appliances | Reconnaissance | PRE |
| [T1591](https://attack.mitre.org/techniques/T1591) | Gather Victim Org Information | Reconnaissance | PRE |
| [T1591.001](https://attack.mitre.org/techniques/T1591/001) | Determine Physical Locations | Reconnaissance | PRE |
| [T1591.002](https://attack.mitre.org/techniques/T1591/002) | Business Relationships | Reconnaissance | PRE |
| [T1591.003](https://attack.mitre.org/techniques/T1591/003) | Identify Business Tempo | Reconnaissance | PRE |
| [T1591.004](https://attack.mitre.org/techniques/T1591/004) | Identify Roles | Reconnaissance | PRE |
| [T1592](https://attack.mitre.org/techniques/T1592) | Gather Victim Host Information | Reconnaissance | PRE |
| [T1592.001](https://attack.mitre.org/techniques/T1592/001) | Hardware | Reconnaissance | PRE |
| [T1592.002](https://attack.mitre.org/techniques/T1592/002) | Software | Reconnaissance | PRE |
| [T1592.003](https://attack.mitre.org/techniques/T1592/003) | Firmware | Reconnaissance | PRE |
| [T1592.004](https://attack.mitre.org/techniques/T1592/004) | Client Configurations | Reconnaissance | PRE |
| [T1593](https://attack.mitre.org/techniques/T1593) | Search Open Websites/Domains | Reconnaissance | PRE |
| [T1593.001](https://attack.mitre.org/techniques/T1593/001) | Social Media | Reconnaissance | PRE |
| [T1593.002](https://attack.mitre.org/techniques/T1593/002) | Search Engines | Reconnaissance | PRE |
| [T1593.003](https://attack.mitre.org/techniques/T1593/003) | Code Repositories | Reconnaissance | PRE |
| [T1594](https://attack.mitre.org/techniques/T1594) | Search Victim-Owned Websites | Reconnaissance | PRE |
| [T1595](https://attack.mitre.org/techniques/T1595) | Active Scanning | Reconnaissance | PRE |
| [T1595.001](https://attack.mitre.org/techniques/T1595/001) | Scanning IP Blocks | Reconnaissance | PRE |
| [T1595.002](https://attack.mitre.org/techniques/T1595/002) | Vulnerability Scanning | Reconnaissance | PRE |
| [T1595.003](https://attack.mitre.org/techniques/T1595/003) | Wordlist Scanning | Reconnaissance | PRE |
| [T1596](https://attack.mitre.org/techniques/T1596) | Search Open Technical Databases | Reconnaissance | PRE |
| [T1596.001](https://attack.mitre.org/techniques/T1596/001) | DNS/Passive DNS | Reconnaissance | PRE |
| [T1596.002](https://attack.mitre.org/techniques/T1596/002) | WHOIS | Reconnaissance | PRE |
| [T1596.003](https://attack.mitre.org/techniques/T1596/003) | Digital Certificates | Reconnaissance | PRE |
| [T1596.004](https://attack.mitre.org/techniques/T1596/004) | CDNs | Reconnaissance | PRE |
| [T1596.005](https://attack.mitre.org/techniques/T1596/005) | Scan Databases | Reconnaissance | PRE |
| [T1597](https://attack.mitre.org/techniques/T1597) | Search Closed Sources | Reconnaissance | PRE |
| [T1597.001](https://attack.mitre.org/techniques/T1597/001) | Threat Intel Vendors | Reconnaissance | PRE |
| [T1597.002](https://attack.mitre.org/techniques/T1597/002) | Purchase Technical Data | Reconnaissance | PRE |
| [T1598](https://attack.mitre.org/techniques/T1598) | Phishing for Information | Reconnaissance | PRE |
| [T1598.001](https://attack.mitre.org/techniques/T1598/001) | Spearphishing Service | Reconnaissance | PRE |
| [T1598.002](https://attack.mitre.org/techniques/T1598/002) | Spearphishing Attachment | Reconnaissance | PRE |
| [T1598.003](https://attack.mitre.org/techniques/T1598/003) | Spearphishing Link | Reconnaissance | PRE |
| [T1598.004](https://attack.mitre.org/techniques/T1598/004) | Spearphishing Voice | Reconnaissance | PRE |
| [T1599](https://attack.mitre.org/techniques/T1599) | Network Boundary Bridging | Defense Evasion | Network Devices |
| [T1599.001](https://attack.mitre.org/techniques/T1599/001) | Network Address Translation Traversal | Defense Evasion | Network Devices |
| [T1600](https://attack.mitre.org/techniques/T1600) | Weaken Encryption | Defense Evasion | Network Devices |
| [T1600.001](https://attack.mitre.org/techniques/T1600/001) | Reduce Key Space | Defense Evasion | Network Devices |
| [T1600.002](https://attack.mitre.org/techniques/T1600/002) | Disable Crypto Hardware | Defense Evasion | Network Devices |
| [T1601](https://attack.mitre.org/techniques/T1601) | Modify System Image | Defense Evasion | Network Devices |
| [T1601.001](https://attack.mitre.org/techniques/T1601/001) | Patch System Image | Defense Evasion | Network Devices |
| [T1601.002](https://attack.mitre.org/techniques/T1601/002) | Downgrade System Image | Defense Evasion | Network Devices |
| [T1602](https://attack.mitre.org/techniques/T1602) | Data from Configuration Repository | Collection | Network Devices |
| [T1602.001](https://attack.mitre.org/techniques/T1602/001) | SNMP (MIB Dump) | Collection | Network Devices |
| [T1602.002](https://attack.mitre.org/techniques/T1602/002) | Network Device Configuration Dump | Collection | Network Devices |
| [T1606](https://attack.mitre.org/techniques/T1606) | Forge Web Credentials | Credential Access | SaaS, Windows, macOS, Linux, IaaS, Office Suite, Identity Provider |
| [T1606.001](https://attack.mitre.org/techniques/T1606/001) | Web Cookies | Credential Access | Linux, macOS, Windows, SaaS, IaaS |
| [T1606.002](https://attack.mitre.org/techniques/T1606/002) | SAML Tokens | Credential Access | SaaS, Windows, IaaS, Office Suite, Identity Provider |
| [T1608](https://attack.mitre.org/techniques/T1608) | Stage Capabilities | Resource Development | PRE |
| [T1608.001](https://attack.mitre.org/techniques/T1608/001) | Upload Malware | Resource Development | PRE |
| [T1608.002](https://attack.mitre.org/techniques/T1608/002) | Upload Tool | Resource Development | PRE |
| [T1608.003](https://attack.mitre.org/techniques/T1608/003) | Install Digital Certificate | Resource Development | PRE |
| [T1608.004](https://attack.mitre.org/techniques/T1608/004) | Drive-by Target | Resource Development | PRE |
| [T1608.005](https://attack.mitre.org/techniques/T1608/005) | Link Target | Resource Development | PRE |
| [T1608.006](https://attack.mitre.org/techniques/T1608/006) | SEO Poisoning | Resource Development | PRE |
| [T1609](https://attack.mitre.org/techniques/T1609) | Container Administration Command | Execution | Containers |
| [T1610](https://attack.mitre.org/techniques/T1610) | Deploy Container | Defense Evasion, Execution | Containers |
| [T1611](https://attack.mitre.org/techniques/T1611) | Escape to Host | Privilege Escalation | Windows, Linux, Containers, ESXi |
| [T1612](https://attack.mitre.org/techniques/T1612) | Build Image on Host | Defense Evasion | Containers |
| [T1613](https://attack.mitre.org/techniques/T1613) | Container and Resource Discovery | Discovery | Containers |
| [T1614](https://attack.mitre.org/techniques/T1614) | System Location Discovery | Discovery | IaaS, Linux, macOS, Windows |
| [T1614.001](https://attack.mitre.org/techniques/T1614/001) | System Language Discovery | Discovery | Linux, macOS, Windows |
| [T1615](https://attack.mitre.org/techniques/T1615) | Group Policy Discovery | Discovery | Windows |
| [T1619](https://attack.mitre.org/techniques/T1619) | Cloud Storage Object Discovery | Discovery | IaaS |
| [T1620](https://attack.mitre.org/techniques/T1620) | Reflective Code Loading | Defense Evasion | Linux, macOS, Windows |
| [T1621](https://attack.mitre.org/techniques/T1621) | Multi-Factor Authentication Request Generation | Credential Access | Windows, Linux, macOS, IaaS, SaaS, Office Suite, Identity Provider |
| [T1622](https://attack.mitre.org/techniques/T1622) | Debugger Evasion | Defense Evasion, Discovery | Linux, macOS, Windows |
| [T1647](https://attack.mitre.org/techniques/T1647) | Plist File Modification | Defense Evasion | macOS |
| [T1648](https://attack.mitre.org/techniques/T1648) | Serverless Execution | Execution | SaaS, IaaS, Office Suite |
| [T1649](https://attack.mitre.org/techniques/T1649) | Steal or Forge Authentication Certificates | Credential Access | Windows, Linux, macOS, Identity Provider |
| [T1650](https://attack.mitre.org/techniques/T1650) | Acquire Access | Resource Development | PRE |
| [T1651](https://attack.mitre.org/techniques/T1651) | Cloud Administration Command | Execution | IaaS |
| [T1652](https://attack.mitre.org/techniques/T1652) | Device Driver Discovery | Discovery | Linux, macOS, Windows |
| [T1653](https://attack.mitre.org/techniques/T1653) | Power Settings | Persistence | Windows, Linux, macOS, Network Devices |
| [T1654](https://attack.mitre.org/techniques/T1654) | Log Enumeration | Discovery | ESXi, IaaS, Linux, macOS, Windows |
| [T1656](https://attack.mitre.org/techniques/T1656) | Impersonation | Defense Evasion | Linux, macOS, Office Suite, SaaS, Windows |
| [T1657](https://attack.mitre.org/techniques/T1657) | Financial Theft | Impact | Linux, macOS, Office Suite, SaaS, Windows |
| [T1659](https://attack.mitre.org/techniques/T1659) | Content Injection | Command And Control, Initial Access | Linux, macOS, Windows |
| [T1665](https://attack.mitre.org/techniques/T1665) | Hide Infrastructure | Command And Control | ESXi, Linux, Network Devices, Windows, macOS |
| [T1666](https://attack.mitre.org/techniques/T1666) | Modify Cloud Resource Hierarchy | Defense Evasion | IaaS |
| [T1667](https://attack.mitre.org/techniques/T1667) | Email Bombing | Impact | Linux, Office Suite, Windows, macOS |
| [T1668](https://attack.mitre.org/techniques/T1668) | Exclusive Control | Persistence | Linux, macOS, Windows |
| [T1669](https://attack.mitre.org/techniques/T1669) | Wi-Fi Networks | Initial Access | Linux, Network Devices, Windows, macOS |
| [T1671](https://attack.mitre.org/techniques/T1671) | Cloud Application Integration | Persistence | Office Suite, SaaS |
| [T1672](https://attack.mitre.org/techniques/T1672) | Email Spoofing | Defense Evasion | Office Suite, Windows, macOS, Linux |
| [T1673](https://attack.mitre.org/techniques/T1673) | Virtual Machine Discovery | Discovery | ESXi, Linux, macOS, Windows |
| [T1674](https://attack.mitre.org/techniques/T1674) | Input Injection | Execution | Windows, macOS, Linux |
| [T1675](https://attack.mitre.org/techniques/T1675) | ESXi Administration Command | Execution | ESXi |
| [T1677](https://attack.mitre.org/techniques/T1677) | Poisoned Pipeline Execution | Execution | SaaS |
| [T1678](https://attack.mitre.org/techniques/T1678) | Delay Execution | Defense Evasion | Linux, macOS, Windows |
| [T1679](https://attack.mitre.org/techniques/T1679) | Selective Exclusion | Defense Evasion | Windows |
| [T1680](https://attack.mitre.org/techniques/T1680) | Local Storage Discovery | Discovery | ESXi, IaaS, Linux, macOS, Windows |
| [T1681](https://attack.mitre.org/techniques/T1681) | Search Threat Vendor Data | Reconnaissance | PRE |

---

## Techniques by Tactic

### Reconnaissance

*45 techniques (11 parent, 34 sub-techniques)*

| T-Code | Name | Description |
|--------|------|-------------|
| [T1589](https://attack.mitre.org/techniques/T1589) | Gather Victim Identity Information | Adversaries may gather information about the victim's identity that can be used during targeting. Information about identities may include a variety of details, including personal data (ex: employee... |
| [T1589.001](https://attack.mitre.org/techniques/T1589/001) | ↳ Credentials | Adversaries may gather credentials that can be used during targeting. Account credentials gathered by adversaries may be those directly associated with the target victim organization or attempt to... |
| [T1589.002](https://attack.mitre.org/techniques/T1589/002) | ↳ Email Addresses | Adversaries may gather email addresses that can be used during targeting. Even if internal instances exist, organizations may have public-facing email infrastructure and addresses for employees.... |
| [T1589.003](https://attack.mitre.org/techniques/T1589/003) | ↳ Employee Names | Adversaries may gather employee names that can be used during targeting. Employee names be used to derive email addresses as well as to help guide other reconnaissance efforts and/or craft... |
| [T1590](https://attack.mitre.org/techniques/T1590) | Gather Victim Network Information | Adversaries may gather information about the victim's networks that can be used during targeting. Information about networks may include a variety of details, including administrative data (ex: IP... |
| [T1590.001](https://attack.mitre.org/techniques/T1590/001) | ↳ Domain Properties | Adversaries may gather information about the victim's network domain(s) that can be used during targeting. Information about domains and their properties may include a variety of details, including... |
| [T1590.002](https://attack.mitre.org/techniques/T1590/002) | ↳ DNS | Adversaries may gather information about the victim's DNS that can be used during targeting. DNS information may include a variety of details, including registered name servers as well as records... |
| [T1590.003](https://attack.mitre.org/techniques/T1590/003) | ↳ Network Trust Dependencies | Adversaries may gather information about the victim's network trust dependencies that can be used during targeting. Information about network trusts may include a variety of details, including second... |
| [T1590.004](https://attack.mitre.org/techniques/T1590/004) | ↳ Network Topology | Adversaries may gather information about the victim's network topology that can be used during targeting. Information about network topologies may include a variety of details, including the physical... |
| [T1590.005](https://attack.mitre.org/techniques/T1590/005) | ↳ IP Addresses | Adversaries may gather the victim's IP addresses that can be used during targeting. Public IP addresses may be allocated to organizations by block, or a range of sequential addresses. Information... |
| [T1590.006](https://attack.mitre.org/techniques/T1590/006) | ↳ Network Security Appliances | Adversaries may gather information about the victim's network security appliances that can be used during targeting. Information about network security appliances may include a variety of details,... |
| [T1591](https://attack.mitre.org/techniques/T1591) | Gather Victim Org Information | Adversaries may gather information about the victim's organization that can be used during targeting. Information about an organization may include a variety of details, including the names of... |
| [T1591.001](https://attack.mitre.org/techniques/T1591/001) | ↳ Determine Physical Locations | Adversaries may gather the victim's physical location(s) that can be used during targeting. Information about physical locations of a target organization may include a variety of details, including... |
| [T1591.002](https://attack.mitre.org/techniques/T1591/002) | ↳ Business Relationships | Adversaries may gather information about the victim's business relationships that can be used during targeting. Information about an organization’s business relationships may include a variety of... |
| [T1591.003](https://attack.mitre.org/techniques/T1591/003) | ↳ Identify Business Tempo | Adversaries may gather information about the victim's business tempo that can be used during targeting. Information about an organization’s business tempo may include a variety of details, including... |
| [T1591.004](https://attack.mitre.org/techniques/T1591/004) | ↳ Identify Roles | Adversaries may gather information about identities and roles within the victim organization that can be used during targeting. Information about business roles may reveal a variety of targetable... |
| [T1592](https://attack.mitre.org/techniques/T1592) | Gather Victim Host Information | Adversaries may gather information about the victim's hosts that can be used during targeting. Information about hosts may include a variety of details, including administrative data (ex: name,... |
| [T1592.001](https://attack.mitre.org/techniques/T1592/001) | ↳ Hardware | Adversaries may gather information about the victim's host hardware that can be used during targeting. Information about hardware infrastructure may include a variety of details such as types and... |
| [T1592.002](https://attack.mitre.org/techniques/T1592/002) | ↳ Software | Adversaries may gather information about the victim's host software that can be used during targeting. Information about installed software may include a variety of details such as types and versions... |
| [T1592.003](https://attack.mitre.org/techniques/T1592/003) | ↳ Firmware | Adversaries may gather information about the victim's host firmware that can be used during targeting. Information about host firmware may include a variety of details such as type and versions on... |
| [T1592.004](https://attack.mitre.org/techniques/T1592/004) | ↳ Client Configurations | Adversaries may gather information about the victim's client configurations that can be used during targeting. Information about client configurations may include a variety of details and settings,... |
| [T1593](https://attack.mitre.org/techniques/T1593) | Search Open Websites/Domains | Adversaries may search freely available websites and/or domains for information about victims that can be used during targeting. Information about victims may be available in various online sites,... |
| [T1593.001](https://attack.mitre.org/techniques/T1593/001) | ↳ Social Media | Adversaries may search social media for information about victims that can be used during targeting. Social media sites may contain various information about a victim organization, such as business... |
| [T1593.002](https://attack.mitre.org/techniques/T1593/002) | ↳ Search Engines | Adversaries may use search engines to collect information about victims that can be used during targeting. Search engine services typical crawl online sites to index context and may provide users... |
| [T1593.003](https://attack.mitre.org/techniques/T1593/003) | ↳ Code Repositories | Adversaries may search public code repositories for information about victims that can be used during targeting. Victims may store code in repositories on various third-party websites such as GitHub,... |
| [T1594](https://attack.mitre.org/techniques/T1594) | Search Victim-Owned Websites | Adversaries may search websites owned by the victim for information that can be used during targeting. Victim-owned websites may contain a variety of details, including names of... |
| [T1595](https://attack.mitre.org/techniques/T1595) | Active Scanning | Adversaries may execute active reconnaissance scans to gather information that can be used during targeting. Active scans are those where the adversary probes victim infrastructure via network... |
| [T1595.001](https://attack.mitre.org/techniques/T1595/001) | ↳ Scanning IP Blocks | Adversaries may scan victim IP blocks to gather information that can be used during targeting. Public IP addresses may be allocated to organizations by block, or a range of sequential addresses.... |
| [T1595.002](https://attack.mitre.org/techniques/T1595/002) | ↳ Vulnerability Scanning | Adversaries may scan victims for vulnerabilities that can be used during targeting. Vulnerability scans typically check if the configuration of a target host/application (ex: software and version)... |
| [T1595.003](https://attack.mitre.org/techniques/T1595/003) | ↳ Wordlist Scanning | Adversaries may iteratively probe infrastructure using brute-forcing and crawling techniques. While this technique employs similar methods to [Brute Force](https://attack.mitre.org/techniques/T1110),... |
| [T1596](https://attack.mitre.org/techniques/T1596) | Search Open Technical Databases | Adversaries may search freely available technical databases for information about victims that can be used during targeting. Information about victims may be available in online databases and... |
| [T1596.001](https://attack.mitre.org/techniques/T1596/001) | ↳ DNS/Passive DNS | Adversaries may search DNS data for information about victims that can be used during targeting. DNS information may include a variety of details, including registered name servers as well as records... |
| [T1596.002](https://attack.mitre.org/techniques/T1596/002) | ↳ WHOIS | Adversaries may search public WHOIS data for information about victims that can be used during targeting. WHOIS data is stored by regional Internet registries (RIR) responsible for allocating and... |
| [T1596.003](https://attack.mitre.org/techniques/T1596/003) | ↳ Digital Certificates | Adversaries may search public digital certificate data for information about victims that can be used during targeting. Digital certificates are issued by a certificate authority (CA) in order to... |
| [T1596.004](https://attack.mitre.org/techniques/T1596/004) | ↳ CDNs | Adversaries may search content delivery network (CDN) data about victims that can be used during targeting. CDNs allow an organization to host content from a distributed, load balanced array of... |
| [T1596.005](https://attack.mitre.org/techniques/T1596/005) | ↳ Scan Databases | Adversaries may search within public scan databases for information about victims that can be used during targeting. Various online services continuously publish the results of Internet... |
| [T1597](https://attack.mitre.org/techniques/T1597) | Search Closed Sources | Adversaries may search and gather information about victims from closed (e.g., paid, private, or otherwise not freely available) sources that can be used during targeting. Information about victims... |
| [T1597.001](https://attack.mitre.org/techniques/T1597/001) | ↳ Threat Intel Vendors | Adversaries may search private data from threat intelligence vendors for information that can be used during targeting. Threat intelligence vendors may offer paid feeds or portals that offer more... |
| [T1597.002](https://attack.mitre.org/techniques/T1597/002) | ↳ Purchase Technical Data | Adversaries may purchase technical information about victims that can be used during targeting. Information about victims may be available for purchase within reputable private sources and databases,... |
| [T1598](https://attack.mitre.org/techniques/T1598) | Phishing for Information | Adversaries may send phishing messages to elicit sensitive information that can be used during targeting. Phishing for information is an attempt to trick targets into divulging information,... |
| [T1598.001](https://attack.mitre.org/techniques/T1598/001) | ↳ Spearphishing Service | Adversaries may send spearphishing messages via third-party services to elicit sensitive information that can be used during targeting. Spearphishing for information is an attempt to trick targets... |
| [T1598.002](https://attack.mitre.org/techniques/T1598/002) | ↳ Spearphishing Attachment | Adversaries may send spearphishing messages with a malicious attachment to elicit sensitive information that can be used during targeting. Spearphishing for information is an attempt to trick targets... |
| [T1598.003](https://attack.mitre.org/techniques/T1598/003) | ↳ Spearphishing Link | Adversaries may send spearphishing messages with a malicious link to elicit sensitive information that can be used during targeting. Spearphishing for information is an attempt to trick targets into... |
| [T1598.004](https://attack.mitre.org/techniques/T1598/004) | ↳ Spearphishing Voice | Adversaries may use voice communications to elicit sensitive information that can be used during targeting. Spearphishing for information is an attempt to trick targets into divulging information,... |
| [T1681](https://attack.mitre.org/techniques/T1681) | Search Threat Vendor Data | Threat actors may seek information/indicators from closed or open threat intelligence sources gathered about their own campaigns, as well as those conducted by other adversaries that may align with... |

---

### Resource Development

*47 techniques (8 parent, 39 sub-techniques)*

| T-Code | Name | Description |
|--------|------|-------------|
| [T1583](https://attack.mitre.org/techniques/T1583) | Acquire Infrastructure | Adversaries may buy, lease, rent, or obtain infrastructure that can be used during targeting. A wide variety of infrastructure exists for hosting and orchestrating adversary operations.... |
| [T1583.001](https://attack.mitre.org/techniques/T1583/001) | ↳ Domains | Adversaries may acquire domains that can be used during targeting. Domain names are the human readable names used to represent one or more IP addresses. They can be purchased or, in some cases,... |
| [T1583.002](https://attack.mitre.org/techniques/T1583/002) | ↳ DNS Server | Adversaries may set up their own Domain Name System (DNS) servers that can be used during targeting. During post-compromise activity, adversaries may utilize DNS traffic for various tasks, including... |
| [T1583.003](https://attack.mitre.org/techniques/T1583/003) | ↳ Virtual Private Server | Adversaries may rent Virtual Private Servers (VPSs) that can be used during targeting. There exist a variety of cloud service providers that will sell virtual machines/containers as a service. By... |
| [T1583.004](https://attack.mitre.org/techniques/T1583/004) | ↳ Server | Adversaries may buy, lease, rent, or obtain physical servers that can be used during targeting. Use of servers allows an adversary to stage, launch, and execute an operation. During post-compromise... |
| [T1583.005](https://attack.mitre.org/techniques/T1583/005) | ↳ Botnet | Adversaries may buy, lease, or rent a network of compromised systems that can be used during targeting. A botnet is a network of compromised systems that can be instructed to perform coordinated... |
| [T1583.006](https://attack.mitre.org/techniques/T1583/006) | ↳ Web Services | Adversaries may register for web services that can be used during targeting. A variety of popular websites exist for adversaries to register for a web-based service that can be abused during later... |
| [T1583.007](https://attack.mitre.org/techniques/T1583/007) | ↳ Serverless | Adversaries may purchase and configure serverless cloud infrastructure, such as Cloudflare Workers, AWS Lambda functions, or Google Apps Scripts, that can be used during targeting. By utilizing... |
| [T1583.008](https://attack.mitre.org/techniques/T1583/008) | ↳ Malvertising | Adversaries may purchase online advertisements that can be abused to distribute malware to victims. Ads can be purchased to plant as well as favorably position artifacts in specific locations online,... |
| [T1584](https://attack.mitre.org/techniques/T1584) | Compromise Infrastructure | Adversaries may compromise third-party infrastructure that can be used during targeting. Infrastructure solutions include physical or cloud servers, domains, network devices, and third-party web and... |
| [T1584.001](https://attack.mitre.org/techniques/T1584/001) | ↳ Domains | Adversaries may hijack domains and/or subdomains that can be used during targeting. Domain registration hijacking is the act of changing the registration of a domain name without the permission of... |
| [T1584.002](https://attack.mitre.org/techniques/T1584/002) | ↳ DNS Server | Adversaries may compromise third-party DNS servers that can be used during targeting. During post-compromise activity, adversaries may utilize DNS traffic for various tasks, including for Command and... |
| [T1584.003](https://attack.mitre.org/techniques/T1584/003) | ↳ Virtual Private Server | Adversaries may compromise third-party Virtual Private Servers (VPSs) that can be used during targeting. There exist a variety of cloud service providers that will sell virtual machines/containers as... |
| [T1584.004](https://attack.mitre.org/techniques/T1584/004) | ↳ Server | Adversaries may compromise third-party servers that can be used during targeting. Use of servers allows an adversary to stage, launch, and execute an operation. During post-compromise activity,... |
| [T1584.005](https://attack.mitre.org/techniques/T1584/005) | ↳ Botnet | Adversaries may compromise numerous third-party systems to form a botnet that can be used during targeting. A botnet is a network of compromised systems that can be instructed to perform coordinated... |
| [T1584.006](https://attack.mitre.org/techniques/T1584/006) | ↳ Web Services | Adversaries may compromise access to third-party web services that can be used during targeting. A variety of popular websites exist for legitimate users to register for web-based services, such as... |
| [T1584.007](https://attack.mitre.org/techniques/T1584/007) | ↳ Serverless | Adversaries may compromise serverless cloud infrastructure, such as Cloudflare Workers, AWS Lambda functions, or Google Apps Scripts, that can be used during targeting. By utilizing serverless... |
| [T1584.008](https://attack.mitre.org/techniques/T1584/008) | ↳ Network Devices | Adversaries may compromise third-party network devices that can be used during targeting. Network devices, such as small office/home office (SOHO) routers, may be compromised where the adversary's... |
| [T1585](https://attack.mitre.org/techniques/T1585) | Establish Accounts | Adversaries may create and cultivate accounts with services that can be used during targeting. Adversaries can create accounts that can be used to build a persona to further operations. Persona... |
| [T1585.001](https://attack.mitre.org/techniques/T1585/001) | ↳ Social Media Accounts | Adversaries may create and cultivate social media accounts that can be used during targeting. Adversaries can create social media accounts that can be used to build a persona to further operations.... |
| [T1585.002](https://attack.mitre.org/techniques/T1585/002) | ↳ Email Accounts | Adversaries may create email accounts that can be used during targeting. Adversaries can use accounts created with email providers to further their operations, such as leveraging them to conduct... |
| [T1585.003](https://attack.mitre.org/techniques/T1585/003) | ↳ Cloud Accounts | Adversaries may create accounts with cloud providers that can be used during targeting. Adversaries can use cloud accounts to further their operations, including leveraging cloud storage services... |
| [T1586](https://attack.mitre.org/techniques/T1586) | Compromise Accounts | Adversaries may compromise accounts with services that can be used during targeting. For operations incorporating social engineering, the utilization of an online persona may be important. Rather... |
| [T1586.001](https://attack.mitre.org/techniques/T1586/001) | ↳ Social Media Accounts | Adversaries may compromise social media accounts that can be used during targeting. For operations incorporating social engineering, the utilization of an online persona may be important. Rather than... |
| [T1586.002](https://attack.mitre.org/techniques/T1586/002) | ↳ Email Accounts | Adversaries may compromise email accounts that can be used during targeting. Adversaries can use compromised email accounts to further their operations, such as leveraging them to conduct [Phishing... |
| [T1586.003](https://attack.mitre.org/techniques/T1586/003) | ↳ Cloud Accounts | Adversaries may compromise cloud accounts that can be used during targeting. Adversaries can use compromised cloud accounts to further their operations, including leveraging cloud storage services... |
| [T1587](https://attack.mitre.org/techniques/T1587) | Develop Capabilities | Adversaries may build capabilities that can be used during targeting. Rather than purchasing, freely downloading, or stealing capabilities, adversaries may develop their own capabilities in-house.... |
| [T1587.001](https://attack.mitre.org/techniques/T1587/001) | ↳ Malware | Adversaries may develop malware and malware components that can be used during targeting. Building malicious software can include the development of payloads, droppers, post-compromise tools,... |
| [T1587.002](https://attack.mitre.org/techniques/T1587/002) | ↳ Code Signing Certificates | Adversaries may create self-signed code signing certificates that can be used during targeting. Code signing is the process of digitally signing executables and scripts to confirm the software author... |
| [T1587.003](https://attack.mitre.org/techniques/T1587/003) | ↳ Digital Certificates | Adversaries may create self-signed SSL/TLS certificates that can be used during targeting. SSL/TLS certificates are designed to instill trust. They include information about the key, information... |
| [T1587.004](https://attack.mitre.org/techniques/T1587/004) | ↳ Exploits | Adversaries may develop exploits that can be used during targeting. An exploit takes advantage of a bug or vulnerability in order to cause unintended or unanticipated behavior to occur on computer... |
| [T1588](https://attack.mitre.org/techniques/T1588) | Obtain Capabilities | Adversaries may buy and/or steal capabilities that can be used during targeting. Rather than developing their own capabilities in-house, adversaries may purchase, freely download, or steal them.... |
| [T1588.001](https://attack.mitre.org/techniques/T1588/001) | ↳ Malware | Adversaries may buy, steal, or download malware that can be used during targeting. Malicious software can include payloads, droppers, post-compromise tools, backdoors, packers, and C2 protocols.... |
| [T1588.002](https://attack.mitre.org/techniques/T1588/002) | ↳ Tool | Adversaries may buy, steal, or download software tools that can be used during targeting. Tools can be open or closed source, free or commercial. A tool can be used for malicious purposes by an... |
| [T1588.003](https://attack.mitre.org/techniques/T1588/003) | ↳ Code Signing Certificates | Adversaries may buy and/or steal code signing certificates that can be used during targeting. Code signing is the process of digitally signing executables and scripts to confirm the software author... |
| [T1588.004](https://attack.mitre.org/techniques/T1588/004) | ↳ Digital Certificates | Adversaries may buy and/or steal SSL/TLS certificates that can be used during targeting. SSL/TLS certificates are designed to instill trust. They include information about the key, information about... |
| [T1588.005](https://attack.mitre.org/techniques/T1588/005) | ↳ Exploits | Adversaries may buy, steal, or download exploits that can be used during targeting. An exploit takes advantage of a bug or vulnerability in order to cause unintended or unanticipated behavior to... |
| [T1588.006](https://attack.mitre.org/techniques/T1588/006) | ↳ Vulnerabilities | Adversaries may acquire information about vulnerabilities that can be used during targeting. A vulnerability is a weakness in computer hardware or software that can, potentially, be exploited by an... |
| [T1588.007](https://attack.mitre.org/techniques/T1588/007) | ↳ Artificial Intelligence | Adversaries may obtain access to generative artificial intelligence tools, such as large language models (LLMs), to aid various techniques during targeting. These tools may be used to inform,... |
| [T1608](https://attack.mitre.org/techniques/T1608) | Stage Capabilities | Adversaries may upload, install, or otherwise set up capabilities that can be used during targeting. To support their operations, an adversary may need to take capabilities they developed ([Develop... |
| [T1608.001](https://attack.mitre.org/techniques/T1608/001) | ↳ Upload Malware | Adversaries may upload malware to third-party or adversary controlled infrastructure to make it accessible during targeting. Malicious software can include payloads, droppers, post-compromise tools,... |
| [T1608.002](https://attack.mitre.org/techniques/T1608/002) | ↳ Upload Tool | Adversaries may upload tools to third-party or adversary controlled infrastructure to make it accessible during targeting. Tools can be open or closed source, free or commercial. Tools can be used... |
| [T1608.003](https://attack.mitre.org/techniques/T1608/003) | ↳ Install Digital Certificate | Adversaries may install SSL/TLS certificates that can be used during targeting. SSL/TLS certificates are files that can be installed on servers to enable secure communications between systems.... |
| [T1608.004](https://attack.mitre.org/techniques/T1608/004) | ↳ Drive-by Target | Adversaries may prepare an operational environment to infect systems that visit a website over the normal course of browsing. Endpoint systems may be compromised through browsing to adversary... |
| [T1608.005](https://attack.mitre.org/techniques/T1608/005) | ↳ Link Target | Adversaries may put in place resources that are referenced by a link that can be used during targeting. An adversary may rely upon a user clicking a malicious link in order to divulge information... |
| [T1608.006](https://attack.mitre.org/techniques/T1608/006) | ↳ SEO Poisoning | Adversaries may poison mechanisms that influence search engine optimization (SEO) to further lure staged capabilities towards potential victims. Search engines typically display results to users... |
| [T1650](https://attack.mitre.org/techniques/T1650) | Acquire Access | Adversaries may purchase or otherwise acquire an existing access to a target system or network. A variety of online services and initial access broker networks are available to sell access to... |

---

### Initial Access

*22 techniques (11 parent, 11 sub-techniques)*

| T-Code | Name | Description |
|--------|------|-------------|
| [T1078](https://attack.mitre.org/techniques/T1078) | Valid Accounts | Adversaries may obtain and abuse credentials of existing accounts as a means of gaining Initial Access, Persistence, Privilege Escalation, or Defense Evasion. Compromised credentials may be used to... |
| [T1078.001](https://attack.mitre.org/techniques/T1078/001) | ↳ Default Accounts | Adversaries may obtain and abuse credentials of a default account as a means of gaining Initial Access, Persistence, Privilege Escalation, or Defense Evasion. Default accounts are those that are... |
| [T1078.002](https://attack.mitre.org/techniques/T1078/002) | ↳ Domain Accounts | Adversaries may obtain and abuse credentials of a domain account as a means of gaining Initial Access, Persistence, Privilege Escalation, or Defense Evasion.(Citation: TechNet Credential Theft)... |
| [T1078.003](https://attack.mitre.org/techniques/T1078/003) | ↳ Local Accounts | Adversaries may obtain and abuse credentials of a local account as a means of gaining Initial Access, Persistence, Privilege Escalation, or Defense Evasion. Local accounts are those configured by an... |
| [T1078.004](https://attack.mitre.org/techniques/T1078/004) | ↳ Cloud Accounts | Valid accounts in cloud environments may allow adversaries to perform actions to achieve Initial Access, Persistence, Privilege Escalation, or Defense Evasion. Cloud accounts are those created and... |
| [T1091](https://attack.mitre.org/techniques/T1091) | Replication Through Removable Media | Adversaries may move onto systems, possibly those on disconnected or air-gapped networks, by copying malware to removable media and taking advantage of Autorun features when the media is inserted... |
| [T1133](https://attack.mitre.org/techniques/T1133) | External Remote Services | Adversaries may leverage external-facing remote services to initially access and/or persist within a network. Remote services such as VPNs, Citrix, and other access mechanisms allow users to connect... |
| [T1189](https://attack.mitre.org/techniques/T1189) | Drive-by Compromise | Adversaries may gain access to a system through a user visiting a website over the normal course of browsing. Multiple ways of delivering exploit code to a browser exist (i.e., [Drive-by... |
| [T1190](https://attack.mitre.org/techniques/T1190) | Exploit Public-Facing Application | Adversaries may attempt to exploit a weakness in an Internet-facing host or system to initially access a network. The weakness in the system can be a software bug, a temporary glitch, or a... |
| [T1195](https://attack.mitre.org/techniques/T1195) | Supply Chain Compromise | Adversaries may manipulate products or product delivery mechanisms prior to receipt by a final consumer for the purpose of data or system compromise. Supply chain compromise can take place at any... |
| [T1195.001](https://attack.mitre.org/techniques/T1195/001) | ↳ Compromise Software Dependencies and Development Tools | Adversaries may manipulate software dependencies and development tools prior to receipt by a final consumer for the purpose of data or system compromise. Applications often depend on external... |
| [T1195.002](https://attack.mitre.org/techniques/T1195/002) | ↳ Compromise Software Supply Chain | Adversaries may manipulate application software prior to receipt by a final consumer for the purpose of data or system compromise. Supply chain compromise of software can take place in a number of... |
| [T1195.003](https://attack.mitre.org/techniques/T1195/003) | ↳ Compromise Hardware Supply Chain | Adversaries may manipulate hardware components in products prior to receipt by a final consumer for the purpose of data or system compromise. By modifying hardware or firmware in the supply chain,... |
| [T1199](https://attack.mitre.org/techniques/T1199) | Trusted Relationship | Adversaries may breach or otherwise leverage organizations who have access to intended victims. Access through trusted third party relationship abuses an existing connection that may not be protected... |
| [T1200](https://attack.mitre.org/techniques/T1200) | Hardware Additions | Adversaries may physically introduce computer accessories, networking hardware, or other computing devices into a system or network that can be used as a vector to gain access. Rather than just... |
| [T1566](https://attack.mitre.org/techniques/T1566) | Phishing | Adversaries may send phishing messages to gain access to victim systems. All forms of phishing are electronically delivered social engineering. Phishing can be targeted, known as spearphishing. In... |
| [T1566.001](https://attack.mitre.org/techniques/T1566/001) | ↳ Spearphishing Attachment | Adversaries may send spearphishing emails with a malicious attachment in an attempt to gain access to victim systems. Spearphishing attachment is a specific variant of spearphishing. Spearphishing... |
| [T1566.002](https://attack.mitre.org/techniques/T1566/002) | ↳ Spearphishing Link | Adversaries may send spearphishing emails with a malicious link in an attempt to gain access to victim systems. Spearphishing with a link is a specific variant of spearphishing. It is different from... |
| [T1566.003](https://attack.mitre.org/techniques/T1566/003) | ↳ Spearphishing via Service | Adversaries may send spearphishing messages via third-party services in an attempt to gain access to victim systems. Spearphishing via service is a specific variant of spearphishing. It is different... |
| [T1566.004](https://attack.mitre.org/techniques/T1566/004) | ↳ Spearphishing Voice | Adversaries may use voice communications to ultimately gain access to victim systems. Spearphishing voice is a specific variant of spearphishing. It is different from other forms of spearphishing in... |
| [T1659](https://attack.mitre.org/techniques/T1659) | Content Injection | Adversaries may gain access and continuously communicate with victims by injecting malicious content into systems through online network traffic. Rather than luring victims to malicious payloads... |
| [T1669](https://attack.mitre.org/techniques/T1669) | Wi-Fi Networks | Adversaries may gain initial access to target systems by connecting to wireless networks. They may accomplish this by exploiting open Wi-Fi networks used by target devices or by accessing secured... |

---

### Execution

*46 techniques (17 parent, 29 sub-techniques)*

| T-Code | Name | Description |
|--------|------|-------------|
| [T1047](https://attack.mitre.org/techniques/T1047) | Windows Management Instrumentation | Adversaries may abuse Windows Management Instrumentation (WMI) to execute malicious commands and payloads. WMI is designed for programmers and is the infrastructure for management data and operations... |
| [T1053](https://attack.mitre.org/techniques/T1053) | Scheduled Task/Job | Adversaries may abuse task scheduling functionality to facilitate initial or recurring execution of malicious code. Utilities exist within all major operating systems to schedule programs or scripts... |
| [T1053.002](https://attack.mitre.org/techniques/T1053/002) | ↳ At | Adversaries may abuse the [at](https://attack.mitre.org/software/S0110) utility to perform task scheduling for initial or recurring execution of malicious code. The... |
| [T1053.003](https://attack.mitre.org/techniques/T1053/003) | ↳ Cron | Adversaries may abuse the <code>cron</code> utility to perform task scheduling for initial or recurring execution of malicious code.(Citation: 20 macOS Common Tools and Techniques) The... |
| [T1053.005](https://attack.mitre.org/techniques/T1053/005) | ↳ Scheduled Task | Adversaries may abuse the Windows Task Scheduler to perform task scheduling for initial or recurring execution of malicious code. There are multiple ways to access the Task Scheduler in Windows. The... |
| [T1053.006](https://attack.mitre.org/techniques/T1053/006) | ↳ Systemd Timers | Adversaries may abuse systemd timers to perform task scheduling for initial or recurring execution of malicious code. Systemd timers are unit files with file extension <code>.timer</code> that... |
| [T1053.007](https://attack.mitre.org/techniques/T1053/007) | ↳ Container Orchestration Job | Adversaries may abuse task scheduling functionality provided by container orchestration tools such as Kubernetes to schedule deployment of containers configured to execute malicious code. Container... |
| [T1059](https://attack.mitre.org/techniques/T1059) | Command and Scripting Interpreter | Adversaries may abuse command and script interpreters to execute commands, scripts, or binaries. These interfaces and languages provide ways of interacting with computer systems and are a common... |
| [T1059.001](https://attack.mitre.org/techniques/T1059/001) | ↳ PowerShell | Adversaries may abuse PowerShell commands and scripts for execution. PowerShell is a powerful interactive command-line interface and scripting environment included in the Windows operating... |
| [T1059.002](https://attack.mitre.org/techniques/T1059/002) | ↳ AppleScript | Adversaries may abuse AppleScript for execution. AppleScript is a macOS scripting language designed to control applications and parts of the OS via inter-application messages called... |
| [T1059.003](https://attack.mitre.org/techniques/T1059/003) | ↳ Windows Command Shell | Adversaries may abuse the Windows command shell for execution. The Windows command shell ([cmd](https://attack.mitre.org/software/S0106)) is the primary command prompt on Windows systems. The Windows... |
| [T1059.004](https://attack.mitre.org/techniques/T1059/004) | ↳ Unix Shell | Adversaries may abuse Unix shell commands and scripts for execution. Unix shells are the primary command prompt on Linux, macOS, and ESXi systems, though many variations of the Unix shell exist (e.g.... |
| [T1059.005](https://attack.mitre.org/techniques/T1059/005) | ↳ Visual Basic | Adversaries may abuse Visual Basic (VB) for execution. VB is a programming language created by Microsoft with interoperability with many Windows technologies such as [Component Object... |
| [T1059.006](https://attack.mitre.org/techniques/T1059/006) | ↳ Python | Adversaries may abuse Python commands and scripts for execution. Python is a very popular scripting/programming language, with capabilities to perform many functions. Python can be executed... |
| [T1059.007](https://attack.mitre.org/techniques/T1059/007) | ↳ JavaScript | Adversaries may abuse various implementations of JavaScript for execution. JavaScript (JS) is a platform-independent scripting language (compiled just-in-time at runtime) commonly associated with... |
| [T1059.008](https://attack.mitre.org/techniques/T1059/008) | ↳ Network Device CLI | Adversaries may abuse scripting or built-in command line interpreters (CLI) on network devices to execute malicious command and payloads. The CLI is the primary means through which users and... |
| [T1059.009](https://attack.mitre.org/techniques/T1059/009) | ↳ Cloud API | Adversaries may abuse cloud APIs to execute malicious commands. APIs available in cloud environments provide various functionalities and are a feature-rich method for programmatic access to nearly... |
| [T1059.010](https://attack.mitre.org/techniques/T1059/010) | ↳ AutoHotKey & AutoIT | Adversaries may execute commands and perform malicious tasks using AutoIT and AutoHotKey automation scripts. AutoIT and AutoHotkey (AHK) are scripting languages that enable users to automate Windows... |
| [T1059.011](https://attack.mitre.org/techniques/T1059/011) | ↳ Lua | Adversaries may abuse Lua commands and scripts for execution. Lua is a cross-platform scripting and programming language primarily designed for embedded use in applications. Lua can be executed on... |
| [T1059.012](https://attack.mitre.org/techniques/T1059/012) | ↳ Hypervisor CLI | Adversaries may abuse hypervisor command line interpreters (CLIs) to execute malicious commands. Hypervisor CLIs typically enable a wide variety of functionality for managing both the hypervisor... |
| [T1059.013](https://attack.mitre.org/techniques/T1059/013) | ↳ Container CLI/API | Adversaries may abuse built-in CLI tools or API calls to execute malicious commands in containerized environments. The Docker CLI is used for managing containers via an exposed API point from the... |
| [T1072](https://attack.mitre.org/techniques/T1072) | Software Deployment Tools | Adversaries may gain access to and use centralized software suites installed within an enterprise to execute commands and move laterally through the network. Configuration management and software... |
| [T1106](https://attack.mitre.org/techniques/T1106) | Native API | Adversaries may interact with the native OS application programming interface (API) to execute behaviors. Native APIs provide a controlled means of calling low-level OS services within the kernel,... |
| [T1129](https://attack.mitre.org/techniques/T1129) | Shared Modules | Adversaries may execute malicious payloads via loading shared modules. Shared modules are executable files that are loaded into processes to provide access to reusable code, such as specific custom... |
| [T1203](https://attack.mitre.org/techniques/T1203) | Exploitation for Client Execution | Adversaries may exploit software vulnerabilities in client applications to execute code. Vulnerabilities can exist in software due to unsecure coding practices that can lead to unanticipated... |
| [T1204](https://attack.mitre.org/techniques/T1204) | User Execution | An adversary may rely upon specific actions by a user in order to gain execution. Users may be subjected to social engineering to get them to execute malicious code by, for example, opening a... |
| [T1204.001](https://attack.mitre.org/techniques/T1204/001) | ↳ Malicious Link | An adversary may rely upon a user clicking a malicious link in order to gain execution. Users may be subjected to social engineering to get them to click on a link that will lead to code execution.... |
| [T1204.002](https://attack.mitre.org/techniques/T1204/002) | ↳ Malicious File | An adversary may rely upon a user opening a malicious file in order to gain execution. Users may be subjected to social engineering to get them to open a file that will lead to code execution. This... |
| [T1204.003](https://attack.mitre.org/techniques/T1204/003) | ↳ Malicious Image | Adversaries may rely on a user running a malicious image to facilitate execution. Amazon Web Services (AWS) Amazon Machine Images (AMIs), Google Cloud Platform (GCP) Images, and Azure Images as well... |
| [T1204.004](https://attack.mitre.org/techniques/T1204/004) | ↳ Malicious Copy and Paste | An adversary may rely upon a user copying and pasting code in order to gain execution. Users may be subjected to social engineering to get them to copy and paste code directly into a [Command and... |
| [T1204.005](https://attack.mitre.org/techniques/T1204/005) | ↳ Malicious Library | Adversaries may rely on a user installing a malicious library to facilitate execution. Threat actors may [Upload Malware](https://attack.mitre.org/techniques/T1608/001) to package managers such as... |
| [T1559](https://attack.mitre.org/techniques/T1559) | Inter-Process Communication | Adversaries may abuse inter-process communication (IPC) mechanisms for local code or command execution. IPC is typically used by processes to share data, communicate with each other, or synchronize... |
| [T1559.001](https://attack.mitre.org/techniques/T1559/001) | ↳ Component Object Model | Adversaries may use the Windows Component Object Model (COM) for local code execution. COM is an inter-process communication (IPC) component of the native Windows application programming interface... |
| [T1559.002](https://attack.mitre.org/techniques/T1559/002) | ↳ Dynamic Data Exchange | Adversaries may use Windows Dynamic Data Exchange (DDE) to execute arbitrary commands. DDE is a client-server protocol for one-time and/or continuous inter-process communication (IPC) between... |
| [T1559.003](https://attack.mitre.org/techniques/T1559/003) | ↳ XPC Services | Adversaries can provide malicious content to an XPC service daemon for local code execution. macOS uses XPC services for basic inter-process communication between various processes, such as between... |
| [T1569](https://attack.mitre.org/techniques/T1569) | System Services | Adversaries may abuse system services or daemons to execute commands or programs. Adversaries can execute malicious content by interacting with or creating services either locally or remotely. Many... |
| [T1569.001](https://attack.mitre.org/techniques/T1569/001) | ↳ Launchctl | Adversaries may abuse launchctl to execute commands or programs. Launchctl interfaces with launchd, the service management framework for macOS. Launchctl supports taking subcommands on the... |
| [T1569.002](https://attack.mitre.org/techniques/T1569/002) | ↳ Service Execution | Adversaries may abuse the Windows service control manager to execute malicious commands or payloads. The Windows service control manager (<code>services.exe</code>) is an interface to manage and... |
| [T1569.003](https://attack.mitre.org/techniques/T1569/003) | ↳ Systemctl | Adversaries may abuse systemctl to execute commands or programs. Systemctl is the primary interface for systemd, the Linux init system and service manager. Typically invoked from a shell, Systemctl... |
| [T1609](https://attack.mitre.org/techniques/T1609) | Container Administration Command | Adversaries may abuse a container administration service to execute commands within a container. A container administration service such as the Docker daemon, the Kubernetes API server, or the... |
| [T1610](https://attack.mitre.org/techniques/T1610) | Deploy Container | Adversaries may deploy a container into an environment to facilitate execution or evade defenses. In some cases, adversaries may deploy a new container to execute processes associated with a... |
| [T1648](https://attack.mitre.org/techniques/T1648) | Serverless Execution | Adversaries may abuse serverless computing, integration, and automation services to execute arbitrary code in cloud environments. Many cloud providers offer a variety of serverless resources,... |
| [T1651](https://attack.mitre.org/techniques/T1651) | Cloud Administration Command | Adversaries may abuse cloud management services to execute commands within virtual machines. Resources such as AWS Systems Manager, Azure RunCommand, and Runbooks allow users to remotely run scripts... |
| [T1674](https://attack.mitre.org/techniques/T1674) | Input Injection | Adversaries may simulate keystrokes on a victim’s computer by various means to perform any type of action on behalf of the user, such as launching the command interpreter using keyboard shortcuts,... |
| [T1675](https://attack.mitre.org/techniques/T1675) | ESXi Administration Command | Adversaries may abuse ESXi administration services to execute commands on guest machines hosted within an ESXi virtual environment. Persistent background services on ESXi-hosted VMs, such as the... |
| [T1677](https://attack.mitre.org/techniques/T1677) | Poisoned Pipeline Execution | Adversaries may manipulate continuous integration / continuous development (CI/CD) processes by injecting malicious code into the build process. There are several mechanisms for poisoning pipelines:... |

---

### Persistence

*126 techniques (23 parent, 103 sub-techniques)*

| T-Code | Name | Description |
|--------|------|-------------|
| [T1037](https://attack.mitre.org/techniques/T1037) | Boot or Logon Initialization Scripts | Adversaries may use scripts automatically executed at boot or logon initialization to establish persistence.(Citation: Mandiant APT29 Eye Spy Email Nov 22)(Citation: Anomali Rocke March 2019)... |
| [T1037.001](https://attack.mitre.org/techniques/T1037/001) | ↳ Logon Script (Windows) | Adversaries may use Windows logon scripts automatically executed at logon initialization to establish persistence. Windows allows logon scripts to be run whenever a specific user or group of users... |
| [T1037.002](https://attack.mitre.org/techniques/T1037/002) | ↳ Login Hook | Adversaries may use a Login Hook to establish persistence executed upon user logon. A login hook is a plist file that points to a specific script to execute with root privileges upon user logon. The... |
| [T1037.003](https://attack.mitre.org/techniques/T1037/003) | ↳ Network Logon Script | Adversaries may use network logon scripts automatically executed at logon initialization to establish persistence. Network logon scripts can be assigned using Active Directory or Group Policy... |
| [T1037.004](https://attack.mitre.org/techniques/T1037/004) | ↳ RC Scripts | Adversaries may establish persistence by modifying RC scripts, which are executed during a Unix-like system’s startup. These files allow system administrators to map and start custom services at... |
| [T1037.005](https://attack.mitre.org/techniques/T1037/005) | ↳ Startup Items | Adversaries may use startup items automatically executed at boot initialization to establish persistence. Startup items execute during the final phase of the boot process and contain shell scripts or... |
| [T1053](https://attack.mitre.org/techniques/T1053) | Scheduled Task/Job | Adversaries may abuse task scheduling functionality to facilitate initial or recurring execution of malicious code. Utilities exist within all major operating systems to schedule programs or scripts... |
| [T1053.002](https://attack.mitre.org/techniques/T1053/002) | ↳ At | Adversaries may abuse the [at](https://attack.mitre.org/software/S0110) utility to perform task scheduling for initial or recurring execution of malicious code. The... |
| [T1053.003](https://attack.mitre.org/techniques/T1053/003) | ↳ Cron | Adversaries may abuse the <code>cron</code> utility to perform task scheduling for initial or recurring execution of malicious code.(Citation: 20 macOS Common Tools and Techniques) The... |
| [T1053.005](https://attack.mitre.org/techniques/T1053/005) | ↳ Scheduled Task | Adversaries may abuse the Windows Task Scheduler to perform task scheduling for initial or recurring execution of malicious code. There are multiple ways to access the Task Scheduler in Windows. The... |
| [T1053.006](https://attack.mitre.org/techniques/T1053/006) | ↳ Systemd Timers | Adversaries may abuse systemd timers to perform task scheduling for initial or recurring execution of malicious code. Systemd timers are unit files with file extension <code>.timer</code> that... |
| [T1053.007](https://attack.mitre.org/techniques/T1053/007) | ↳ Container Orchestration Job | Adversaries may abuse task scheduling functionality provided by container orchestration tools such as Kubernetes to schedule deployment of containers configured to execute malicious code. Container... |
| [T1078](https://attack.mitre.org/techniques/T1078) | Valid Accounts | Adversaries may obtain and abuse credentials of existing accounts as a means of gaining Initial Access, Persistence, Privilege Escalation, or Defense Evasion. Compromised credentials may be used to... |
| [T1078.001](https://attack.mitre.org/techniques/T1078/001) | ↳ Default Accounts | Adversaries may obtain and abuse credentials of a default account as a means of gaining Initial Access, Persistence, Privilege Escalation, or Defense Evasion. Default accounts are those that are... |
| [T1078.002](https://attack.mitre.org/techniques/T1078/002) | ↳ Domain Accounts | Adversaries may obtain and abuse credentials of a domain account as a means of gaining Initial Access, Persistence, Privilege Escalation, or Defense Evasion.(Citation: TechNet Credential Theft)... |
| [T1078.003](https://attack.mitre.org/techniques/T1078/003) | ↳ Local Accounts | Adversaries may obtain and abuse credentials of a local account as a means of gaining Initial Access, Persistence, Privilege Escalation, or Defense Evasion. Local accounts are those configured by an... |
| [T1078.004](https://attack.mitre.org/techniques/T1078/004) | ↳ Cloud Accounts | Valid accounts in cloud environments may allow adversaries to perform actions to achieve Initial Access, Persistence, Privilege Escalation, or Defense Evasion. Cloud accounts are those created and... |
| [T1098](https://attack.mitre.org/techniques/T1098) | Account Manipulation | Adversaries may manipulate accounts to maintain and/or elevate access to victim systems. Account manipulation may consist of any action that preserves or modifies adversary access to a compromised... |
| [T1098.001](https://attack.mitre.org/techniques/T1098/001) | ↳ Additional Cloud Credentials | Adversaries may add adversary-controlled credentials to a cloud account to maintain persistent access to victim accounts and instances within the environment. For example, adversaries may add... |
| [T1098.002](https://attack.mitre.org/techniques/T1098/002) | ↳ Additional Email Delegate Permissions | Adversaries may grant additional permission levels to maintain persistent access to an adversary-controlled email account. For example, the <code>Add-MailboxPermission</code>... |
| [T1098.003](https://attack.mitre.org/techniques/T1098/003) | ↳ Additional Cloud Roles | An adversary may add additional roles or permissions to an adversary-controlled cloud account to maintain persistent access to a tenant. For example, adversaries may update IAM policies in... |
| [T1098.004](https://attack.mitre.org/techniques/T1098/004) | ↳ SSH Authorized Keys | Adversaries may modify the SSH <code>authorized_keys</code> file to maintain persistence on a victim host. Linux distributions, macOS, and ESXi hypervisors commonly use key-based authentication to... |
| [T1098.005](https://attack.mitre.org/techniques/T1098/005) | ↳ Device Registration | Adversaries may register a device to an adversary-controlled account. Devices may be registered in a multifactor authentication (MFA) system, which handles authentication to the network, or in a... |
| [T1098.006](https://attack.mitre.org/techniques/T1098/006) | ↳ Additional Container Cluster Roles | An adversary may add additional roles or permissions to an adversary-controlled user or service account to maintain persistent access to a container orchestration system. For example, an adversary... |
| [T1098.007](https://attack.mitre.org/techniques/T1098/007) | ↳ Additional Local or Domain Groups | An adversary may add additional local or domain groups to an adversary-controlled account to maintain persistent access to a system or domain. On Windows, accounts may use the `net localgroup` and... |
| [T1112](https://attack.mitre.org/techniques/T1112) | Modify Registry | Adversaries may interact with the Windows Registry as part of a variety of other techniques to aid in defense evasion, persistence, and execution. Access to specific areas of the Registry depends on... |
| [T1133](https://attack.mitre.org/techniques/T1133) | External Remote Services | Adversaries may leverage external-facing remote services to initially access and/or persist within a network. Remote services such as VPNs, Citrix, and other access mechanisms allow users to connect... |
| [T1136](https://attack.mitre.org/techniques/T1136) | Create Account | Adversaries may create an account to maintain access to victim systems.(Citation: Symantec WastedLocker June 2020) With a sufficient level of access, creating such accounts may be used to establish... |
| [T1136.001](https://attack.mitre.org/techniques/T1136/001) | ↳ Local Account | Adversaries may create a local account to maintain access to victim systems. Local accounts are those configured by an organization for use by users, remote support, services, or for administration... |
| [T1136.002](https://attack.mitre.org/techniques/T1136/002) | ↳ Domain Account | Adversaries may create a domain account to maintain access to victim systems. Domain accounts are those managed by Active Directory Domain Services where access and permissions are configured across... |
| [T1136.003](https://attack.mitre.org/techniques/T1136/003) | ↳ Cloud Account | Adversaries may create a cloud account to maintain access to victim systems. With a sufficient level of access, such accounts may be used to establish secondary credentialed access that does not... |
| [T1137](https://attack.mitre.org/techniques/T1137) | Office Application Startup | Adversaries may leverage Microsoft Office-based applications for persistence between startups. Microsoft Office is a fairly common application suite on Windows-based operating systems within an... |
| [T1137.001](https://attack.mitre.org/techniques/T1137/001) | ↳ Office Template Macros | Adversaries may abuse Microsoft Office templates to obtain persistence on a compromised system. Microsoft Office contains templates that are part of common Office applications and are used to... |
| [T1137.002](https://attack.mitre.org/techniques/T1137/002) | ↳ Office Test | Adversaries may abuse the Microsoft Office "Office Test" Registry key to obtain persistence on a compromised system. An Office Test Registry location exists that allows a user to specify an arbitrary... |
| [T1137.003](https://attack.mitre.org/techniques/T1137/003) | ↳ Outlook Forms | Adversaries may abuse Microsoft Outlook forms to obtain persistence on a compromised system. Outlook forms are used as templates for presentation and functionality in Outlook messages. Custom Outlook... |
| [T1137.004](https://attack.mitre.org/techniques/T1137/004) | ↳ Outlook Home Page | Adversaries may abuse Microsoft Outlook's Home Page feature to obtain persistence on a compromised system. Outlook Home Page is a legacy feature used to customize the presentation of Outlook folders.... |
| [T1137.005](https://attack.mitre.org/techniques/T1137/005) | ↳ Outlook Rules | Adversaries may abuse Microsoft Outlook rules to obtain persistence on a compromised system. Outlook rules allow a user to define automated behavior to manage email messages. A benign rule might, for... |
| [T1137.006](https://attack.mitre.org/techniques/T1137/006) | ↳ Add-ins | Adversaries may abuse Microsoft Office add-ins to obtain persistence on a compromised system. Office add-ins can be used to add functionality to Office programs. (Citation: Microsoft Office Add-ins)... |
| [T1176](https://attack.mitre.org/techniques/T1176) | Software Extensions | Adversaries may abuse software extensions to establish persistent access to victim systems. Software extensions are modular components that enhance or customize the functionality of software... |
| [T1176.001](https://attack.mitre.org/techniques/T1176/001) | ↳ Browser Extensions | Adversaries may abuse internet browser extensions to establish persistent access to victim systems. Browser extensions or plugins are small programs that can add functionality to and customize... |
| [T1176.002](https://attack.mitre.org/techniques/T1176/002) | ↳ IDE Extensions | Adversaries may abuse an integrated development environment (IDE) extension to establish persistent access to victim systems.(Citation: Mnemonic misuse visual studio) IDEs such as Visual Studio Code,... |
| [T1197](https://attack.mitre.org/techniques/T1197) | BITS Jobs | Adversaries may abuse BITS jobs to persistently execute code and perform various background tasks. Windows Background Intelligent Transfer Service (BITS) is a low-bandwidth, asynchronous file... |
| [T1205](https://attack.mitre.org/techniques/T1205) | Traffic Signaling | Adversaries may use traffic signaling to hide open ports or other malicious functionality used for persistence or command and control. Traffic signaling involves the use of a magic value or sequence... |
| [T1205.001](https://attack.mitre.org/techniques/T1205/001) | ↳ Port Knocking | Adversaries may use port knocking to hide open ports used for persistence or command and control. To enable a port, an adversary sends a series of attempted connections to a predefined sequence of... |
| [T1205.002](https://attack.mitre.org/techniques/T1205/002) | ↳ Socket Filters | Adversaries may attach filters to a network socket to monitor then activate backdoors used for persistence or command and control. With elevated permissions, adversaries can use features such as the... |
| [T1505](https://attack.mitre.org/techniques/T1505) | Server Software Component | Adversaries may abuse legitimate extensible development features of servers to establish persistent access to systems. Enterprise server applications may include features that allow developers to... |
| [T1505.001](https://attack.mitre.org/techniques/T1505/001) | ↳ SQL Stored Procedures | Adversaries may abuse SQL stored procedures to establish persistent access to systems. SQL Stored Procedures are code that can be saved and reused so that database users do not waste time rewriting... |
| [T1505.002](https://attack.mitre.org/techniques/T1505/002) | ↳ Transport Agent | Adversaries may abuse Microsoft transport agents to establish persistent access to systems. Microsoft Exchange transport agents can operate on email messages passing through the transport pipeline to... |
| [T1505.003](https://attack.mitre.org/techniques/T1505/003) | ↳ Web Shell | Adversaries may backdoor web servers with web shells to establish persistent access to systems. A Web shell is a Web script that is placed on an openly accessible Web server to allow an adversary to... |
| [T1505.004](https://attack.mitre.org/techniques/T1505/004) | ↳ IIS Components | Adversaries may install malicious components that run on Internet Information Services (IIS) web servers to establish persistence. IIS provides several mechanisms to extend the functionality of the... |
| [T1505.005](https://attack.mitre.org/techniques/T1505/005) | ↳ Terminal Services DLL | Adversaries may abuse components of Terminal Services to enable persistent access to systems. Microsoft Terminal Services, renamed to Remote Desktop Services in some Windows Server OSs as of 2022,... |
| [T1505.006](https://attack.mitre.org/techniques/T1505/006) | ↳ vSphere Installation Bundles | Adversaries may abuse vSphere Installation Bundles (VIBs) to establish persistent access to ESXi hypervisors. VIBs are collections of files used for software distribution and virtual system... |
| [T1525](https://attack.mitre.org/techniques/T1525) | Implant Internal Image | Adversaries may implant cloud or container images with malicious code to establish persistence after gaining access to an environment. Amazon Web Services (AWS) Amazon Machine Images (AMIs), Google... |
| [T1542](https://attack.mitre.org/techniques/T1542) | Pre-OS Boot | Adversaries may abuse Pre-OS Boot mechanisms as a way to establish persistence on a system. During the booting process of a computer, firmware and various startup services are loaded before the... |
| [T1542.001](https://attack.mitre.org/techniques/T1542/001) | ↳ System Firmware | Adversaries may modify system firmware to persist on systems.The BIOS (Basic Input/Output System) and The Unified Extensible Firmware Interface (UEFI) or Extensible Firmware Interface (EFI) are... |
| [T1542.002](https://attack.mitre.org/techniques/T1542/002) | ↳ Component Firmware | Adversaries may modify component firmware to persist on systems. Some adversaries may employ sophisticated means to compromise computer components and install malicious firmware that will execute... |
| [T1542.003](https://attack.mitre.org/techniques/T1542/003) | ↳ Bootkit | Adversaries may use bootkits to persist on systems. A bootkit is a malware variant that modifies the boot sectors of a hard drive, allowing malicious code to execute before a computer's operating... |
| [T1542.004](https://attack.mitre.org/techniques/T1542/004) | ↳ ROMMONkit | Adversaries may abuse the ROM Monitor (ROMMON) by loading an unauthorized firmware with adversary code to provide persistent access and manipulate device behavior that is difficult to detect.... |
| [T1542.005](https://attack.mitre.org/techniques/T1542/005) | ↳ TFTP Boot | Adversaries may abuse netbooting to load an unauthorized network device operating system from a Trivial File Transfer Protocol (TFTP) server. TFTP boot (netbooting) is commonly used by network... |
| [T1543](https://attack.mitre.org/techniques/T1543) | Create or Modify System Process | Adversaries may create or modify system-level processes to repeatedly execute malicious payloads as part of persistence. When operating systems boot up, they can start processes that perform... |
| [T1543.001](https://attack.mitre.org/techniques/T1543/001) | ↳ Launch Agent | Adversaries may create or modify launch agents to repeatedly execute malicious payloads as part of persistence. When a user logs in, a per-user launchd process is started which loads the parameters... |
| [T1543.002](https://attack.mitre.org/techniques/T1543/002) | ↳ Systemd Service | Adversaries may create or modify systemd services to repeatedly execute malicious payloads as part of persistence. Systemd is a system and service manager commonly used for managing background daemon... |
| [T1543.003](https://attack.mitre.org/techniques/T1543/003) | ↳ Windows Service | Adversaries may create or modify Windows services to repeatedly execute malicious payloads as part of persistence. When Windows boots up, it starts programs or applications called services that... |
| [T1543.004](https://attack.mitre.org/techniques/T1543/004) | ↳ Launch Daemon | Adversaries may create or modify Launch Daemons to execute malicious payloads as part of persistence. Launch Daemons are plist files used to interact with Launchd, the service management framework... |
| [T1543.005](https://attack.mitre.org/techniques/T1543/005) | ↳ Container Service | Adversaries may create or modify container or container cluster management tools that run as daemons, agents, or services on individual hosts. These include software for creating and managing... |
| [T1546](https://attack.mitre.org/techniques/T1546) | Event Triggered Execution | Adversaries may establish persistence and/or elevate privileges using system mechanisms that trigger execution based on specific events. Various operating systems have means to monitor and subscribe... |
| [T1546.001](https://attack.mitre.org/techniques/T1546/001) | ↳ Change Default File Association | Adversaries may establish persistence by executing malicious content triggered by a file type association. When a file is opened, the default program used to open the file (also called the file... |
| [T1546.002](https://attack.mitre.org/techniques/T1546/002) | ↳ Screensaver | Adversaries may establish persistence by executing malicious content triggered by user inactivity. Screensavers are programs that execute after a configurable time of user inactivity and consist of... |
| [T1546.003](https://attack.mitre.org/techniques/T1546/003) | ↳ Windows Management Instrumentation Event Subscription | Adversaries may establish persistence and elevate privileges by executing malicious content triggered by a Windows Management Instrumentation (WMI) event subscription. WMI can be used to install... |
| [T1546.004](https://attack.mitre.org/techniques/T1546/004) | ↳ Unix Shell Configuration Modification | Adversaries may establish persistence through executing malicious commands triggered by a user’s shell. User [Unix Shell](https://attack.mitre.org/techniques/T1059/004)s execute several configuration... |
| [T1546.005](https://attack.mitre.org/techniques/T1546/005) | ↳ Trap | Adversaries may establish persistence by executing malicious content triggered by an interrupt signal. The <code>trap</code> command allows programs and shells to specify commands that will be... |
| [T1546.006](https://attack.mitre.org/techniques/T1546/006) | ↳ LC_LOAD_DYLIB Addition | Adversaries may establish persistence by executing malicious content triggered by the execution of tainted binaries. Mach-O binaries have a series of headers that are used to perform certain... |
| [T1546.007](https://attack.mitre.org/techniques/T1546/007) | ↳ Netsh Helper DLL | Adversaries may establish persistence by executing malicious content triggered by Netsh Helper DLLs. Netsh.exe (also referred to as Netshell) is a command-line scripting utility used to interact with... |
| [T1546.008](https://attack.mitre.org/techniques/T1546/008) | ↳ Accessibility Features | Adversaries may establish persistence and/or elevate privileges by executing malicious content triggered by accessibility features. Windows contains accessibility features that may be launched with a... |
| [T1546.009](https://attack.mitre.org/techniques/T1546/009) | ↳ AppCert DLLs | Adversaries may establish persistence and/or elevate privileges by executing malicious content triggered by AppCert DLLs loaded into processes. Dynamic-link libraries (DLLs) that are specified in the... |
| [T1546.010](https://attack.mitre.org/techniques/T1546/010) | ↳ AppInit DLLs | Adversaries may establish persistence and/or elevate privileges by executing malicious content triggered by AppInit DLLs loaded into processes. Dynamic-link libraries (DLLs) that are specified in the... |
| [T1546.011](https://attack.mitre.org/techniques/T1546/011) | ↳ Application Shimming | Adversaries may establish persistence and/or elevate privileges by executing malicious content triggered by application shims. The Microsoft Windows Application Compatibility Infrastructure/Framework... |
| [T1546.012](https://attack.mitre.org/techniques/T1546/012) | ↳ Image File Execution Options Injection | Adversaries may establish persistence and/or elevate privileges by executing malicious content triggered by Image File Execution Options (IFEO) debuggers. IFEOs enable a developer to attach a... |
| [T1546.013](https://attack.mitre.org/techniques/T1546/013) | ↳ PowerShell Profile | Adversaries may gain persistence and elevate privileges by executing malicious content triggered by PowerShell profiles. A PowerShell profile (<code>profile.ps1</code>) is a script that runs when... |
| [T1546.014](https://attack.mitre.org/techniques/T1546/014) | ↳ Emond | Adversaries may gain persistence and elevate privileges by executing malicious content triggered by the Event Monitor Daemon (emond). Emond is a [Launch... |
| [T1546.015](https://attack.mitre.org/techniques/T1546/015) | ↳ Component Object Model Hijacking | Adversaries may establish persistence by executing malicious content triggered by hijacked references to Component Object Model (COM) objects. COM is a system within Windows to enable interaction... |
| [T1546.016](https://attack.mitre.org/techniques/T1546/016) | ↳ Installer Packages | Adversaries may establish persistence and elevate privileges by using an installer to trigger the execution of malicious content. Installer packages are OS specific and contain the resources an... |
| [T1546.017](https://attack.mitre.org/techniques/T1546/017) | ↳ Udev Rules | Adversaries may maintain persistence through executing malicious content triggered using udev rules. Udev is the Linux kernel device manager that dynamically manages device nodes, handles access to... |
| [T1546.018](https://attack.mitre.org/techniques/T1546/018) | ↳ Python Startup Hooks | Adversaries may achieve persistence by leveraging Python’s startup mechanisms, including path configuration (`.pth`) files and the `sitecustomize.py` or `usercustomize.py` modules. These files are... |
| [T1547](https://attack.mitre.org/techniques/T1547) | Boot or Logon Autostart Execution | Adversaries may configure system settings to automatically execute a program during system boot or logon to maintain persistence or gain higher-level privileges on compromised systems. Operating... |
| [T1547.001](https://attack.mitre.org/techniques/T1547/001) | ↳ Registry Run Keys / Startup Folder | Adversaries may achieve persistence by adding a program to a startup folder or referencing it with a Registry run key. Adding an entry to the "run keys" in the Registry or startup folder will cause... |
| [T1547.002](https://attack.mitre.org/techniques/T1547/002) | ↳ Authentication Package | Adversaries may abuse authentication packages to execute DLLs when the system boots. Windows authentication package DLLs are loaded by the Local Security Authority (LSA) process at system start. They... |
| [T1547.003](https://attack.mitre.org/techniques/T1547/003) | ↳ Time Providers | Adversaries may abuse time providers to execute DLLs when the system boots. The Windows Time service (W32Time) enables time synchronization across and within domains.(Citation: Microsoft W32Time Feb... |
| [T1547.004](https://attack.mitre.org/techniques/T1547/004) | ↳ Winlogon Helper DLL | Adversaries may abuse features of Winlogon to execute DLLs and/or executables when a user logs in. Winlogon.exe is a Windows component responsible for actions at logon/logoff as well as the secure... |
| [T1547.005](https://attack.mitre.org/techniques/T1547/005) | ↳ Security Support Provider | Adversaries may abuse security support providers (SSPs) to execute DLLs when the system boots. Windows SSP DLLs are loaded into the Local Security Authority (LSA) process at system start. Once loaded... |
| [T1547.006](https://attack.mitre.org/techniques/T1547/006) | ↳ Kernel Modules and Extensions | Adversaries may modify the kernel to automatically execute programs on system boot. Loadable Kernel Modules (LKMs) are pieces of code that can be loaded and unloaded into the kernel upon demand. They... |
| [T1547.007](https://attack.mitre.org/techniques/T1547/007) | ↳ Re-opened Applications | Adversaries may modify plist files to automatically run an application when a user logs in. When a user logs out or restarts via the macOS Graphical User Interface (GUI), a prompt is provided to the... |
| [T1547.008](https://attack.mitre.org/techniques/T1547/008) | ↳ LSASS Driver | Adversaries may modify or add LSASS drivers to obtain persistence on compromised systems. The Windows security subsystem is a set of components that manage and enforce the security policy for a... |
| [T1547.009](https://attack.mitre.org/techniques/T1547/009) | ↳ Shortcut Modification | Adversaries may create or modify shortcuts that can execute a program during system boot or user login. Shortcuts or symbolic links are used to reference other files or programs that will be opened... |
| [T1547.010](https://attack.mitre.org/techniques/T1547/010) | ↳ Port Monitors | Adversaries may use port monitors to run an adversary supplied DLL during system boot for persistence or privilege escalation. A port monitor can be set through the <code>AddMonitor</code> API call... |
| [T1547.012](https://attack.mitre.org/techniques/T1547/012) | ↳ Print Processors | Adversaries may abuse print processors to run malicious DLLs during system boot for persistence and/or privilege escalation. Print processors are DLLs that are loaded by the print spooler service,... |
| [T1547.013](https://attack.mitre.org/techniques/T1547/013) | ↳ XDG Autostart Entries | Adversaries may add or modify XDG Autostart Entries to execute malicious programs or commands when a user’s desktop environment is loaded at login. XDG Autostart entries are available for any... |
| [T1547.014](https://attack.mitre.org/techniques/T1547/014) | ↳ Active Setup | Adversaries may achieve persistence by adding a Registry key to the Active Setup of the local machine. Active Setup is a Windows mechanism that is used to execute programs when a user logs in. The... |
| [T1547.015](https://attack.mitre.org/techniques/T1547/015) | ↳ Login Items | Adversaries may add login items to execute upon user login to gain persistence or escalate privileges. Login items are applications, documents, folders, or server connections that are automatically... |
| [T1554](https://attack.mitre.org/techniques/T1554) | Compromise Host Software Binary | Adversaries may modify host software binaries to establish persistent access to systems. Software binaries/executables provide a wide range of system commands or services, programs, and libraries.... |
| [T1556](https://attack.mitre.org/techniques/T1556) | Modify Authentication Process | Adversaries may modify authentication mechanisms and processes to access user credentials or enable otherwise unwarranted access to accounts. The authentication process is handled by mechanisms, such... |
| [T1556.001](https://attack.mitre.org/techniques/T1556/001) | ↳ Domain Controller Authentication | Adversaries may patch the authentication process on a domain controller to bypass the typical authentication mechanisms and enable access to accounts. Malware may be used to inject false credentials... |
| [T1556.002](https://attack.mitre.org/techniques/T1556/002) | ↳ Password Filter DLL | Adversaries may register malicious password filter dynamic link libraries (DLLs) into the authentication process to acquire user credentials as they are validated. Windows password filters are... |
| [T1556.003](https://attack.mitre.org/techniques/T1556/003) | ↳ Pluggable Authentication Modules | Adversaries may modify pluggable authentication modules (PAM) to access user credentials or enable otherwise unwarranted access to accounts. PAM is a modular system of configuration files, libraries,... |
| [T1556.004](https://attack.mitre.org/techniques/T1556/004) | ↳ Network Device Authentication | Adversaries may use [Patch System Image](https://attack.mitre.org/techniques/T1601/001) to hard code a password in the operating system, thus bypassing of native authentication mechanisms for local... |
| [T1556.005](https://attack.mitre.org/techniques/T1556/005) | ↳ Reversible Encryption | An adversary may abuse Active Directory authentication encryption properties to gain access to credentials on Windows systems. The <code>AllowReversiblePasswordEncryption</code> property specifies... |
| [T1556.006](https://attack.mitre.org/techniques/T1556/006) | ↳ Multi-Factor Authentication | Adversaries may disable or modify multi-factor authentication (MFA) mechanisms to enable persistent access to compromised accounts. Once adversaries have gained access to a network by either... |
| [T1556.007](https://attack.mitre.org/techniques/T1556/007) | ↳ Hybrid Identity | Adversaries may patch, modify, or otherwise backdoor cloud authentication processes that are tied to on-premises user identities in order to bypass typical authentication mechanisms, access... |
| [T1556.008](https://attack.mitre.org/techniques/T1556/008) | ↳ Network Provider DLL | Adversaries may register malicious network provider dynamic link libraries (DLLs) to capture cleartext user credentials during the authentication process. Network provider DLLs allow Windows to... |
| [T1556.009](https://attack.mitre.org/techniques/T1556/009) | ↳ Conditional Access Policies | Adversaries may disable or modify conditional access policies to enable persistent access to compromised accounts. Conditional access policies are additional verifications used by identity providers... |
| [T1574](https://attack.mitre.org/techniques/T1574) | Hijack Execution Flow | Adversaries may execute their own malicious payloads by hijacking the way operating systems run programs. Hijacking execution flow can be for the purposes of persistence, since this hijacked... |
| [T1574.001](https://attack.mitre.org/techniques/T1574/001) | ↳ DLL | Adversaries may abuse dynamic-link library files (DLLs) in order to achieve persistence, escalate privileges, and evade defenses. DLLs are libraries that contain code and data that can be... |
| [T1574.004](https://attack.mitre.org/techniques/T1574/004) | ↳ Dylib Hijacking | Adversaries may execute their own payloads by placing a malicious dynamic library (dylib) with an expected name in a path a victim application searches at runtime. The dynamic loader will try to find... |
| [T1574.005](https://attack.mitre.org/techniques/T1574/005) | ↳ Executable Installer File Permissions Weakness | Adversaries may execute their own malicious payloads by hijacking the binaries used by an installer. These processes may automatically execute specific binaries as part of their functionality or to... |
| [T1574.006](https://attack.mitre.org/techniques/T1574/006) | ↳ Dynamic Linker Hijacking | Adversaries may execute their own malicious payloads by hijacking environment variables the dynamic linker uses to load shared libraries. During the execution preparation phase of a program, the... |
| [T1574.007](https://attack.mitre.org/techniques/T1574/007) | ↳ Path Interception by PATH Environment Variable | Adversaries may execute their own malicious payloads by hijacking environment variables used to load libraries. The PATH environment variable contains a list of directories (User and System) that the... |
| [T1574.008](https://attack.mitre.org/techniques/T1574/008) | ↳ Path Interception by Search Order Hijacking | Adversaries may execute their own malicious payloads by hijacking the search order used to load other programs. Because some programs do not call other programs using the full path, adversaries may... |
| [T1574.009](https://attack.mitre.org/techniques/T1574/009) | ↳ Path Interception by Unquoted Path | Adversaries may execute their own malicious payloads by hijacking vulnerable file path references. Adversaries can take advantage of paths that lack surrounding quotations by placing an executable in... |
| [T1574.010](https://attack.mitre.org/techniques/T1574/010) | ↳ Services File Permissions Weakness | Adversaries may execute their own malicious payloads by hijacking the binaries used by services. Adversaries may use flaws in the permissions of Windows services to replace the binary that is... |
| [T1574.011](https://attack.mitre.org/techniques/T1574/011) | ↳ Services Registry Permissions Weakness | Adversaries may execute their own malicious payloads by hijacking the Registry entries used by services. Flaws in the permissions for Registry keys related to services can allow adversaries to... |
| [T1574.012](https://attack.mitre.org/techniques/T1574/012) | ↳ COR_PROFILER | Adversaries may leverage the COR_PROFILER environment variable to hijack the execution flow of programs that load the .NET CLR. The COR_PROFILER is a .NET Framework feature which allows developers to... |
| [T1574.013](https://attack.mitre.org/techniques/T1574/013) | ↳ KernelCallbackTable | Adversaries may abuse the <code>KernelCallbackTable</code> of a process to hijack its execution flow in order to run their own payloads.(Citation: Lazarus APT January 2022)(Citation: FinFisher... |
| [T1574.014](https://attack.mitre.org/techniques/T1574/014) | ↳ AppDomainManager | Adversaries may execute their own malicious payloads by hijacking how the .NET `AppDomainManager` loads assemblies. The .NET framework uses the `AppDomainManager` class to create and manage one or... |
| [T1653](https://attack.mitre.org/techniques/T1653) | Power Settings | Adversaries may impair a system's ability to hibernate, reboot, or shut down in order to extend access to infected machines. When a computer enters a dormant state, some or all software and hardware... |
| [T1668](https://attack.mitre.org/techniques/T1668) | Exclusive Control | Adversaries who successfully compromise a system may attempt to maintain persistence by “closing the door” behind them – in other words, by preventing other threat actors from initially accessing or... |
| [T1671](https://attack.mitre.org/techniques/T1671) | Cloud Application Integration | Adversaries may achieve persistence by leveraging OAuth application integrations in a software-as-a-service environment. Adversaries may create a custom application, add a legitimate application into... |

---

### Privilege Escalation

*109 techniques (14 parent, 95 sub-techniques)*

| T-Code | Name | Description |
|--------|------|-------------|
| [T1037](https://attack.mitre.org/techniques/T1037) | Boot or Logon Initialization Scripts | Adversaries may use scripts automatically executed at boot or logon initialization to establish persistence.(Citation: Mandiant APT29 Eye Spy Email Nov 22)(Citation: Anomali Rocke March 2019)... |
| [T1037.001](https://attack.mitre.org/techniques/T1037/001) | ↳ Logon Script (Windows) | Adversaries may use Windows logon scripts automatically executed at logon initialization to establish persistence. Windows allows logon scripts to be run whenever a specific user or group of users... |
| [T1037.002](https://attack.mitre.org/techniques/T1037/002) | ↳ Login Hook | Adversaries may use a Login Hook to establish persistence executed upon user logon. A login hook is a plist file that points to a specific script to execute with root privileges upon user logon. The... |
| [T1037.003](https://attack.mitre.org/techniques/T1037/003) | ↳ Network Logon Script | Adversaries may use network logon scripts automatically executed at logon initialization to establish persistence. Network logon scripts can be assigned using Active Directory or Group Policy... |
| [T1037.004](https://attack.mitre.org/techniques/T1037/004) | ↳ RC Scripts | Adversaries may establish persistence by modifying RC scripts, which are executed during a Unix-like system’s startup. These files allow system administrators to map and start custom services at... |
| [T1037.005](https://attack.mitre.org/techniques/T1037/005) | ↳ Startup Items | Adversaries may use startup items automatically executed at boot initialization to establish persistence. Startup items execute during the final phase of the boot process and contain shell scripts or... |
| [T1053](https://attack.mitre.org/techniques/T1053) | Scheduled Task/Job | Adversaries may abuse task scheduling functionality to facilitate initial or recurring execution of malicious code. Utilities exist within all major operating systems to schedule programs or scripts... |
| [T1053.002](https://attack.mitre.org/techniques/T1053/002) | ↳ At | Adversaries may abuse the [at](https://attack.mitre.org/software/S0110) utility to perform task scheduling for initial or recurring execution of malicious code. The... |
| [T1053.003](https://attack.mitre.org/techniques/T1053/003) | ↳ Cron | Adversaries may abuse the <code>cron</code> utility to perform task scheduling for initial or recurring execution of malicious code.(Citation: 20 macOS Common Tools and Techniques) The... |
| [T1053.005](https://attack.mitre.org/techniques/T1053/005) | ↳ Scheduled Task | Adversaries may abuse the Windows Task Scheduler to perform task scheduling for initial or recurring execution of malicious code. There are multiple ways to access the Task Scheduler in Windows. The... |
| [T1053.006](https://attack.mitre.org/techniques/T1053/006) | ↳ Systemd Timers | Adversaries may abuse systemd timers to perform task scheduling for initial or recurring execution of malicious code. Systemd timers are unit files with file extension <code>.timer</code> that... |
| [T1053.007](https://attack.mitre.org/techniques/T1053/007) | ↳ Container Orchestration Job | Adversaries may abuse task scheduling functionality provided by container orchestration tools such as Kubernetes to schedule deployment of containers configured to execute malicious code. Container... |
| [T1055](https://attack.mitre.org/techniques/T1055) | Process Injection | Adversaries may inject code into processes in order to evade process-based defenses as well as possibly elevate privileges. Process injection is a method of executing arbitrary code in the address... |
| [T1055.001](https://attack.mitre.org/techniques/T1055/001) | ↳ Dynamic-link Library Injection | Adversaries may inject dynamic-link libraries (DLLs) into processes in order to evade process-based defenses as well as possibly elevate privileges. DLL injection is a method of executing arbitrary... |
| [T1055.002](https://attack.mitre.org/techniques/T1055/002) | ↳ Portable Executable Injection | Adversaries may inject portable executables (PE) into processes in order to evade process-based defenses as well as possibly elevate privileges. PE injection is a method of executing arbitrary code... |
| [T1055.003](https://attack.mitre.org/techniques/T1055/003) | ↳ Thread Execution Hijacking | Adversaries may inject malicious code into hijacked processes in order to evade process-based defenses as well as possibly elevate privileges. Thread Execution Hijacking is a method of executing... |
| [T1055.004](https://attack.mitre.org/techniques/T1055/004) | ↳ Asynchronous Procedure Call | Adversaries may inject malicious code into processes via the asynchronous procedure call (APC) queue in order to evade process-based defenses as well as possibly elevate privileges. APC injection is... |
| [T1055.005](https://attack.mitre.org/techniques/T1055/005) | ↳ Thread Local Storage | Adversaries may inject malicious code into processes via thread local storage (TLS) callbacks in order to evade process-based defenses as well as possibly elevate privileges. TLS callback injection... |
| [T1055.008](https://attack.mitre.org/techniques/T1055/008) | ↳ Ptrace System Calls | Adversaries may inject malicious code into processes via ptrace (process trace) system calls in order to evade process-based defenses as well as possibly elevate privileges. Ptrace system call... |
| [T1055.009](https://attack.mitre.org/techniques/T1055/009) | ↳ Proc Memory | Adversaries may inject malicious code into processes via the /proc filesystem in order to evade process-based defenses as well as possibly elevate privileges. Proc memory injection is a method of... |
| [T1055.011](https://attack.mitre.org/techniques/T1055/011) | ↳ Extra Window Memory Injection | Adversaries may inject malicious code into process via Extra Window Memory (EWM) in order to evade process-based defenses as well as possibly elevate privileges. EWM injection is a method of... |
| [T1055.012](https://attack.mitre.org/techniques/T1055/012) | ↳ Process Hollowing | Adversaries may inject malicious code into suspended and hollowed processes in order to evade process-based defenses. Process hollowing is a method of executing arbitrary code in the address space of... |
| [T1055.013](https://attack.mitre.org/techniques/T1055/013) | ↳ Process Doppelgänging | Adversaries may inject malicious code into process via process doppelgänging in order to evade process-based defenses as well as possibly elevate privileges. Process doppelgänging is a method of... |
| [T1055.014](https://attack.mitre.org/techniques/T1055/014) | ↳ VDSO Hijacking | Adversaries may inject malicious code into processes via VDSO hijacking in order to evade process-based defenses as well as possibly elevate privileges. Virtual dynamic shared object (vdso) hijacking... |
| [T1055.015](https://attack.mitre.org/techniques/T1055/015) | ↳ ListPlanting | Adversaries may abuse list-view controls to inject malicious code into hijacked processes in order to evade process-based defenses as well as possibly elevate privileges. ListPlanting is a method of... |
| [T1068](https://attack.mitre.org/techniques/T1068) | Exploitation for Privilege Escalation | Adversaries may exploit software vulnerabilities in an attempt to elevate privileges. Exploitation of a software vulnerability occurs when an adversary takes advantage of a programming error in a... |
| [T1078](https://attack.mitre.org/techniques/T1078) | Valid Accounts | Adversaries may obtain and abuse credentials of existing accounts as a means of gaining Initial Access, Persistence, Privilege Escalation, or Defense Evasion. Compromised credentials may be used to... |
| [T1078.001](https://attack.mitre.org/techniques/T1078/001) | ↳ Default Accounts | Adversaries may obtain and abuse credentials of a default account as a means of gaining Initial Access, Persistence, Privilege Escalation, or Defense Evasion. Default accounts are those that are... |
| [T1078.002](https://attack.mitre.org/techniques/T1078/002) | ↳ Domain Accounts | Adversaries may obtain and abuse credentials of a domain account as a means of gaining Initial Access, Persistence, Privilege Escalation, or Defense Evasion.(Citation: TechNet Credential Theft)... |
| [T1078.003](https://attack.mitre.org/techniques/T1078/003) | ↳ Local Accounts | Adversaries may obtain and abuse credentials of a local account as a means of gaining Initial Access, Persistence, Privilege Escalation, or Defense Evasion. Local accounts are those configured by an... |
| [T1078.004](https://attack.mitre.org/techniques/T1078/004) | ↳ Cloud Accounts | Valid accounts in cloud environments may allow adversaries to perform actions to achieve Initial Access, Persistence, Privilege Escalation, or Defense Evasion. Cloud accounts are those created and... |
| [T1098](https://attack.mitre.org/techniques/T1098) | Account Manipulation | Adversaries may manipulate accounts to maintain and/or elevate access to victim systems. Account manipulation may consist of any action that preserves or modifies adversary access to a compromised... |
| [T1098.001](https://attack.mitre.org/techniques/T1098/001) | ↳ Additional Cloud Credentials | Adversaries may add adversary-controlled credentials to a cloud account to maintain persistent access to victim accounts and instances within the environment. For example, adversaries may add... |
| [T1098.002](https://attack.mitre.org/techniques/T1098/002) | ↳ Additional Email Delegate Permissions | Adversaries may grant additional permission levels to maintain persistent access to an adversary-controlled email account. For example, the <code>Add-MailboxPermission</code>... |
| [T1098.003](https://attack.mitre.org/techniques/T1098/003) | ↳ Additional Cloud Roles | An adversary may add additional roles or permissions to an adversary-controlled cloud account to maintain persistent access to a tenant. For example, adversaries may update IAM policies in... |
| [T1098.004](https://attack.mitre.org/techniques/T1098/004) | ↳ SSH Authorized Keys | Adversaries may modify the SSH <code>authorized_keys</code> file to maintain persistence on a victim host. Linux distributions, macOS, and ESXi hypervisors commonly use key-based authentication to... |
| [T1098.005](https://attack.mitre.org/techniques/T1098/005) | ↳ Device Registration | Adversaries may register a device to an adversary-controlled account. Devices may be registered in a multifactor authentication (MFA) system, which handles authentication to the network, or in a... |
| [T1098.006](https://attack.mitre.org/techniques/T1098/006) | ↳ Additional Container Cluster Roles | An adversary may add additional roles or permissions to an adversary-controlled user or service account to maintain persistent access to a container orchestration system. For example, an adversary... |
| [T1098.007](https://attack.mitre.org/techniques/T1098/007) | ↳ Additional Local or Domain Groups | An adversary may add additional local or domain groups to an adversary-controlled account to maintain persistent access to a system or domain. On Windows, accounts may use the `net localgroup` and... |
| [T1134](https://attack.mitre.org/techniques/T1134) | Access Token Manipulation | Adversaries may modify access tokens to operate under a different user or system security context to perform actions and bypass access controls. Windows uses access tokens to determine the ownership... |
| [T1134.001](https://attack.mitre.org/techniques/T1134/001) | ↳ Token Impersonation/Theft | Adversaries may duplicate then impersonate another user's existing token to escalate privileges and bypass access controls. For example, an adversary can duplicate an existing token using... |
| [T1134.002](https://attack.mitre.org/techniques/T1134/002) | ↳ Create Process with Token | Adversaries may create a new process with an existing token to escalate privileges and bypass access controls. Processes can be created with the token and resulting security context of another user... |
| [T1134.003](https://attack.mitre.org/techniques/T1134/003) | ↳ Make and Impersonate Token | Adversaries may make new tokens and impersonate users to escalate privileges and bypass access controls. For example, if an adversary has a username and password but the user is not logged onto the... |
| [T1134.004](https://attack.mitre.org/techniques/T1134/004) | ↳ Parent PID Spoofing | Adversaries may spoof the parent process identifier (PPID) of a new process to evade process-monitoring defenses or to elevate privileges. New processes are typically spawned directly from their... |
| [T1134.005](https://attack.mitre.org/techniques/T1134/005) | ↳ SID-History Injection | Adversaries may use SID-History Injection to escalate privileges and bypass access controls. The Windows security identifier (SID) is a unique value that identifies a user or group account. SIDs are... |
| [T1484](https://attack.mitre.org/techniques/T1484) | Domain or Tenant Policy Modification | Adversaries may modify the configuration settings of a domain or identity tenant to evade defenses and/or escalate privileges in centrally managed environments. Such services provide a centralized... |
| [T1484.001](https://attack.mitre.org/techniques/T1484/001) | ↳ Group Policy Modification | Adversaries may modify Group Policy Objects (GPOs) to subvert the intended discretionary access controls for a domain, usually with the intention of escalating privileges on the domain. Group policy... |
| [T1484.002](https://attack.mitre.org/techniques/T1484/002) | ↳ Trust Modification | Adversaries may add new domain trusts, modify the properties of existing domain trusts, or otherwise change the configuration of trust relationships between domains and tenants to evade defenses... |
| [T1543](https://attack.mitre.org/techniques/T1543) | Create or Modify System Process | Adversaries may create or modify system-level processes to repeatedly execute malicious payloads as part of persistence. When operating systems boot up, they can start processes that perform... |
| [T1543.001](https://attack.mitre.org/techniques/T1543/001) | ↳ Launch Agent | Adversaries may create or modify launch agents to repeatedly execute malicious payloads as part of persistence. When a user logs in, a per-user launchd process is started which loads the parameters... |
| [T1543.002](https://attack.mitre.org/techniques/T1543/002) | ↳ Systemd Service | Adversaries may create or modify systemd services to repeatedly execute malicious payloads as part of persistence. Systemd is a system and service manager commonly used for managing background daemon... |
| [T1543.003](https://attack.mitre.org/techniques/T1543/003) | ↳ Windows Service | Adversaries may create or modify Windows services to repeatedly execute malicious payloads as part of persistence. When Windows boots up, it starts programs or applications called services that... |
| [T1543.004](https://attack.mitre.org/techniques/T1543/004) | ↳ Launch Daemon | Adversaries may create or modify Launch Daemons to execute malicious payloads as part of persistence. Launch Daemons are plist files used to interact with Launchd, the service management framework... |
| [T1543.005](https://attack.mitre.org/techniques/T1543/005) | ↳ Container Service | Adversaries may create or modify container or container cluster management tools that run as daemons, agents, or services on individual hosts. These include software for creating and managing... |
| [T1546](https://attack.mitre.org/techniques/T1546) | Event Triggered Execution | Adversaries may establish persistence and/or elevate privileges using system mechanisms that trigger execution based on specific events. Various operating systems have means to monitor and subscribe... |
| [T1546.001](https://attack.mitre.org/techniques/T1546/001) | ↳ Change Default File Association | Adversaries may establish persistence by executing malicious content triggered by a file type association. When a file is opened, the default program used to open the file (also called the file... |
| [T1546.002](https://attack.mitre.org/techniques/T1546/002) | ↳ Screensaver | Adversaries may establish persistence by executing malicious content triggered by user inactivity. Screensavers are programs that execute after a configurable time of user inactivity and consist of... |
| [T1546.003](https://attack.mitre.org/techniques/T1546/003) | ↳ Windows Management Instrumentation Event Subscription | Adversaries may establish persistence and elevate privileges by executing malicious content triggered by a Windows Management Instrumentation (WMI) event subscription. WMI can be used to install... |
| [T1546.004](https://attack.mitre.org/techniques/T1546/004) | ↳ Unix Shell Configuration Modification | Adversaries may establish persistence through executing malicious commands triggered by a user’s shell. User [Unix Shell](https://attack.mitre.org/techniques/T1059/004)s execute several configuration... |
| [T1546.005](https://attack.mitre.org/techniques/T1546/005) | ↳ Trap | Adversaries may establish persistence by executing malicious content triggered by an interrupt signal. The <code>trap</code> command allows programs and shells to specify commands that will be... |
| [T1546.006](https://attack.mitre.org/techniques/T1546/006) | ↳ LC_LOAD_DYLIB Addition | Adversaries may establish persistence by executing malicious content triggered by the execution of tainted binaries. Mach-O binaries have a series of headers that are used to perform certain... |
| [T1546.007](https://attack.mitre.org/techniques/T1546/007) | ↳ Netsh Helper DLL | Adversaries may establish persistence by executing malicious content triggered by Netsh Helper DLLs. Netsh.exe (also referred to as Netshell) is a command-line scripting utility used to interact with... |
| [T1546.008](https://attack.mitre.org/techniques/T1546/008) | ↳ Accessibility Features | Adversaries may establish persistence and/or elevate privileges by executing malicious content triggered by accessibility features. Windows contains accessibility features that may be launched with a... |
| [T1546.009](https://attack.mitre.org/techniques/T1546/009) | ↳ AppCert DLLs | Adversaries may establish persistence and/or elevate privileges by executing malicious content triggered by AppCert DLLs loaded into processes. Dynamic-link libraries (DLLs) that are specified in the... |
| [T1546.010](https://attack.mitre.org/techniques/T1546/010) | ↳ AppInit DLLs | Adversaries may establish persistence and/or elevate privileges by executing malicious content triggered by AppInit DLLs loaded into processes. Dynamic-link libraries (DLLs) that are specified in the... |
| [T1546.011](https://attack.mitre.org/techniques/T1546/011) | ↳ Application Shimming | Adversaries may establish persistence and/or elevate privileges by executing malicious content triggered by application shims. The Microsoft Windows Application Compatibility Infrastructure/Framework... |
| [T1546.012](https://attack.mitre.org/techniques/T1546/012) | ↳ Image File Execution Options Injection | Adversaries may establish persistence and/or elevate privileges by executing malicious content triggered by Image File Execution Options (IFEO) debuggers. IFEOs enable a developer to attach a... |
| [T1546.013](https://attack.mitre.org/techniques/T1546/013) | ↳ PowerShell Profile | Adversaries may gain persistence and elevate privileges by executing malicious content triggered by PowerShell profiles. A PowerShell profile (<code>profile.ps1</code>) is a script that runs when... |
| [T1546.014](https://attack.mitre.org/techniques/T1546/014) | ↳ Emond | Adversaries may gain persistence and elevate privileges by executing malicious content triggered by the Event Monitor Daemon (emond). Emond is a [Launch... |
| [T1546.015](https://attack.mitre.org/techniques/T1546/015) | ↳ Component Object Model Hijacking | Adversaries may establish persistence by executing malicious content triggered by hijacked references to Component Object Model (COM) objects. COM is a system within Windows to enable interaction... |
| [T1546.016](https://attack.mitre.org/techniques/T1546/016) | ↳ Installer Packages | Adversaries may establish persistence and elevate privileges by using an installer to trigger the execution of malicious content. Installer packages are OS specific and contain the resources an... |
| [T1546.017](https://attack.mitre.org/techniques/T1546/017) | ↳ Udev Rules | Adversaries may maintain persistence through executing malicious content triggered using udev rules. Udev is the Linux kernel device manager that dynamically manages device nodes, handles access to... |
| [T1546.018](https://attack.mitre.org/techniques/T1546/018) | ↳ Python Startup Hooks | Adversaries may achieve persistence by leveraging Python’s startup mechanisms, including path configuration (`.pth`) files and the `sitecustomize.py` or `usercustomize.py` modules. These files are... |
| [T1547](https://attack.mitre.org/techniques/T1547) | Boot or Logon Autostart Execution | Adversaries may configure system settings to automatically execute a program during system boot or logon to maintain persistence or gain higher-level privileges on compromised systems. Operating... |
| [T1547.001](https://attack.mitre.org/techniques/T1547/001) | ↳ Registry Run Keys / Startup Folder | Adversaries may achieve persistence by adding a program to a startup folder or referencing it with a Registry run key. Adding an entry to the "run keys" in the Registry or startup folder will cause... |
| [T1547.002](https://attack.mitre.org/techniques/T1547/002) | ↳ Authentication Package | Adversaries may abuse authentication packages to execute DLLs when the system boots. Windows authentication package DLLs are loaded by the Local Security Authority (LSA) process at system start. They... |
| [T1547.003](https://attack.mitre.org/techniques/T1547/003) | ↳ Time Providers | Adversaries may abuse time providers to execute DLLs when the system boots. The Windows Time service (W32Time) enables time synchronization across and within domains.(Citation: Microsoft W32Time Feb... |
| [T1547.004](https://attack.mitre.org/techniques/T1547/004) | ↳ Winlogon Helper DLL | Adversaries may abuse features of Winlogon to execute DLLs and/or executables when a user logs in. Winlogon.exe is a Windows component responsible for actions at logon/logoff as well as the secure... |
| [T1547.005](https://attack.mitre.org/techniques/T1547/005) | ↳ Security Support Provider | Adversaries may abuse security support providers (SSPs) to execute DLLs when the system boots. Windows SSP DLLs are loaded into the Local Security Authority (LSA) process at system start. Once loaded... |
| [T1547.006](https://attack.mitre.org/techniques/T1547/006) | ↳ Kernel Modules and Extensions | Adversaries may modify the kernel to automatically execute programs on system boot. Loadable Kernel Modules (LKMs) are pieces of code that can be loaded and unloaded into the kernel upon demand. They... |
| [T1547.007](https://attack.mitre.org/techniques/T1547/007) | ↳ Re-opened Applications | Adversaries may modify plist files to automatically run an application when a user logs in. When a user logs out or restarts via the macOS Graphical User Interface (GUI), a prompt is provided to the... |
| [T1547.008](https://attack.mitre.org/techniques/T1547/008) | ↳ LSASS Driver | Adversaries may modify or add LSASS drivers to obtain persistence on compromised systems. The Windows security subsystem is a set of components that manage and enforce the security policy for a... |
| [T1547.009](https://attack.mitre.org/techniques/T1547/009) | ↳ Shortcut Modification | Adversaries may create or modify shortcuts that can execute a program during system boot or user login. Shortcuts or symbolic links are used to reference other files or programs that will be opened... |
| [T1547.010](https://attack.mitre.org/techniques/T1547/010) | ↳ Port Monitors | Adversaries may use port monitors to run an adversary supplied DLL during system boot for persistence or privilege escalation. A port monitor can be set through the <code>AddMonitor</code> API call... |
| [T1547.012](https://attack.mitre.org/techniques/T1547/012) | ↳ Print Processors | Adversaries may abuse print processors to run malicious DLLs during system boot for persistence and/or privilege escalation. Print processors are DLLs that are loaded by the print spooler service,... |
| [T1547.013](https://attack.mitre.org/techniques/T1547/013) | ↳ XDG Autostart Entries | Adversaries may add or modify XDG Autostart Entries to execute malicious programs or commands when a user’s desktop environment is loaded at login. XDG Autostart entries are available for any... |
| [T1547.014](https://attack.mitre.org/techniques/T1547/014) | ↳ Active Setup | Adversaries may achieve persistence by adding a Registry key to the Active Setup of the local machine. Active Setup is a Windows mechanism that is used to execute programs when a user logs in. The... |
| [T1547.015](https://attack.mitre.org/techniques/T1547/015) | ↳ Login Items | Adversaries may add login items to execute upon user login to gain persistence or escalate privileges. Login items are applications, documents, folders, or server connections that are automatically... |
| [T1548](https://attack.mitre.org/techniques/T1548) | Abuse Elevation Control Mechanism | Adversaries may circumvent mechanisms designed to control elevate privileges to gain higher-level permissions. Most modern systems contain native elevation control mechanisms that are intended to... |
| [T1548.001](https://attack.mitre.org/techniques/T1548/001) | ↳ Setuid and Setgid | An adversary may abuse configurations where an application has the setuid or setgid bits set in order to get code running in a different (and possibly more privileged) user’s context. On Linux or... |
| [T1548.002](https://attack.mitre.org/techniques/T1548/002) | ↳ Bypass User Account Control | Adversaries may bypass UAC mechanisms to elevate process privileges on system. Windows User Account Control (UAC) allows a program to elevate its privileges (tracked as integrity levels ranging from... |
| [T1548.003](https://attack.mitre.org/techniques/T1548/003) | ↳ Sudo and Sudo Caching | Adversaries may perform sudo caching and/or use the sudoers file to elevate privileges. Adversaries may do this to execute commands as other users or spawn processes with higher privileges. Within... |
| [T1548.004](https://attack.mitre.org/techniques/T1548/004) | ↳ Elevated Execution with Prompt | Adversaries may leverage the <code>AuthorizationExecuteWithPrivileges</code> API to escalate privileges by prompting the user for credentials.(Citation: AppleDocs AuthorizationExecuteWithPrivileges)... |
| [T1548.005](https://attack.mitre.org/techniques/T1548/005) | ↳ Temporary Elevated Cloud Access | Adversaries may abuse permission configurations that allow them to gain temporarily elevated access to cloud resources. Many cloud environments allow administrators to grant user or service accounts... |
| [T1548.006](https://attack.mitre.org/techniques/T1548/006) | ↳ TCC Manipulation | Adversaries can manipulate or abuse the Transparency, Consent, & Control (TCC) service or database to grant malicious executables elevated permissions. TCC is a Privacy & Security macOS control... |
| [T1574](https://attack.mitre.org/techniques/T1574) | Hijack Execution Flow | Adversaries may execute their own malicious payloads by hijacking the way operating systems run programs. Hijacking execution flow can be for the purposes of persistence, since this hijacked... |
| [T1574.001](https://attack.mitre.org/techniques/T1574/001) | ↳ DLL | Adversaries may abuse dynamic-link library files (DLLs) in order to achieve persistence, escalate privileges, and evade defenses. DLLs are libraries that contain code and data that can be... |
| [T1574.004](https://attack.mitre.org/techniques/T1574/004) | ↳ Dylib Hijacking | Adversaries may execute their own payloads by placing a malicious dynamic library (dylib) with an expected name in a path a victim application searches at runtime. The dynamic loader will try to find... |
| [T1574.005](https://attack.mitre.org/techniques/T1574/005) | ↳ Executable Installer File Permissions Weakness | Adversaries may execute their own malicious payloads by hijacking the binaries used by an installer. These processes may automatically execute specific binaries as part of their functionality or to... |
| [T1574.006](https://attack.mitre.org/techniques/T1574/006) | ↳ Dynamic Linker Hijacking | Adversaries may execute their own malicious payloads by hijacking environment variables the dynamic linker uses to load shared libraries. During the execution preparation phase of a program, the... |
| [T1574.007](https://attack.mitre.org/techniques/T1574/007) | ↳ Path Interception by PATH Environment Variable | Adversaries may execute their own malicious payloads by hijacking environment variables used to load libraries. The PATH environment variable contains a list of directories (User and System) that the... |
| [T1574.008](https://attack.mitre.org/techniques/T1574/008) | ↳ Path Interception by Search Order Hijacking | Adversaries may execute their own malicious payloads by hijacking the search order used to load other programs. Because some programs do not call other programs using the full path, adversaries may... |
| [T1574.009](https://attack.mitre.org/techniques/T1574/009) | ↳ Path Interception by Unquoted Path | Adversaries may execute their own malicious payloads by hijacking vulnerable file path references. Adversaries can take advantage of paths that lack surrounding quotations by placing an executable in... |
| [T1574.010](https://attack.mitre.org/techniques/T1574/010) | ↳ Services File Permissions Weakness | Adversaries may execute their own malicious payloads by hijacking the binaries used by services. Adversaries may use flaws in the permissions of Windows services to replace the binary that is... |
| [T1574.011](https://attack.mitre.org/techniques/T1574/011) | ↳ Services Registry Permissions Weakness | Adversaries may execute their own malicious payloads by hijacking the Registry entries used by services. Flaws in the permissions for Registry keys related to services can allow adversaries to... |
| [T1574.012](https://attack.mitre.org/techniques/T1574/012) | ↳ COR_PROFILER | Adversaries may leverage the COR_PROFILER environment variable to hijack the execution flow of programs that load the .NET CLR. The COR_PROFILER is a .NET Framework feature which allows developers to... |
| [T1574.013](https://attack.mitre.org/techniques/T1574/013) | ↳ KernelCallbackTable | Adversaries may abuse the <code>KernelCallbackTable</code> of a process to hijack its execution flow in order to run their own payloads.(Citation: Lazarus APT January 2022)(Citation: FinFisher... |
| [T1574.014](https://attack.mitre.org/techniques/T1574/014) | ↳ AppDomainManager | Adversaries may execute their own malicious payloads by hijacking how the .NET `AppDomainManager` loads assemblies. The .NET framework uses the `AppDomainManager` class to create and manage one or... |
| [T1611](https://attack.mitre.org/techniques/T1611) | Escape to Host | Adversaries may break out of a container or virtualized environment to gain access to the underlying host. This can allow an adversary access to other containerized or virtualized resources from the... |

---

### Defense Evasion

*215 techniques (47 parent, 168 sub-techniques)*

| T-Code | Name | Description |
|--------|------|-------------|
| [T1006](https://attack.mitre.org/techniques/T1006) | Direct Volume Access | Adversaries may directly access a volume to bypass file access controls and file system monitoring. Windows allows programs to have direct access to logical volumes. Programs with direct access may... |
| [T1014](https://attack.mitre.org/techniques/T1014) | Rootkit | Adversaries may use rootkits to hide the presence of programs, files, network connections, services, drivers, and other system components. Rootkits are programs that hide the existence of malware by... |
| [T1027](https://attack.mitre.org/techniques/T1027) | Obfuscated Files or Information | Adversaries may attempt to make an executable or file difficult to discover or analyze by encrypting, encoding, or otherwise obfuscating its contents on the system or in transit. This is common... |
| [T1027.001](https://attack.mitre.org/techniques/T1027/001) | ↳ Binary Padding | Adversaries may use binary padding to add junk data and change the on-disk representation of malware. This can be done without affecting the functionality or behavior of a binary, but can increase... |
| [T1027.002](https://attack.mitre.org/techniques/T1027/002) | ↳ Software Packing | Adversaries may perform software packing or virtual machine software protection to conceal their code. Software packing is a method of compressing or encrypting an executable. Packing an executable... |
| [T1027.003](https://attack.mitre.org/techniques/T1027/003) | ↳ Steganography | Adversaries may use steganography techniques in order to prevent the detection of hidden information. Steganographic techniques can be used to hide data in digital media such as images, audio tracks,... |
| [T1027.004](https://attack.mitre.org/techniques/T1027/004) | ↳ Compile After Delivery | Adversaries may attempt to make payloads difficult to discover and analyze by delivering files to victims as uncompiled code. Text-based source code files may subvert analysis and scrutiny from... |
| [T1027.005](https://attack.mitre.org/techniques/T1027/005) | ↳ Indicator Removal from Tools | Adversaries may remove indicators from tools if they believe their malicious tool was detected, quarantined, or otherwise curtailed. They can modify the tool by removing the indicator and using the... |
| [T1027.006](https://attack.mitre.org/techniques/T1027/006) | ↳ HTML Smuggling | Adversaries may smuggle data and files past content filters by hiding malicious payloads inside of seemingly benign HTML files. HTML documents can store large binary objects known as JavaScript Blobs... |
| [T1027.007](https://attack.mitre.org/techniques/T1027/007) | ↳ Dynamic API Resolution | Adversaries may obfuscate then dynamically resolve API functions called by their malware in order to conceal malicious functionalities and impair defensive analysis. Malware commonly uses various... |
| [T1027.008](https://attack.mitre.org/techniques/T1027/008) | ↳ Stripped Payloads | Adversaries may attempt to make a payload difficult to analyze by removing symbols, strings, and other human readable information. Scripts and executables may contain variables names and other... |
| [T1027.009](https://attack.mitre.org/techniques/T1027/009) | ↳ Embedded Payloads | Adversaries may embed payloads within other files to conceal malicious content from defenses. Otherwise seemingly benign files (such as scripts and executables) may be abused to carry and obfuscate... |
| [T1027.010](https://attack.mitre.org/techniques/T1027/010) | ↳ Command Obfuscation | Adversaries may obfuscate content during command execution to impede detection. Command-line obfuscation is a method of making strings and patterns within commands and scripts more difficult to... |
| [T1027.011](https://attack.mitre.org/techniques/T1027/011) | ↳ Fileless Storage | Adversaries may store data in "fileless" formats to conceal malicious activity from defenses. Fileless storage can be broadly defined as any format other than a file. Common examples of non-volatile... |
| [T1027.012](https://attack.mitre.org/techniques/T1027/012) | ↳ LNK Icon Smuggling | Adversaries may smuggle commands to download malicious payloads past content filters by hiding them within otherwise seemingly benign windows shortcut files. Windows shortcut files (.LNK) include... |
| [T1027.013](https://attack.mitre.org/techniques/T1027/013) | ↳ Encrypted/Encoded File | Adversaries may encrypt or encode files to obfuscate strings, bytes, and other specific patterns to impede detection. Encrypting and/or encoding file content aims to conceal malicious artifacts... |
| [T1027.014](https://attack.mitre.org/techniques/T1027/014) | ↳ Polymorphic Code | Adversaries may utilize polymorphic code (also known as metamorphic or mutating code) to evade detection. Polymorphic code is a type of software capable of changing its runtime footprint during code... |
| [T1027.015](https://attack.mitre.org/techniques/T1027/015) | ↳ Compression | Adversaries may use compression to obfuscate their payloads or files. Compressed file formats such as ZIP, gzip, 7z, and RAR can compress and archive multiple files together to make it easier and... |
| [T1027.016](https://attack.mitre.org/techniques/T1027/016) | ↳ Junk Code Insertion | Adversaries may use junk code / dead code to obfuscate a malware’s functionality. Junk code is code that either does not execute, or if it does execute, does not change the functionality of the code.... |
| [T1027.017](https://attack.mitre.org/techniques/T1027/017) | ↳ SVG Smuggling | Adversaries may smuggle data and files past content filters by hiding malicious payloads inside of seemingly benign SVG files.(Citation: Trustwave SVG Smuggling 2025) SVGs, or Scalable Vector... |
| [T1036](https://attack.mitre.org/techniques/T1036) | Masquerading | Adversaries may attempt to manipulate features of their artifacts to make them appear legitimate or benign to users and/or security tools. Masquerading occurs when the name or location of an object,... |
| [T1036.001](https://attack.mitre.org/techniques/T1036/001) | ↳ Invalid Code Signature | Adversaries may attempt to mimic features of valid code signatures to increase the chance of deceiving a user, analyst, or tool. Code signing provides a level of authenticity on a binary from the... |
| [T1036.002](https://attack.mitre.org/techniques/T1036/002) | ↳ Right-to-Left Override | Adversaries may abuse the right-to-left override (RTLO or RLO) character (U+202E) to disguise a string and/or file name to make it appear benign. RTLO is a non-printing Unicode character that causes... |
| [T1036.003](https://attack.mitre.org/techniques/T1036/003) | ↳ Rename Legitimate Utilities | Adversaries may rename legitimate / system utilities to try to evade security mechanisms concerning the usage of those utilities. Security monitoring and control mechanisms may be in place for... |
| [T1036.004](https://attack.mitre.org/techniques/T1036/004) | ↳ Masquerade Task or Service | Adversaries may attempt to manipulate the name of a task or service to make it appear legitimate or benign. Tasks/services executed by the Task Scheduler or systemd will typically be given a name... |
| [T1036.005](https://attack.mitre.org/techniques/T1036/005) | ↳ Match Legitimate Resource Name or Location | Adversaries may match or approximate the name or location of legitimate files, Registry keys, or other resources when naming/placing them. This is done for the sake of evading defenses and... |
| [T1036.006](https://attack.mitre.org/techniques/T1036/006) | ↳ Space after Filename | Adversaries can hide a program's true filetype by changing the extension of a file. With certain file types (specifically this does not work with .app extensions), appending a space to the end of a... |
| [T1036.007](https://attack.mitre.org/techniques/T1036/007) | ↳ Double File Extension | Adversaries may abuse a double extension in the filename as a means of masquerading the true file type. A file name may include a secondary file type extension that may cause only the first extension... |
| [T1036.008](https://attack.mitre.org/techniques/T1036/008) | ↳ Masquerade File Type | Adversaries may masquerade malicious payloads as legitimate files through changes to the payload's formatting, including the file’s signature, extension, icon, and contents. Various file types have a... |
| [T1036.009](https://attack.mitre.org/techniques/T1036/009) | ↳ Break Process Trees | An adversary may attempt to evade process tree-based analysis by modifying executed malware's parent process ID (PPID). If endpoint protection software leverages the “parent-child" relationship for... |
| [T1036.010](https://attack.mitre.org/techniques/T1036/010) | ↳ Masquerade Account Name | Adversaries may match or approximate the names of legitimate accounts to make newly created ones appear benign. This will typically occur during [Create... |
| [T1036.011](https://attack.mitre.org/techniques/T1036/011) | ↳ Overwrite Process Arguments | Adversaries may modify a process's in-memory arguments to change its name in order to appear as a legitimate or benign process. On Linux, the operating system stores command-line arguments in the... |
| [T1036.012](https://attack.mitre.org/techniques/T1036/012) | ↳ Browser Fingerprint | Adversaries may attempt to blend in with legitimate traffic by spoofing browser and system attributes like operating system, system language, platform, user-agent string, resolution, time zone, etc.... |
| [T1055](https://attack.mitre.org/techniques/T1055) | Process Injection | Adversaries may inject code into processes in order to evade process-based defenses as well as possibly elevate privileges. Process injection is a method of executing arbitrary code in the address... |
| [T1055.001](https://attack.mitre.org/techniques/T1055/001) | ↳ Dynamic-link Library Injection | Adversaries may inject dynamic-link libraries (DLLs) into processes in order to evade process-based defenses as well as possibly elevate privileges. DLL injection is a method of executing arbitrary... |
| [T1055.002](https://attack.mitre.org/techniques/T1055/002) | ↳ Portable Executable Injection | Adversaries may inject portable executables (PE) into processes in order to evade process-based defenses as well as possibly elevate privileges. PE injection is a method of executing arbitrary code... |
| [T1055.003](https://attack.mitre.org/techniques/T1055/003) | ↳ Thread Execution Hijacking | Adversaries may inject malicious code into hijacked processes in order to evade process-based defenses as well as possibly elevate privileges. Thread Execution Hijacking is a method of executing... |
| [T1055.004](https://attack.mitre.org/techniques/T1055/004) | ↳ Asynchronous Procedure Call | Adversaries may inject malicious code into processes via the asynchronous procedure call (APC) queue in order to evade process-based defenses as well as possibly elevate privileges. APC injection is... |
| [T1055.005](https://attack.mitre.org/techniques/T1055/005) | ↳ Thread Local Storage | Adversaries may inject malicious code into processes via thread local storage (TLS) callbacks in order to evade process-based defenses as well as possibly elevate privileges. TLS callback injection... |
| [T1055.008](https://attack.mitre.org/techniques/T1055/008) | ↳ Ptrace System Calls | Adversaries may inject malicious code into processes via ptrace (process trace) system calls in order to evade process-based defenses as well as possibly elevate privileges. Ptrace system call... |
| [T1055.009](https://attack.mitre.org/techniques/T1055/009) | ↳ Proc Memory | Adversaries may inject malicious code into processes via the /proc filesystem in order to evade process-based defenses as well as possibly elevate privileges. Proc memory injection is a method of... |
| [T1055.011](https://attack.mitre.org/techniques/T1055/011) | ↳ Extra Window Memory Injection | Adversaries may inject malicious code into process via Extra Window Memory (EWM) in order to evade process-based defenses as well as possibly elevate privileges. EWM injection is a method of... |
| [T1055.012](https://attack.mitre.org/techniques/T1055/012) | ↳ Process Hollowing | Adversaries may inject malicious code into suspended and hollowed processes in order to evade process-based defenses. Process hollowing is a method of executing arbitrary code in the address space of... |
| [T1055.013](https://attack.mitre.org/techniques/T1055/013) | ↳ Process Doppelgänging | Adversaries may inject malicious code into process via process doppelgänging in order to evade process-based defenses as well as possibly elevate privileges. Process doppelgänging is a method of... |
| [T1055.014](https://attack.mitre.org/techniques/T1055/014) | ↳ VDSO Hijacking | Adversaries may inject malicious code into processes via VDSO hijacking in order to evade process-based defenses as well as possibly elevate privileges. Virtual dynamic shared object (vdso) hijacking... |
| [T1055.015](https://attack.mitre.org/techniques/T1055/015) | ↳ ListPlanting | Adversaries may abuse list-view controls to inject malicious code into hijacked processes in order to evade process-based defenses as well as possibly elevate privileges. ListPlanting is a method of... |
| [T1070](https://attack.mitre.org/techniques/T1070) | Indicator Removal | Adversaries may delete or modify artifacts generated within systems to remove evidence of their presence or hinder defenses. Various artifacts may be created by an adversary or something that can be... |
| [T1070.001](https://attack.mitre.org/techniques/T1070/001) | ↳ Clear Windows Event Logs | Adversaries may clear Windows Event Logs to hide the activity of an intrusion. Windows Event Logs are a record of a computer's alerts and notifications. There are three system-defined sources of... |
| [T1070.002](https://attack.mitre.org/techniques/T1070/002) | ↳ Clear Linux or Mac System Logs | Adversaries may clear system logs to hide evidence of an intrusion. macOS and Linux both keep track of system or user-initiated actions via system logs. The majority of native system logging is... |
| [T1070.003](https://attack.mitre.org/techniques/T1070/003) | ↳ Clear Command History | In addition to clearing system logs, an adversary may clear the command history of a compromised account to conceal the actions undertaken during an intrusion. Various command interpreters keep track... |
| [T1070.004](https://attack.mitre.org/techniques/T1070/004) | ↳ File Deletion | Adversaries may delete files left behind by the actions of their intrusion activity. Malware, tools, or other non-native files dropped or created on a system by an adversary (ex: [Ingress Tool... |
| [T1070.005](https://attack.mitre.org/techniques/T1070/005) | ↳ Network Share Connection Removal | Adversaries may remove share connections that are no longer useful in order to clean up traces of their operation. Windows shared drive and [SMB/Windows Admin... |
| [T1070.006](https://attack.mitre.org/techniques/T1070/006) | ↳ Timestomp | Adversaries may modify file time attributes to hide new files or changes to existing files. Timestomping is a technique that modifies the timestamps of a file (the modify, access, create, and change... |
| [T1070.007](https://attack.mitre.org/techniques/T1070/007) | ↳ Clear Network Connection History and Configurations | Adversaries may clear or remove evidence of malicious network connections in order to clean up traces of their operations. Configuration settings as well as various artifacts that highlight... |
| [T1070.008](https://attack.mitre.org/techniques/T1070/008) | ↳ Clear Mailbox Data | Adversaries may modify mail and mail application data to remove evidence of their activity. Email applications allow users and other programs to export and delete mailbox data via command line tools... |
| [T1070.009](https://attack.mitre.org/techniques/T1070/009) | ↳ Clear Persistence | Adversaries may clear artifacts associated with previously established persistence on a host system to remove evidence of their activity. This may involve various actions, such as removing services,... |
| [T1070.010](https://attack.mitre.org/techniques/T1070/010) | ↳ Relocate Malware | Once a payload is delivered, adversaries may reproduce copies of the same malware on the victim system to remove evidence of their presence and/or avoid defenses. Copying malware payloads to new... |
| [T1078](https://attack.mitre.org/techniques/T1078) | Valid Accounts | Adversaries may obtain and abuse credentials of existing accounts as a means of gaining Initial Access, Persistence, Privilege Escalation, or Defense Evasion. Compromised credentials may be used to... |
| [T1078.001](https://attack.mitre.org/techniques/T1078/001) | ↳ Default Accounts | Adversaries may obtain and abuse credentials of a default account as a means of gaining Initial Access, Persistence, Privilege Escalation, or Defense Evasion. Default accounts are those that are... |
| [T1078.002](https://attack.mitre.org/techniques/T1078/002) | ↳ Domain Accounts | Adversaries may obtain and abuse credentials of a domain account as a means of gaining Initial Access, Persistence, Privilege Escalation, or Defense Evasion.(Citation: TechNet Credential Theft)... |
| [T1078.003](https://attack.mitre.org/techniques/T1078/003) | ↳ Local Accounts | Adversaries may obtain and abuse credentials of a local account as a means of gaining Initial Access, Persistence, Privilege Escalation, or Defense Evasion. Local accounts are those configured by an... |
| [T1078.004](https://attack.mitre.org/techniques/T1078/004) | ↳ Cloud Accounts | Valid accounts in cloud environments may allow adversaries to perform actions to achieve Initial Access, Persistence, Privilege Escalation, or Defense Evasion. Cloud accounts are those created and... |
| [T1112](https://attack.mitre.org/techniques/T1112) | Modify Registry | Adversaries may interact with the Windows Registry as part of a variety of other techniques to aid in defense evasion, persistence, and execution. Access to specific areas of the Registry depends on... |
| [T1127](https://attack.mitre.org/techniques/T1127) | Trusted Developer Utilities Proxy Execution | Adversaries may take advantage of trusted developer utilities to proxy execution of malicious payloads. There are many utilities used for software development related tasks that can be used to... |
| [T1127.001](https://attack.mitre.org/techniques/T1127/001) | ↳ MSBuild | Adversaries may use MSBuild to proxy execution of code through a trusted Windows utility. MSBuild.exe (Microsoft Build Engine) is a software build platform used by Visual Studio. It handles XML... |
| [T1127.002](https://attack.mitre.org/techniques/T1127/002) | ↳ ClickOnce | Adversaries may use ClickOnce applications (.appref-ms and .application files) to proxy execution of code through a trusted Windows utility.(Citation: Burke/CISA ClickOnce BlackHat) ClickOnce is a... |
| [T1127.003](https://attack.mitre.org/techniques/T1127/003) | ↳ JamPlus | Adversaries may use `JamPlus` to proxy the execution of a malicious script. `JamPlus` is a build utility tool for code and data build systems. It works with several popular compilers and can be used... |
| [T1134](https://attack.mitre.org/techniques/T1134) | Access Token Manipulation | Adversaries may modify access tokens to operate under a different user or system security context to perform actions and bypass access controls. Windows uses access tokens to determine the ownership... |
| [T1134.001](https://attack.mitre.org/techniques/T1134/001) | ↳ Token Impersonation/Theft | Adversaries may duplicate then impersonate another user's existing token to escalate privileges and bypass access controls. For example, an adversary can duplicate an existing token using... |
| [T1134.002](https://attack.mitre.org/techniques/T1134/002) | ↳ Create Process with Token | Adversaries may create a new process with an existing token to escalate privileges and bypass access controls. Processes can be created with the token and resulting security context of another user... |
| [T1134.003](https://attack.mitre.org/techniques/T1134/003) | ↳ Make and Impersonate Token | Adversaries may make new tokens and impersonate users to escalate privileges and bypass access controls. For example, if an adversary has a username and password but the user is not logged onto the... |
| [T1134.004](https://attack.mitre.org/techniques/T1134/004) | ↳ Parent PID Spoofing | Adversaries may spoof the parent process identifier (PPID) of a new process to evade process-monitoring defenses or to elevate privileges. New processes are typically spawned directly from their... |
| [T1134.005](https://attack.mitre.org/techniques/T1134/005) | ↳ SID-History Injection | Adversaries may use SID-History Injection to escalate privileges and bypass access controls. The Windows security identifier (SID) is a unique value that identifies a user or group account. SIDs are... |
| [T1140](https://attack.mitre.org/techniques/T1140) | Deobfuscate/Decode Files or Information | Adversaries may use [Obfuscated Files or Information](https://attack.mitre.org/techniques/T1027) to hide artifacts of an intrusion from analysis. They may require separate mechanisms to decode or... |
| [T1197](https://attack.mitre.org/techniques/T1197) | BITS Jobs | Adversaries may abuse BITS jobs to persistently execute code and perform various background tasks. Windows Background Intelligent Transfer Service (BITS) is a low-bandwidth, asynchronous file... |
| [T1202](https://attack.mitre.org/techniques/T1202) | Indirect Command Execution | Adversaries may abuse utilities that allow for command execution to bypass security restrictions that limit the use of command-line interpreters. Various Windows utilities may be used to execute... |
| [T1205](https://attack.mitre.org/techniques/T1205) | Traffic Signaling | Adversaries may use traffic signaling to hide open ports or other malicious functionality used for persistence or command and control. Traffic signaling involves the use of a magic value or sequence... |
| [T1205.001](https://attack.mitre.org/techniques/T1205/001) | ↳ Port Knocking | Adversaries may use port knocking to hide open ports used for persistence or command and control. To enable a port, an adversary sends a series of attempted connections to a predefined sequence of... |
| [T1205.002](https://attack.mitre.org/techniques/T1205/002) | ↳ Socket Filters | Adversaries may attach filters to a network socket to monitor then activate backdoors used for persistence or command and control. With elevated permissions, adversaries can use features such as the... |
| [T1207](https://attack.mitre.org/techniques/T1207) | Rogue Domain Controller | Adversaries may register a rogue Domain Controller to enable manipulation of Active Directory data. DCShadow may be used to create a rogue Domain Controller (DC). DCShadow is a method of manipulating... |
| [T1211](https://attack.mitre.org/techniques/T1211) | Exploitation for Defense Evasion | Adversaries may exploit a system or application vulnerability to bypass security features. Exploitation of a vulnerability occurs when an adversary takes advantage of a programming error in a... |
| [T1216](https://attack.mitre.org/techniques/T1216) | System Script Proxy Execution | Adversaries may use trusted scripts, often signed with certificates, to proxy the execution of malicious files. Several Microsoft signed scripts that have been downloaded from Microsoft or are... |
| [T1216.001](https://attack.mitre.org/techniques/T1216/001) | ↳ PubPrn | Adversaries may use PubPrn to proxy execution of malicious remote files. PubPrn.vbs is a [Visual Basic](https://attack.mitre.org/techniques/T1059/005) script that publishes a printer to Active... |
| [T1216.002](https://attack.mitre.org/techniques/T1216/002) | ↳ SyncAppvPublishingServer | Adversaries may abuse SyncAppvPublishingServer.vbs to proxy execution of malicious [PowerShell](https://attack.mitre.org/techniques/T1059/001) commands. SyncAppvPublishingServer.vbs is a Visual Basic... |
| [T1218](https://attack.mitre.org/techniques/T1218) | System Binary Proxy Execution | Adversaries may bypass process and/or signature-based defenses by proxying execution of malicious content with signed, or otherwise trusted, binaries. Binaries used in this technique are often... |
| [T1218.001](https://attack.mitre.org/techniques/T1218/001) | ↳ Compiled HTML File | Adversaries may abuse Compiled HTML files (.chm) to conceal malicious code. CHM files are commonly distributed as part of the Microsoft HTML Help system. CHM files are compressed compilations of... |
| [T1218.002](https://attack.mitre.org/techniques/T1218/002) | ↳ Control Panel | Adversaries may abuse control.exe to proxy execution of malicious payloads. The Windows Control Panel process binary (control.exe) handles execution of Control Panel items, which are utilities that... |
| [T1218.003](https://attack.mitre.org/techniques/T1218/003) | ↳ CMSTP | Adversaries may abuse CMSTP to proxy execution of malicious code. The Microsoft Connection Manager Profile Installer (CMSTP.exe) is a command-line program used to install Connection Manager service... |
| [T1218.004](https://attack.mitre.org/techniques/T1218/004) | ↳ InstallUtil | Adversaries may use InstallUtil to proxy execution of code through a trusted Windows utility. InstallUtil is a command-line utility that allows for installation and uninstallation of resources by... |
| [T1218.005](https://attack.mitre.org/techniques/T1218/005) | ↳ Mshta | Adversaries may abuse mshta.exe to proxy execution of malicious .hta files and Javascript or VBScript through a trusted Windows utility. There are several examples of different types of threats... |
| [T1218.007](https://attack.mitre.org/techniques/T1218/007) | ↳ Msiexec | Adversaries may abuse msiexec.exe to proxy execution of malicious payloads. Msiexec.exe is the command-line utility for the Windows Installer and is thus commonly associated with executing... |
| [T1218.008](https://attack.mitre.org/techniques/T1218/008) | ↳ Odbcconf | Adversaries may abuse odbcconf.exe to proxy execution of malicious payloads. Odbcconf.exe is a Windows utility that allows you to configure Open Database Connectivity (ODBC) drivers and data source... |
| [T1218.009](https://attack.mitre.org/techniques/T1218/009) | ↳ Regsvcs/Regasm | Adversaries may abuse Regsvcs and Regasm to proxy execution of code through a trusted Windows utility. Regsvcs and Regasm are Windows command-line utilities that are used to register .NET [Component... |
| [T1218.010](https://attack.mitre.org/techniques/T1218/010) | ↳ Regsvr32 | Adversaries may abuse Regsvr32.exe to proxy execution of malicious code. Regsvr32.exe is a command-line program used to register and unregister object linking and embedding controls, including... |
| [T1218.011](https://attack.mitre.org/techniques/T1218/011) | ↳ Rundll32 | Adversaries may abuse rundll32.exe to proxy execution of malicious code. Using rundll32.exe, vice executing directly (i.e. [Shared Modules](https://attack.mitre.org/techniques/T1129)), may avoid... |
| [T1218.012](https://attack.mitre.org/techniques/T1218/012) | ↳ Verclsid | Adversaries may abuse verclsid.exe to proxy execution of malicious code. Verclsid.exe is known as the Extension CLSID Verification Host and is responsible for verifying each shell extension before... |
| [T1218.013](https://attack.mitre.org/techniques/T1218/013) | ↳ Mavinject | Adversaries may abuse mavinject.exe to proxy execution of malicious code. Mavinject.exe is the Microsoft Application Virtualization Injector, a Windows utility that can inject code into external... |
| [T1218.014](https://attack.mitre.org/techniques/T1218/014) | ↳ MMC | Adversaries may abuse mmc.exe to proxy execution of malicious .msc files. Microsoft Management Console (MMC) is a binary that may be signed by Microsoft and is used in several ways in either its GUI... |
| [T1218.015](https://attack.mitre.org/techniques/T1218/015) | ↳ Electron Applications | Adversaries may abuse components of the Electron framework to execute malicious code. The Electron framework hosts many common applications such as Signal, Slack, and Microsoft Teams.(Citation:... |
| [T1220](https://attack.mitre.org/techniques/T1220) | XSL Script Processing | Adversaries may bypass application control and obscure execution of code by embedding scripts inside XSL files. Extensible Stylesheet Language (XSL) files are commonly used to describe the processing... |
| [T1221](https://attack.mitre.org/techniques/T1221) | Template Injection | Adversaries may create or modify references in user document templates to conceal malicious code or force authentication attempts. For example, Microsoft’s Office Open XML (OOXML) specification... |
| [T1222](https://attack.mitre.org/techniques/T1222) | File and Directory Permissions Modification | Adversaries may modify file or directory permissions/attributes to evade access control lists (ACLs) and access protected files.(Citation: Hybrid Analysis Icacls1 June 2018)(Citation: Hybrid Analysis... |
| [T1222.001](https://attack.mitre.org/techniques/T1222/001) | ↳ Windows File and Directory Permissions Modification | Adversaries may modify file or directory permissions/attributes to evade access control lists (ACLs) and access protected files.(Citation: Hybrid Analysis Icacls1 June 2018)(Citation: Hybrid Analysis... |
| [T1222.002](https://attack.mitre.org/techniques/T1222/002) | ↳ Linux and Mac File and Directory Permissions Modification | Adversaries may modify file or directory permissions/attributes to evade access control lists (ACLs) and access protected files.(Citation: Hybrid Analysis Icacls1 June 2018)(Citation: Hybrid Analysis... |
| [T1480](https://attack.mitre.org/techniques/T1480) | Execution Guardrails | Adversaries may use execution guardrails to constrain execution or actions based on adversary supplied and environment specific conditions that are expected to be present on the target. Guardrails... |
| [T1480.001](https://attack.mitre.org/techniques/T1480/001) | ↳ Environmental Keying | Adversaries may environmentally key payloads or other features of malware to evade defenses and constraint execution to a specific target environment. Environmental keying uses cryptography to... |
| [T1480.002](https://attack.mitre.org/techniques/T1480/002) | ↳ Mutual Exclusion | Adversaries may constrain execution or actions based on the presence of a mutex associated with malware. A mutex is a locking mechanism used to synchronize access to a resource. Only one thread or... |
| [T1484](https://attack.mitre.org/techniques/T1484) | Domain or Tenant Policy Modification | Adversaries may modify the configuration settings of a domain or identity tenant to evade defenses and/or escalate privileges in centrally managed environments. Such services provide a centralized... |
| [T1484.001](https://attack.mitre.org/techniques/T1484/001) | ↳ Group Policy Modification | Adversaries may modify Group Policy Objects (GPOs) to subvert the intended discretionary access controls for a domain, usually with the intention of escalating privileges on the domain. Group policy... |
| [T1484.002](https://attack.mitre.org/techniques/T1484/002) | ↳ Trust Modification | Adversaries may add new domain trusts, modify the properties of existing domain trusts, or otherwise change the configuration of trust relationships between domains and tenants to evade defenses... |
| [T1497](https://attack.mitre.org/techniques/T1497) | Virtualization/Sandbox Evasion | Adversaries may employ various means to detect and avoid virtualization and analysis environments. This may include changing behaviors based on the results of checks for the presence of artifacts... |
| [T1497.001](https://attack.mitre.org/techniques/T1497/001) | ↳ System Checks | Adversaries may employ various system checks to detect and avoid virtualization and analysis environments. This may include changing behaviors based on the results of checks for the presence of... |
| [T1497.002](https://attack.mitre.org/techniques/T1497/002) | ↳ User Activity Based Checks | Adversaries may employ various user activity checks to detect and avoid virtualization and analysis environments. This may include changing behaviors based on the results of checks for the presence... |
| [T1497.003](https://attack.mitre.org/techniques/T1497/003) | ↳ Time Based Checks | Adversaries may employ various time-based methods to detect virtualization and analysis environments, particularly those that attempt to manipulate time mechanisms to simulate longer elapses of time.... |
| [T1535](https://attack.mitre.org/techniques/T1535) | Unused/Unsupported Cloud Regions | Adversaries may create cloud instances in unused geographic service regions in order to evade detection. Access is usually obtained through compromising accounts used to manage cloud infrastructure.... |
| [T1542](https://attack.mitre.org/techniques/T1542) | Pre-OS Boot | Adversaries may abuse Pre-OS Boot mechanisms as a way to establish persistence on a system. During the booting process of a computer, firmware and various startup services are loaded before the... |
| [T1542.001](https://attack.mitre.org/techniques/T1542/001) | ↳ System Firmware | Adversaries may modify system firmware to persist on systems.The BIOS (Basic Input/Output System) and The Unified Extensible Firmware Interface (UEFI) or Extensible Firmware Interface (EFI) are... |
| [T1542.002](https://attack.mitre.org/techniques/T1542/002) | ↳ Component Firmware | Adversaries may modify component firmware to persist on systems. Some adversaries may employ sophisticated means to compromise computer components and install malicious firmware that will execute... |
| [T1542.003](https://attack.mitre.org/techniques/T1542/003) | ↳ Bootkit | Adversaries may use bootkits to persist on systems. A bootkit is a malware variant that modifies the boot sectors of a hard drive, allowing malicious code to execute before a computer's operating... |
| [T1542.004](https://attack.mitre.org/techniques/T1542/004) | ↳ ROMMONkit | Adversaries may abuse the ROM Monitor (ROMMON) by loading an unauthorized firmware with adversary code to provide persistent access and manipulate device behavior that is difficult to detect.... |
| [T1542.005](https://attack.mitre.org/techniques/T1542/005) | ↳ TFTP Boot | Adversaries may abuse netbooting to load an unauthorized network device operating system from a Trivial File Transfer Protocol (TFTP) server. TFTP boot (netbooting) is commonly used by network... |
| [T1548](https://attack.mitre.org/techniques/T1548) | Abuse Elevation Control Mechanism | Adversaries may circumvent mechanisms designed to control elevate privileges to gain higher-level permissions. Most modern systems contain native elevation control mechanisms that are intended to... |
| [T1548.001](https://attack.mitre.org/techniques/T1548/001) | ↳ Setuid and Setgid | An adversary may abuse configurations where an application has the setuid or setgid bits set in order to get code running in a different (and possibly more privileged) user’s context. On Linux or... |
| [T1548.002](https://attack.mitre.org/techniques/T1548/002) | ↳ Bypass User Account Control | Adversaries may bypass UAC mechanisms to elevate process privileges on system. Windows User Account Control (UAC) allows a program to elevate its privileges (tracked as integrity levels ranging from... |
| [T1548.003](https://attack.mitre.org/techniques/T1548/003) | ↳ Sudo and Sudo Caching | Adversaries may perform sudo caching and/or use the sudoers file to elevate privileges. Adversaries may do this to execute commands as other users or spawn processes with higher privileges. Within... |
| [T1548.004](https://attack.mitre.org/techniques/T1548/004) | ↳ Elevated Execution with Prompt | Adversaries may leverage the <code>AuthorizationExecuteWithPrivileges</code> API to escalate privileges by prompting the user for credentials.(Citation: AppleDocs AuthorizationExecuteWithPrivileges)... |
| [T1548.005](https://attack.mitre.org/techniques/T1548/005) | ↳ Temporary Elevated Cloud Access | Adversaries may abuse permission configurations that allow them to gain temporarily elevated access to cloud resources. Many cloud environments allow administrators to grant user or service accounts... |
| [T1548.006](https://attack.mitre.org/techniques/T1548/006) | ↳ TCC Manipulation | Adversaries can manipulate or abuse the Transparency, Consent, & Control (TCC) service or database to grant malicious executables elevated permissions. TCC is a Privacy & Security macOS control... |
| [T1550](https://attack.mitre.org/techniques/T1550) | Use Alternate Authentication Material | Adversaries may use alternate authentication material, such as password hashes, Kerberos tickets, and application access tokens, in order to move laterally within an environment and bypass normal... |
| [T1550.001](https://attack.mitre.org/techniques/T1550/001) | ↳ Application Access Token | Adversaries may use stolen application access tokens to bypass the typical authentication process and access restricted accounts, information, or services on remote systems. These tokens are... |
| [T1550.002](https://attack.mitre.org/techniques/T1550/002) | ↳ Pass the Hash | Adversaries may “pass the hash” using stolen password hashes to move laterally within an environment, bypassing normal system access controls. Pass the hash (PtH) is a method of authenticating as a... |
| [T1550.003](https://attack.mitre.org/techniques/T1550/003) | ↳ Pass the Ticket | Adversaries may “pass the ticket” using stolen Kerberos tickets to move laterally within an environment, bypassing normal system access controls. Pass the ticket (PtT) is a method of authenticating... |
| [T1550.004](https://attack.mitre.org/techniques/T1550/004) | ↳ Web Session Cookie | Adversaries can use stolen session cookies to authenticate to web applications and services. This technique bypasses some multi-factor authentication protocols since the session is already... |
| [T1553](https://attack.mitre.org/techniques/T1553) | Subvert Trust Controls | Adversaries may undermine security controls that will either warn users of untrusted activity or prevent execution of untrusted programs. Operating systems and security products may contain... |
| [T1553.001](https://attack.mitre.org/techniques/T1553/001) | ↳ Gatekeeper Bypass | Adversaries may modify file attributes and subvert Gatekeeper functionality to evade user prompts and execute untrusted programs. Gatekeeper is a set of technologies that act as layer of Apple’s... |
| [T1553.002](https://attack.mitre.org/techniques/T1553/002) | ↳ Code Signing | Adversaries may create, acquire, or steal code signing materials to sign their malware or tools. Code signing provides a level of authenticity on a binary from the developer and a guarantee that the... |
| [T1553.003](https://attack.mitre.org/techniques/T1553/003) | ↳ SIP and Trust Provider Hijacking | Adversaries may tamper with SIP and trust provider components to mislead the operating system and application control tools when conducting signature validation checks. In user mode, Windows... |
| [T1553.004](https://attack.mitre.org/techniques/T1553/004) | ↳ Install Root Certificate | Adversaries may install a root certificate on a compromised system to avoid warnings when connecting to adversary controlled web servers. Root certificates are used in public key cryptography to... |
| [T1553.005](https://attack.mitre.org/techniques/T1553/005) | ↳ Mark-of-the-Web Bypass | Adversaries may abuse specific file formats to subvert Mark-of-the-Web (MOTW) controls. In Windows, when files are downloaded from the Internet, they are tagged with a hidden NTFS Alternate Data... |
| [T1553.006](https://attack.mitre.org/techniques/T1553/006) | ↳ Code Signing Policy Modification | Adversaries may modify code signing policies to enable execution of unsigned or self-signed code. Code signing provides a level of authenticity on a program from a developer and a guarantee that the... |
| [T1556](https://attack.mitre.org/techniques/T1556) | Modify Authentication Process | Adversaries may modify authentication mechanisms and processes to access user credentials or enable otherwise unwarranted access to accounts. The authentication process is handled by mechanisms, such... |
| [T1556.001](https://attack.mitre.org/techniques/T1556/001) | ↳ Domain Controller Authentication | Adversaries may patch the authentication process on a domain controller to bypass the typical authentication mechanisms and enable access to accounts. Malware may be used to inject false credentials... |
| [T1556.002](https://attack.mitre.org/techniques/T1556/002) | ↳ Password Filter DLL | Adversaries may register malicious password filter dynamic link libraries (DLLs) into the authentication process to acquire user credentials as they are validated. Windows password filters are... |
| [T1556.003](https://attack.mitre.org/techniques/T1556/003) | ↳ Pluggable Authentication Modules | Adversaries may modify pluggable authentication modules (PAM) to access user credentials or enable otherwise unwarranted access to accounts. PAM is a modular system of configuration files, libraries,... |
| [T1556.004](https://attack.mitre.org/techniques/T1556/004) | ↳ Network Device Authentication | Adversaries may use [Patch System Image](https://attack.mitre.org/techniques/T1601/001) to hard code a password in the operating system, thus bypassing of native authentication mechanisms for local... |
| [T1556.005](https://attack.mitre.org/techniques/T1556/005) | ↳ Reversible Encryption | An adversary may abuse Active Directory authentication encryption properties to gain access to credentials on Windows systems. The <code>AllowReversiblePasswordEncryption</code> property specifies... |
| [T1556.006](https://attack.mitre.org/techniques/T1556/006) | ↳ Multi-Factor Authentication | Adversaries may disable or modify multi-factor authentication (MFA) mechanisms to enable persistent access to compromised accounts. Once adversaries have gained access to a network by either... |
| [T1556.007](https://attack.mitre.org/techniques/T1556/007) | ↳ Hybrid Identity | Adversaries may patch, modify, or otherwise backdoor cloud authentication processes that are tied to on-premises user identities in order to bypass typical authentication mechanisms, access... |
| [T1556.008](https://attack.mitre.org/techniques/T1556/008) | ↳ Network Provider DLL | Adversaries may register malicious network provider dynamic link libraries (DLLs) to capture cleartext user credentials during the authentication process. Network provider DLLs allow Windows to... |
| [T1556.009](https://attack.mitre.org/techniques/T1556/009) | ↳ Conditional Access Policies | Adversaries may disable or modify conditional access policies to enable persistent access to compromised accounts. Conditional access policies are additional verifications used by identity providers... |
| [T1562](https://attack.mitre.org/techniques/T1562) | Impair Defenses | Adversaries may maliciously modify components of a victim environment in order to hinder or disable defensive mechanisms. This not only involves impairing preventative defenses, such as firewalls and... |
| [T1562.001](https://attack.mitre.org/techniques/T1562/001) | ↳ Disable or Modify Tools | Adversaries may modify and/or disable security tools to avoid possible detection of their malware/tools and activities. This may take many forms, such as killing security software processes or... |
| [T1562.002](https://attack.mitre.org/techniques/T1562/002) | ↳ Disable Windows Event Logging | Adversaries may disable Windows event logging to limit data that can be leveraged for detections and audits. Windows event logs record user and system activity such as login attempts, process... |
| [T1562.003](https://attack.mitre.org/techniques/T1562/003) | ↳ Impair Command History Logging | Adversaries may impair command history logging to hide commands they run on a compromised system. Various command interpreters keep track of the commands users type in their terminal so that users... |
| [T1562.004](https://attack.mitre.org/techniques/T1562/004) | ↳ Disable or Modify System Firewall | Adversaries may disable or modify system firewalls in order to bypass controls limiting network usage. Changes could be disabling the entire mechanism as well as adding, deleting, or modifying... |
| [T1562.006](https://attack.mitre.org/techniques/T1562/006) | ↳ Indicator Blocking | An adversary may attempt to block indicators or events typically captured by sensors from being gathered and analyzed. This could include maliciously redirecting(Citation: Microsoft Lamin Sept 2017)... |
| [T1562.007](https://attack.mitre.org/techniques/T1562/007) | ↳ Disable or Modify Cloud Firewall | Adversaries may disable or modify a firewall within a cloud environment to bypass controls that limit access to cloud resources. Cloud firewalls are separate from system firewalls that are described... |
| [T1562.008](https://attack.mitre.org/techniques/T1562/008) | ↳ Disable or Modify Cloud Logs | An adversary may disable or modify cloud logging capabilities and integrations to limit what data is collected on their activities and avoid detection. Cloud environments allow for collection and... |
| [T1562.009](https://attack.mitre.org/techniques/T1562/009) | ↳ Safe Mode Boot | Adversaries may abuse Windows safe mode to disable endpoint defenses. Safe mode starts up the Windows operating system with a limited set of drivers and services. Third-party security software such... |
| [T1562.010](https://attack.mitre.org/techniques/T1562/010) | ↳ Downgrade Attack | Adversaries may downgrade or use a version of system features that may be outdated, vulnerable, and/or does not support updated security controls. Downgrade attacks typically take advantage of a... |
| [T1562.011](https://attack.mitre.org/techniques/T1562/011) | ↳ Spoof Security Alerting | Adversaries may spoof security alerting from tools, presenting false evidence to impair defenders’ awareness of malicious activity.(Citation: BlackBasta) Messages produced by defensive tools contain... |
| [T1562.012](https://attack.mitre.org/techniques/T1562/012) | ↳ Disable or Modify Linux Audit System | Adversaries may disable or modify the Linux audit system to hide malicious activity and avoid detection. Linux admins use the Linux Audit system to track security-relevant information on a system.... |
| [T1562.013](https://attack.mitre.org/techniques/T1562/013) | ↳ Disable or Modify Network Device Firewall | Adversaries may disable network device-based firewall mechanisms entirely or add, delete, or modify particular rules in order to bypass controls limiting network usage. Modifying or disabling a... |
| [T1564](https://attack.mitre.org/techniques/T1564) | Hide Artifacts | Adversaries may attempt to hide artifacts associated with their behaviors to evade detection. Operating systems may have features to hide various artifacts, such as important system files and... |
| [T1564.001](https://attack.mitre.org/techniques/T1564/001) | ↳ Hidden Files and Directories | Adversaries may set files and directories to be hidden to evade detection mechanisms. To prevent normal users from accidentally changing special files on a system, most operating systems have the... |
| [T1564.002](https://attack.mitre.org/techniques/T1564/002) | ↳ Hidden Users | Adversaries may use hidden users to hide the presence of user accounts they create or modify. Administrators may want to hide users when there are many user accounts on a given system or if they want... |
| [T1564.003](https://attack.mitre.org/techniques/T1564/003) | ↳ Hidden Window | Adversaries may use hidden windows to conceal malicious activity from the plain sight of users. In some cases, windows that would typically be displayed when an application carries out an operation... |
| [T1564.004](https://attack.mitre.org/techniques/T1564/004) | ↳ NTFS File Attributes | Adversaries may use NTFS file attributes to hide their malicious data in order to evade detection. Every New Technology File System (NTFS) formatted partition contains a Master File Table (MFT) that... |
| [T1564.005](https://attack.mitre.org/techniques/T1564/005) | ↳ Hidden File System | Adversaries may use a hidden file system to conceal malicious activity from users and security tools. File systems provide a structure to store and access data from physical storage. Typically, a... |
| [T1564.006](https://attack.mitre.org/techniques/T1564/006) | ↳ Run Virtual Instance | Adversaries may carry out malicious operations using a virtual instance to avoid detection. A wide variety of virtualization technologies exist that allow for the emulation of a computer or computing... |
| [T1564.007](https://attack.mitre.org/techniques/T1564/007) | ↳ VBA Stomping | Adversaries may hide malicious Visual Basic for Applications (VBA) payloads embedded within MS Office documents by replacing the VBA source code with benign data.(Citation: FireEye VBA stomp Feb... |
| [T1564.008](https://attack.mitre.org/techniques/T1564/008) | ↳ Email Hiding Rules | Adversaries may use email rules to hide inbound emails in a compromised user's mailbox. Many email clients allow users to create inbox rules for various email functions, including moving emails to... |
| [T1564.009](https://attack.mitre.org/techniques/T1564/009) | ↳ Resource Forking | Adversaries may abuse resource forks to hide malicious code or executables to evade detection and bypass security applications. A resource fork provides applications a structured way to store... |
| [T1564.010](https://attack.mitre.org/techniques/T1564/010) | ↳ Process Argument Spoofing | Adversaries may attempt to hide process command-line arguments by overwriting process memory. Process command-line arguments are stored in the process environment block (PEB), a data structure used... |
| [T1564.011](https://attack.mitre.org/techniques/T1564/011) | ↳ Ignore Process Interrupts | Adversaries may evade defensive mechanisms by executing commands that hide from process interrupt signals. Many operating systems use signals to deliver messages to control process behavior. Command... |
| [T1564.012](https://attack.mitre.org/techniques/T1564/012) | ↳ File/Path Exclusions | Adversaries may attempt to hide their file-based artifacts by writing them to specific folders or file names excluded from antivirus (AV) scanning and other defensive capabilities. AV and other... |
| [T1564.013](https://attack.mitre.org/techniques/T1564/013) | ↳ Bind Mounts | Adversaries may abuse bind mounts on file structures to hide their activity and artifacts from native utilities. A bind mount maps a directory or file from one location on the filesystem to another,... |
| [T1564.014](https://attack.mitre.org/techniques/T1564/014) | ↳ Extended Attributes | Adversaries may abuse extended attributes (xattrs) on macOS and Linux to hide their malicious data in order to evade detection. Extended attributes are key-value pairs of file and directory metadata... |
| [T1574](https://attack.mitre.org/techniques/T1574) | Hijack Execution Flow | Adversaries may execute their own malicious payloads by hijacking the way operating systems run programs. Hijacking execution flow can be for the purposes of persistence, since this hijacked... |
| [T1574.001](https://attack.mitre.org/techniques/T1574/001) | ↳ DLL | Adversaries may abuse dynamic-link library files (DLLs) in order to achieve persistence, escalate privileges, and evade defenses. DLLs are libraries that contain code and data that can be... |
| [T1574.004](https://attack.mitre.org/techniques/T1574/004) | ↳ Dylib Hijacking | Adversaries may execute their own payloads by placing a malicious dynamic library (dylib) with an expected name in a path a victim application searches at runtime. The dynamic loader will try to find... |
| [T1574.005](https://attack.mitre.org/techniques/T1574/005) | ↳ Executable Installer File Permissions Weakness | Adversaries may execute their own malicious payloads by hijacking the binaries used by an installer. These processes may automatically execute specific binaries as part of their functionality or to... |
| [T1574.006](https://attack.mitre.org/techniques/T1574/006) | ↳ Dynamic Linker Hijacking | Adversaries may execute their own malicious payloads by hijacking environment variables the dynamic linker uses to load shared libraries. During the execution preparation phase of a program, the... |
| [T1574.007](https://attack.mitre.org/techniques/T1574/007) | ↳ Path Interception by PATH Environment Variable | Adversaries may execute their own malicious payloads by hijacking environment variables used to load libraries. The PATH environment variable contains a list of directories (User and System) that the... |
| [T1574.008](https://attack.mitre.org/techniques/T1574/008) | ↳ Path Interception by Search Order Hijacking | Adversaries may execute their own malicious payloads by hijacking the search order used to load other programs. Because some programs do not call other programs using the full path, adversaries may... |
| [T1574.009](https://attack.mitre.org/techniques/T1574/009) | ↳ Path Interception by Unquoted Path | Adversaries may execute their own malicious payloads by hijacking vulnerable file path references. Adversaries can take advantage of paths that lack surrounding quotations by placing an executable in... |
| [T1574.010](https://attack.mitre.org/techniques/T1574/010) | ↳ Services File Permissions Weakness | Adversaries may execute their own malicious payloads by hijacking the binaries used by services. Adversaries may use flaws in the permissions of Windows services to replace the binary that is... |
| [T1574.011](https://attack.mitre.org/techniques/T1574/011) | ↳ Services Registry Permissions Weakness | Adversaries may execute their own malicious payloads by hijacking the Registry entries used by services. Flaws in the permissions for Registry keys related to services can allow adversaries to... |
| [T1574.012](https://attack.mitre.org/techniques/T1574/012) | ↳ COR_PROFILER | Adversaries may leverage the COR_PROFILER environment variable to hijack the execution flow of programs that load the .NET CLR. The COR_PROFILER is a .NET Framework feature which allows developers to... |
| [T1574.013](https://attack.mitre.org/techniques/T1574/013) | ↳ KernelCallbackTable | Adversaries may abuse the <code>KernelCallbackTable</code> of a process to hijack its execution flow in order to run their own payloads.(Citation: Lazarus APT January 2022)(Citation: FinFisher... |
| [T1574.014](https://attack.mitre.org/techniques/T1574/014) | ↳ AppDomainManager | Adversaries may execute their own malicious payloads by hijacking how the .NET `AppDomainManager` loads assemblies. The .NET framework uses the `AppDomainManager` class to create and manage one or... |
| [T1578](https://attack.mitre.org/techniques/T1578) | Modify Cloud Compute Infrastructure | An adversary may attempt to modify a cloud account's compute service infrastructure to evade defenses. A modification to the compute service infrastructure can include the creation, deletion, or... |
| [T1578.001](https://attack.mitre.org/techniques/T1578/001) | ↳ Create Snapshot | An adversary may create a snapshot or data backup within a cloud account to evade defenses. A snapshot is a point-in-time copy of an existing cloud compute component such as a virtual machine (VM),... |
| [T1578.002](https://attack.mitre.org/techniques/T1578/002) | ↳ Create Cloud Instance | An adversary may create a new instance or virtual machine (VM) within the compute service of a cloud account to evade defenses. Creating a new instance may allow an adversary to bypass firewall rules... |
| [T1578.003](https://attack.mitre.org/techniques/T1578/003) | ↳ Delete Cloud Instance | An adversary may delete a cloud instance after they have performed malicious activities in an attempt to evade detection and remove evidence of their presence. Deleting an instance or virtual machine... |
| [T1578.004](https://attack.mitre.org/techniques/T1578/004) | ↳ Revert Cloud Instance | An adversary may revert changes made to a cloud instance after they have performed malicious activities in attempt to evade detection and remove evidence of their presence. In highly virtualized... |
| [T1578.005](https://attack.mitre.org/techniques/T1578/005) | ↳ Modify Cloud Compute Configurations | Adversaries may modify settings that directly affect the size, locations, and resources available to cloud compute infrastructure in order to evade defenses. These settings may include service... |
| [T1599](https://attack.mitre.org/techniques/T1599) | Network Boundary Bridging | Adversaries may bridge network boundaries by compromising perimeter network devices or internal devices responsible for network segmentation. Breaching these devices may enable an adversary to bypass... |
| [T1599.001](https://attack.mitre.org/techniques/T1599/001) | ↳ Network Address Translation Traversal | Adversaries may bridge network boundaries by modifying a network device’s Network Address Translation (NAT) configuration. Malicious modifications to NAT may enable an adversary to bypass... |
| [T1600](https://attack.mitre.org/techniques/T1600) | Weaken Encryption | Adversaries may compromise a network device’s encryption capability in order to bypass encryption that would otherwise protect data communications. (Citation: Cisco Synful Knock Evolution) Encryption... |
| [T1600.001](https://attack.mitre.org/techniques/T1600/001) | ↳ Reduce Key Space | Adversaries may reduce the level of effort required to decrypt data transmitted over the network by reducing the cipher strength of encrypted communications.(Citation: Cisco Synful Knock Evolution)... |
| [T1600.002](https://attack.mitre.org/techniques/T1600/002) | ↳ Disable Crypto Hardware | Adversaries disable a network device’s dedicated hardware encryption, which may enable them to leverage weaknesses in software encryption in order to reduce the effort involved in collecting,... |
| [T1601](https://attack.mitre.org/techniques/T1601) | Modify System Image | Adversaries may make changes to the operating system of embedded network devices to weaken defenses and provide new capabilities for themselves. On such devices, the operating systems are typically... |
| [T1601.001](https://attack.mitre.org/techniques/T1601/001) | ↳ Patch System Image | Adversaries may modify the operating system of a network device to introduce new capabilities or weaken existing defenses.(Citation: Killing the myth of Cisco IOS rootkits) (Citation: Killing IOS... |
| [T1601.002](https://attack.mitre.org/techniques/T1601/002) | ↳ Downgrade System Image | Adversaries may install an older version of the operating system of a network device to weaken security. Older operating system versions on network devices often have weaker encryption ciphers and,... |
| [T1610](https://attack.mitre.org/techniques/T1610) | Deploy Container | Adversaries may deploy a container into an environment to facilitate execution or evade defenses. In some cases, adversaries may deploy a new container to execute processes associated with a... |
| [T1612](https://attack.mitre.org/techniques/T1612) | Build Image on Host | Adversaries may build a container image directly on a host to bypass defenses that monitor for the retrieval of malicious images from a public registry. A remote <code>build</code> request may be... |
| [T1620](https://attack.mitre.org/techniques/T1620) | Reflective Code Loading | Adversaries may reflectively load code into a process in order to conceal the execution of malicious payloads. Reflective loading involves allocating then executing payloads directly within the... |
| [T1622](https://attack.mitre.org/techniques/T1622) | Debugger Evasion | Adversaries may employ various means to detect and avoid debuggers. Debuggers are typically used by defenders to trace and/or analyze the execution of potential malware payloads.(Citation:... |
| [T1647](https://attack.mitre.org/techniques/T1647) | Plist File Modification | Adversaries may modify property list files (plist files) to enable other malicious activity, while also potentially evading and bypassing system defenses. macOS applications use plist files, such as... |
| [T1656](https://attack.mitre.org/techniques/T1656) | Impersonation | Adversaries may impersonate a trusted person or organization in order to persuade and trick a target into performing some action on their behalf. For example, adversaries may communicate with victims... |
| [T1666](https://attack.mitre.org/techniques/T1666) | Modify Cloud Resource Hierarchy | Adversaries may attempt to modify hierarchical structures in infrastructure-as-a-service (IaaS) environments in order to evade defenses. IaaS environments often group resources into a hierarchy,... |
| [T1672](https://attack.mitre.org/techniques/T1672) | Email Spoofing | Adversaries may fake, or spoof, a sender’s identity by modifying the value of relevant email headers in order to establish contact with victims under false pretenses.(Citation: Proofpoint TA427 April... |
| [T1678](https://attack.mitre.org/techniques/T1678) | Delay Execution | Adversaries may employ various time-based methods to evade detection and analysis. These techniques often exploit system clocks, delays, or timing mechanisms to obscure malicious activity, blend in... |
| [T1679](https://attack.mitre.org/techniques/T1679) | Selective Exclusion | Adversaries may intentionally exclude certain files, folders, directories, file types, or system components from encryption or tampering during a ransomware or malicious payload execution. Some file... |

---

### Credential Access

*67 techniques (17 parent, 50 sub-techniques)*

| T-Code | Name | Description |
|--------|------|-------------|
| [T1003](https://attack.mitre.org/techniques/T1003) | OS Credential Dumping | Adversaries may attempt to dump credentials to obtain account login and credential material, normally in the form of a hash or a clear text password. Credentials can be obtained from OS caches,... |
| [T1003.001](https://attack.mitre.org/techniques/T1003/001) | ↳ LSASS Memory | Adversaries may attempt to access credential material stored in the process memory of the Local Security Authority Subsystem Service (LSASS). After a user logs on, the system generates and stores a... |
| [T1003.002](https://attack.mitre.org/techniques/T1003/002) | ↳ Security Account Manager | Adversaries may attempt to extract credential material from the Security Account Manager (SAM) database either through in-memory techniques or through the Windows Registry where the SAM database is... |
| [T1003.003](https://attack.mitre.org/techniques/T1003/003) | ↳ NTDS | Adversaries may attempt to access or create a copy of the Active Directory domain database in order to steal credential information, as well as obtain other information about domain members such as... |
| [T1003.004](https://attack.mitre.org/techniques/T1003/004) | ↳ LSA Secrets | Adversaries with SYSTEM access to a host may attempt to access Local Security Authority (LSA) secrets, which can contain a variety of different credential materials, such as credentials for service... |
| [T1003.005](https://attack.mitre.org/techniques/T1003/005) | ↳ Cached Domain Credentials | Adversaries may attempt to access cached domain credentials used to allow authentication to occur in the event a domain controller is unavailable.(Citation: Microsoft - Cached Creds) On Windows Vista... |
| [T1003.006](https://attack.mitre.org/techniques/T1003/006) | ↳ DCSync | Adversaries may attempt to access credentials and other sensitive information by abusing a Windows Domain Controller's application programming interface (API)(Citation: Microsoft DRSR Dec 2017)... |
| [T1003.007](https://attack.mitre.org/techniques/T1003/007) | ↳ Proc Filesystem | Adversaries may gather credentials from the proc filesystem or `/proc`. The proc filesystem is a pseudo-filesystem used as an interface to kernel data structures for Linux based systems managing... |
| [T1003.008](https://attack.mitre.org/techniques/T1003/008) | ↳ /etc/passwd and /etc/shadow | Adversaries may attempt to dump the contents of <code>/etc/passwd</code> and <code>/etc/shadow</code> to enable offline password cracking. Most modern Linux operating systems use a combination of... |
| [T1040](https://attack.mitre.org/techniques/T1040) | Network Sniffing | Adversaries may passively sniff network traffic to capture information about an environment, including authentication material passed over the network. Network sniffing refers to using the network... |
| [T1056](https://attack.mitre.org/techniques/T1056) | Input Capture | Adversaries may use methods of capturing user input to obtain credentials or collect information. During normal system usage, users often provide credentials to various different locations, such as... |
| [T1056.001](https://attack.mitre.org/techniques/T1056/001) | ↳ Keylogging | Adversaries may log user keystrokes to intercept credentials as the user types them. Keylogging is likely to be used to acquire credentials for new access opportunities when [OS Credential... |
| [T1056.002](https://attack.mitre.org/techniques/T1056/002) | ↳ GUI Input Capture | Adversaries may mimic common operating system GUI components to prompt users for credentials with a seemingly legitimate prompt. When programs are executed that need additional privileges than are... |
| [T1056.003](https://attack.mitre.org/techniques/T1056/003) | ↳ Web Portal Capture | Adversaries may install code on externally facing portals, such as a VPN login page, to capture and transmit credentials of users who attempt to log into the service. For example, a compromised login... |
| [T1056.004](https://attack.mitre.org/techniques/T1056/004) | ↳ Credential API Hooking | Adversaries may hook into Windows application programming interface (API) functions and Linux system functions to collect user credentials. Malicious hooking mechanisms may capture API or function... |
| [T1110](https://attack.mitre.org/techniques/T1110) | Brute Force | Adversaries may use brute force techniques to gain access to accounts when passwords are unknown or when password hashes are obtained.(Citation: TrendMicro Pawn Storm Dec 2020) Without knowledge of... |
| [T1110.001](https://attack.mitre.org/techniques/T1110/001) | ↳ Password Guessing | Adversaries with no prior knowledge of legitimate credentials within the system or environment may guess passwords to attempt access to accounts. Without knowledge of the password for an account, an... |
| [T1110.002](https://attack.mitre.org/techniques/T1110/002) | ↳ Password Cracking | Adversaries may use password cracking to attempt to recover usable credentials, such as plaintext passwords, when credential material such as password hashes are obtained. [OS Credential... |
| [T1110.003](https://attack.mitre.org/techniques/T1110/003) | ↳ Password Spraying | Adversaries may use a single or small list of commonly used passwords against many different accounts to attempt to acquire valid account credentials. Password spraying uses one password (e.g.... |
| [T1110.004](https://attack.mitre.org/techniques/T1110/004) | ↳ Credential Stuffing | Adversaries may use credentials obtained from breach dumps of unrelated accounts to gain access to target accounts through credential overlap. Occasionally, large numbers of username and password... |
| [T1111](https://attack.mitre.org/techniques/T1111) | Multi-Factor Authentication Interception | Adversaries may target multi-factor authentication (MFA) mechanisms, (i.e., smart cards, token generators, etc.) to gain access to credentials that can be used to access systems, services, and... |
| [T1187](https://attack.mitre.org/techniques/T1187) | Forced Authentication | Adversaries may gather credential material by invoking or forcing a user to automatically provide authentication information through a mechanism in which they can intercept. The Server Message Block... |
| [T1212](https://attack.mitre.org/techniques/T1212) | Exploitation for Credential Access | Adversaries may exploit software vulnerabilities in an attempt to collect credentials. Exploitation of a software vulnerability occurs when an adversary takes advantage of a programming error in a... |
| [T1528](https://attack.mitre.org/techniques/T1528) | Steal Application Access Token | Adversaries can steal application access tokens as a means of acquiring credentials to access remote systems and resources. Application access tokens are used to make authorized API requests on... |
| [T1539](https://attack.mitre.org/techniques/T1539) | Steal Web Session Cookie | An adversary may steal web application or service session cookies and use them to gain access to web applications or Internet services as an authenticated user without needing credentials. Web... |
| [T1552](https://attack.mitre.org/techniques/T1552) | Unsecured Credentials | Adversaries may search compromised systems to find and obtain insecurely stored credentials. These credentials can be stored and/or misplaced in many locations on a system, including plaintext files... |
| [T1552.001](https://attack.mitre.org/techniques/T1552/001) | ↳ Credentials In Files | Adversaries may search local file systems and remote file shares for files containing insecurely stored credentials. These can be files created by users to store their own credentials, shared... |
| [T1552.002](https://attack.mitre.org/techniques/T1552/002) | ↳ Credentials in Registry | Adversaries may search the Registry on compromised systems for insecurely stored credentials. The Windows Registry stores configuration information that can be used by the system or other programs.... |
| [T1552.003](https://attack.mitre.org/techniques/T1552/003) | ↳ Shell History | Adversaries may search the command history on compromised systems for insecurely stored credentials. On Linux and macOS systems, shells such as Bash and Zsh keep track of the commands users type on... |
| [T1552.004](https://attack.mitre.org/techniques/T1552/004) | ↳ Private Keys | Adversaries may search for private key certificate files on compromised systems for insecurely stored credentials. Private cryptographic keys and certificates are used for authentication,... |
| [T1552.005](https://attack.mitre.org/techniques/T1552/005) | ↳ Cloud Instance Metadata API | Adversaries may attempt to access the Cloud Instance Metadata API to collect credentials and other sensitive data. Most cloud service providers support a Cloud Instance Metadata API which is a... |
| [T1552.006](https://attack.mitre.org/techniques/T1552/006) | ↳ Group Policy Preferences | Adversaries may attempt to find unsecured credentials in Group Policy Preferences (GPP). GPP are tools that allow administrators to create domain policies with embedded credentials. These policies... |
| [T1552.007](https://attack.mitre.org/techniques/T1552/007) | ↳ Container API | Adversaries may gather credentials via APIs within a containers environment. APIs in these environments, such as the Docker API and Kubernetes APIs, allow a user to remotely manage their container... |
| [T1552.008](https://attack.mitre.org/techniques/T1552/008) | ↳ Chat Messages | Adversaries may directly collect unsecured credentials stored or passed through user communication services. Credentials may be sent and stored in user chat communication applications such as email,... |
| [T1555](https://attack.mitre.org/techniques/T1555) | Credentials from Password Stores | Adversaries may search for common password storage locations to obtain user credentials.(Citation: F-Secure The Dukes) Passwords are stored in several places on a system, depending on the operating... |
| [T1555.001](https://attack.mitre.org/techniques/T1555/001) | ↳ Keychain | Adversaries may acquire credentials from Keychain. Keychain (or Keychain Services) is the macOS credential management system that stores account names, passwords, private keys, certificates,... |
| [T1555.002](https://attack.mitre.org/techniques/T1555/002) | ↳ Securityd Memory | An adversary with root access may gather credentials by reading `securityd`’s memory. `securityd` is a service/daemon responsible for implementing security protocols such as encryption and... |
| [T1555.003](https://attack.mitre.org/techniques/T1555/003) | ↳ Credentials from Web Browsers | Adversaries may acquire credentials from web browsers by reading files specific to the target browser.(Citation: Talos Olympic Destroyer 2018) Web browsers commonly save credentials such as website... |
| [T1555.004](https://attack.mitre.org/techniques/T1555/004) | ↳ Windows Credential Manager | Adversaries may acquire credentials from the Windows Credential Manager. The Credential Manager stores credentials for signing into websites, applications, and/or devices that request authentication... |
| [T1555.005](https://attack.mitre.org/techniques/T1555/005) | ↳ Password Managers | Adversaries may acquire user credentials from third-party password managers.(Citation: ise Password Manager February 2019) Password managers are applications designed to store user credentials,... |
| [T1555.006](https://attack.mitre.org/techniques/T1555/006) | ↳ Cloud Secrets Management Stores | Adversaries may acquire credentials from cloud-native secret management solutions such as AWS Secrets Manager, GCP Secret Manager, Azure Key Vault, and Terraform Vault. Secrets managers support the... |
| [T1556](https://attack.mitre.org/techniques/T1556) | Modify Authentication Process | Adversaries may modify authentication mechanisms and processes to access user credentials or enable otherwise unwarranted access to accounts. The authentication process is handled by mechanisms, such... |
| [T1556.001](https://attack.mitre.org/techniques/T1556/001) | ↳ Domain Controller Authentication | Adversaries may patch the authentication process on a domain controller to bypass the typical authentication mechanisms and enable access to accounts. Malware may be used to inject false credentials... |
| [T1556.002](https://attack.mitre.org/techniques/T1556/002) | ↳ Password Filter DLL | Adversaries may register malicious password filter dynamic link libraries (DLLs) into the authentication process to acquire user credentials as they are validated. Windows password filters are... |
| [T1556.003](https://attack.mitre.org/techniques/T1556/003) | ↳ Pluggable Authentication Modules | Adversaries may modify pluggable authentication modules (PAM) to access user credentials or enable otherwise unwarranted access to accounts. PAM is a modular system of configuration files, libraries,... |
| [T1556.004](https://attack.mitre.org/techniques/T1556/004) | ↳ Network Device Authentication | Adversaries may use [Patch System Image](https://attack.mitre.org/techniques/T1601/001) to hard code a password in the operating system, thus bypassing of native authentication mechanisms for local... |
| [T1556.005](https://attack.mitre.org/techniques/T1556/005) | ↳ Reversible Encryption | An adversary may abuse Active Directory authentication encryption properties to gain access to credentials on Windows systems. The <code>AllowReversiblePasswordEncryption</code> property specifies... |
| [T1556.006](https://attack.mitre.org/techniques/T1556/006) | ↳ Multi-Factor Authentication | Adversaries may disable or modify multi-factor authentication (MFA) mechanisms to enable persistent access to compromised accounts. Once adversaries have gained access to a network by either... |
| [T1556.007](https://attack.mitre.org/techniques/T1556/007) | ↳ Hybrid Identity | Adversaries may patch, modify, or otherwise backdoor cloud authentication processes that are tied to on-premises user identities in order to bypass typical authentication mechanisms, access... |
| [T1556.008](https://attack.mitre.org/techniques/T1556/008) | ↳ Network Provider DLL | Adversaries may register malicious network provider dynamic link libraries (DLLs) to capture cleartext user credentials during the authentication process. Network provider DLLs allow Windows to... |
| [T1556.009](https://attack.mitre.org/techniques/T1556/009) | ↳ Conditional Access Policies | Adversaries may disable or modify conditional access policies to enable persistent access to compromised accounts. Conditional access policies are additional verifications used by identity providers... |
| [T1557](https://attack.mitre.org/techniques/T1557) | Adversary-in-the-Middle | Adversaries may attempt to position themselves between two or more networked devices using an adversary-in-the-middle (AiTM) technique to support follow-on behaviors such as [Network... |
| [T1557.001](https://attack.mitre.org/techniques/T1557/001) | ↳ LLMNR/NBT-NS Poisoning and SMB Relay | By responding to LLMNR/NBT-NS network traffic, adversaries may spoof an authoritative source for name resolution to force communication with an adversary controlled system. This activity may be used... |
| [T1557.002](https://attack.mitre.org/techniques/T1557/002) | ↳ ARP Cache Poisoning | Adversaries may poison Address Resolution Protocol (ARP) caches to position themselves between the communication of two or more networked devices. This activity may be used to enable follow-on... |
| [T1557.003](https://attack.mitre.org/techniques/T1557/003) | ↳ DHCP Spoofing | Adversaries may redirect network traffic to adversary-owned systems by spoofing Dynamic Host Configuration Protocol (DHCP) traffic and acting as a malicious DHCP server on the victim network. By... |
| [T1557.004](https://attack.mitre.org/techniques/T1557/004) | ↳ Evil Twin | Adversaries may host seemingly genuine Wi-Fi access points to deceive users into connecting to malicious networks as a way of supporting follow-on behaviors such as [Network... |
| [T1558](https://attack.mitre.org/techniques/T1558) | Steal or Forge Kerberos Tickets | Adversaries may attempt to subvert Kerberos authentication by stealing or forging Kerberos tickets to enable [Pass the Ticket](https://attack.mitre.org/techniques/T1550/003). Kerberos is an... |
| [T1558.001](https://attack.mitre.org/techniques/T1558/001) | ↳ Golden Ticket | Adversaries who have the KRBTGT account password hash may forge Kerberos ticket-granting tickets (TGT), also known as a golden ticket.(Citation: AdSecurity Kerberos GT Aug 2015) Golden tickets enable... |
| [T1558.002](https://attack.mitre.org/techniques/T1558/002) | ↳ Silver Ticket | Adversaries who have the password hash of a target service account (e.g. SharePoint, MSSQL) may forge Kerberos ticket granting service (TGS) tickets, also known as silver tickets. Kerberos TGS... |
| [T1558.003](https://attack.mitre.org/techniques/T1558/003) | ↳ Kerberoasting | Adversaries may abuse a valid Kerberos ticket-granting ticket (TGT) or sniff network traffic to obtain a ticket-granting service (TGS) ticket that may be vulnerable to [Brute... |
| [T1558.004](https://attack.mitre.org/techniques/T1558/004) | ↳ AS-REP Roasting | Adversaries may reveal credentials of accounts that have disabled Kerberos preauthentication by [Password Cracking](https://attack.mitre.org/techniques/T1110/002) Kerberos messages.(Citation: Harmj0y... |
| [T1558.005](https://attack.mitre.org/techniques/T1558/005) | ↳ Ccache Files | Adversaries may attempt to steal Kerberos tickets stored in credential cache files (or ccache). These files are used for short term storage of a user's active session credentials. The ccache file is... |
| [T1606](https://attack.mitre.org/techniques/T1606) | Forge Web Credentials | Adversaries may forge credential materials that can be used to gain access to web applications or Internet services. Web applications and services (hosted in cloud SaaS environments or on-premise... |
| [T1606.001](https://attack.mitre.org/techniques/T1606/001) | ↳ Web Cookies | Adversaries may forge web cookies that can be used to gain access to web applications or Internet services. Web applications and services (hosted in cloud SaaS environments or on-premise servers)... |
| [T1606.002](https://attack.mitre.org/techniques/T1606/002) | ↳ SAML Tokens | An adversary may forge SAML tokens with any permissions claims and lifetimes if they possess a valid SAML token-signing certificate.(Citation: Microsoft SolarWinds Steps) The default lifetime of a... |
| [T1621](https://attack.mitre.org/techniques/T1621) | Multi-Factor Authentication Request Generation | Adversaries may attempt to bypass multi-factor authentication (MFA) mechanisms and gain access to accounts by generating MFA requests sent to users. Adversaries in possession of credentials to [Valid... |
| [T1649](https://attack.mitre.org/techniques/T1649) | Steal or Forge Authentication Certificates | Adversaries may steal or forge certificates used for authentication to access remote systems or resources. Digital certificates are often used to sign and encrypt messages and/or files. Certificates... |

---

### Discovery

*49 techniques (34 parent, 15 sub-techniques)*

| T-Code | Name | Description |
|--------|------|-------------|
| [T1007](https://attack.mitre.org/techniques/T1007) | System Service Discovery | Adversaries may try to gather information about registered local system services. Adversaries may obtain information about services using tools as well as OS utility commands such as <code>sc... |
| [T1010](https://attack.mitre.org/techniques/T1010) | Application Window Discovery | Adversaries may attempt to get a listing of open application windows. Window listings could convey information about how the system is used.(Citation: Prevailion DarkWatchman 2021) For example,... |
| [T1012](https://attack.mitre.org/techniques/T1012) | Query Registry | Adversaries may interact with the Windows Registry to gather information about the system, configuration, and installed software. The Registry contains a significant amount of information about the... |
| [T1016](https://attack.mitre.org/techniques/T1016) | System Network Configuration Discovery | Adversaries may look for details about the network configuration and settings, such as IP and/or MAC addresses, of systems they access or through information discovery of remote systems. Several... |
| [T1016.001](https://attack.mitre.org/techniques/T1016/001) | ↳ Internet Connection Discovery | Adversaries may check for Internet connectivity on compromised systems. This may be performed during automated discovery and can be accomplished in numerous ways such as using... |
| [T1016.002](https://attack.mitre.org/techniques/T1016/002) | ↳ Wi-Fi Discovery | Adversaries may search for information about Wi-Fi networks, such as network names and passwords, on compromised systems. Adversaries may use Wi-Fi information as part of [Account... |
| [T1018](https://attack.mitre.org/techniques/T1018) | Remote System Discovery | Adversaries may attempt to get a listing of other systems by IP address, hostname, or other logical identifier on a network that may be used for Lateral Movement from the current system.... |
| [T1033](https://attack.mitre.org/techniques/T1033) | System Owner/User Discovery | Adversaries may attempt to identify the primary user, currently logged in user, set of users that commonly uses a system, or whether a user is actively using the system. They may do this, for... |
| [T1040](https://attack.mitre.org/techniques/T1040) | Network Sniffing | Adversaries may passively sniff network traffic to capture information about an environment, including authentication material passed over the network. Network sniffing refers to using the network... |
| [T1046](https://attack.mitre.org/techniques/T1046) | Network Service Discovery | Adversaries may attempt to get a listing of services running on remote hosts and local network infrastructure devices, including those that may be vulnerable to remote software exploitation. Common... |
| [T1049](https://attack.mitre.org/techniques/T1049) | System Network Connections Discovery | Adversaries may attempt to get a listing of network connections to or from the compromised system they are currently accessing or from remote systems by querying for information over the network. An... |
| [T1057](https://attack.mitre.org/techniques/T1057) | Process Discovery | Adversaries may attempt to get information about running processes on a system. Information obtained could be used to gain an understanding of common software/applications running on systems within... |
| [T1069](https://attack.mitre.org/techniques/T1069) | Permission Groups Discovery | Adversaries may attempt to discover group and permission settings. This information can help adversaries determine which user accounts and groups are available, the membership of users in particular... |
| [T1069.001](https://attack.mitre.org/techniques/T1069/001) | ↳ Local Groups | Adversaries may attempt to find local system groups and permission settings. The knowledge of local system permission groups can help adversaries determine which groups exist and which users belong... |
| [T1069.002](https://attack.mitre.org/techniques/T1069/002) | ↳ Domain Groups | Adversaries may attempt to find domain-level groups and permission settings. The knowledge of domain-level permission groups can help adversaries determine which groups exist and which users belong... |
| [T1069.003](https://attack.mitre.org/techniques/T1069/003) | ↳ Cloud Groups | Adversaries may attempt to find cloud groups and permission settings. The knowledge of cloud permission groups can help adversaries determine the particular roles of users and groups within an... |
| [T1082](https://attack.mitre.org/techniques/T1082) | System Information Discovery | An adversary may attempt to get detailed information about the operating system and hardware, including version, patches, hotfixes, service packs, and architecture. Adversaries may use this... |
| [T1083](https://attack.mitre.org/techniques/T1083) | File and Directory Discovery | Adversaries may enumerate files and directories or may search in specific locations of a host or network share for certain information within a file system. Adversaries may use the information from... |
| [T1087](https://attack.mitre.org/techniques/T1087) | Account Discovery | Adversaries may attempt to get a listing of valid accounts, usernames, or email addresses on a system or within a compromised environment. This information can help adversaries determine which... |
| [T1087.001](https://attack.mitre.org/techniques/T1087/001) | ↳ Local Account | Adversaries may attempt to get a listing of local system accounts. This information can help adversaries determine which local accounts exist on a system to aid in follow-on behavior. Commands such... |
| [T1087.002](https://attack.mitre.org/techniques/T1087/002) | ↳ Domain Account | Adversaries may attempt to get a listing of domain accounts. This information can help adversaries determine which domain accounts exist to aid in follow-on behavior such as targeting specific... |
| [T1087.003](https://attack.mitre.org/techniques/T1087/003) | ↳ Email Account | Adversaries may attempt to get a listing of email addresses and accounts. Adversaries may try to dump Exchange address lists such as global address lists (GALs).(Citation: Microsoft Exchange Address... |
| [T1087.004](https://attack.mitre.org/techniques/T1087/004) | ↳ Cloud Account | Adversaries may attempt to get a listing of cloud accounts. Cloud accounts are those created and configured by an organization for use by users, remote support, services, or for administration of... |
| [T1120](https://attack.mitre.org/techniques/T1120) | Peripheral Device Discovery | Adversaries may attempt to gather information about attached peripheral devices and components connected to a computer system.(Citation: Peripheral Discovery Linux)(Citation: Peripheral Discovery... |
| [T1124](https://attack.mitre.org/techniques/T1124) | System Time Discovery | An adversary may gather the system time and/or time zone settings from a local or remote system. The system time is set and stored by services, such as the Windows Time Service on Windows or... |
| [T1135](https://attack.mitre.org/techniques/T1135) | Network Share Discovery | Adversaries may look for folders and drives shared on remote systems as a means of identifying sources of information to gather as a precursor for Collection and to identify potential systems of... |
| [T1201](https://attack.mitre.org/techniques/T1201) | Password Policy Discovery | Adversaries may attempt to access detailed information about the password policy used within an enterprise network or cloud environment. Password policies are a way to enforce complex passwords that... |
| [T1217](https://attack.mitre.org/techniques/T1217) | Browser Information Discovery | Adversaries may enumerate information about browsers to learn more about compromised environments. Data saved by browsers (such as bookmarks, accounts, and browsing history) may reveal a variety of... |
| [T1482](https://attack.mitre.org/techniques/T1482) | Domain Trust Discovery | Adversaries may attempt to gather information on domain trust relationships that may be used to identify lateral movement opportunities in Windows multi-domain/forest environments. Domain trusts... |
| [T1497](https://attack.mitre.org/techniques/T1497) | Virtualization/Sandbox Evasion | Adversaries may employ various means to detect and avoid virtualization and analysis environments. This may include changing behaviors based on the results of checks for the presence of artifacts... |
| [T1497.001](https://attack.mitre.org/techniques/T1497/001) | ↳ System Checks | Adversaries may employ various system checks to detect and avoid virtualization and analysis environments. This may include changing behaviors based on the results of checks for the presence of... |
| [T1497.002](https://attack.mitre.org/techniques/T1497/002) | ↳ User Activity Based Checks | Adversaries may employ various user activity checks to detect and avoid virtualization and analysis environments. This may include changing behaviors based on the results of checks for the presence... |
| [T1497.003](https://attack.mitre.org/techniques/T1497/003) | ↳ Time Based Checks | Adversaries may employ various time-based methods to detect virtualization and analysis environments, particularly those that attempt to manipulate time mechanisms to simulate longer elapses of time.... |
| [T1518](https://attack.mitre.org/techniques/T1518) | Software Discovery | Adversaries may attempt to get a listing of software and software versions that are installed on a system or in a cloud environment. Adversaries may use the information from [Software... |
| [T1518.001](https://attack.mitre.org/techniques/T1518/001) | ↳ Security Software Discovery | Adversaries may attempt to get a listing of security software, configurations, defensive tools, and sensors that are installed on a system or in a cloud environment. This may include things such as... |
| [T1518.002](https://attack.mitre.org/techniques/T1518/002) | ↳ Backup Software Discovery | Adversaries may attempt to get a listing of backup software or configurations that are installed on a system. Adversaries may use this information to shape follow-on behaviors, such as [Data... |
| [T1526](https://attack.mitre.org/techniques/T1526) | Cloud Service Discovery | An adversary may attempt to enumerate the cloud services running on a system after gaining access. These methods can differ from platform-as-a-service (PaaS), to infrastructure-as-a-service (IaaS),... |
| [T1538](https://attack.mitre.org/techniques/T1538) | Cloud Service Dashboard | An adversary may use a cloud service dashboard GUI with stolen credentials to gain useful information from an operational cloud environment, such as specific services, resources, and features. For... |
| [T1580](https://attack.mitre.org/techniques/T1580) | Cloud Infrastructure Discovery | An adversary may attempt to discover infrastructure and resources that are available within an infrastructure-as-a-service (IaaS) environment. This includes compute service resources such as... |
| [T1613](https://attack.mitre.org/techniques/T1613) | Container and Resource Discovery | Adversaries may attempt to discover containers and other resources that are available within a containers environment. Other resources may include images, deployments, pods, nodes, and other... |
| [T1614](https://attack.mitre.org/techniques/T1614) | System Location Discovery | Adversaries may gather information in an attempt to calculate the geographical location of a victim host. Adversaries may use the information from [System Location... |
| [T1614.001](https://attack.mitre.org/techniques/T1614/001) | ↳ System Language Discovery | Adversaries may attempt to gather information about the system language of a victim in order to infer the geographical location of that host. This information may be used to shape follow-on... |
| [T1615](https://attack.mitre.org/techniques/T1615) | Group Policy Discovery | Adversaries may gather information on Group Policy settings to identify paths for privilege escalation, security measures applied within a domain, and to discover patterns in domain objects that can... |
| [T1619](https://attack.mitre.org/techniques/T1619) | Cloud Storage Object Discovery | Adversaries may enumerate objects in cloud storage infrastructure. Adversaries may use this information during automated discovery to shape follow-on behaviors, including requesting all or specific... |
| [T1622](https://attack.mitre.org/techniques/T1622) | Debugger Evasion | Adversaries may employ various means to detect and avoid debuggers. Debuggers are typically used by defenders to trace and/or analyze the execution of potential malware payloads.(Citation:... |
| [T1652](https://attack.mitre.org/techniques/T1652) | Device Driver Discovery | Adversaries may attempt to enumerate local device drivers on a victim host. Information about device drivers may highlight various insights that shape follow-on behaviors, such as the... |
| [T1654](https://attack.mitre.org/techniques/T1654) | Log Enumeration | Adversaries may enumerate system and service logs to find useful data. These logs may highlight various types of valuable insights for an adversary, such as user authentication records ([Account... |
| [T1673](https://attack.mitre.org/techniques/T1673) | Virtual Machine Discovery | An adversary may attempt to enumerate running virtual machines (VMs) after gaining access to a host or hypervisor. For example, adversaries may enumerate a list of VMs on an ESXi hypervisor using a... |
| [T1680](https://attack.mitre.org/techniques/T1680) | Local Storage Discovery | Adversaries may enumerate local drives, disks, and/or volumes and their attributes like total or free space and volume serial number. This can be done to prepare for ransomware-related encryption, to... |

---

### Lateral Movement

*23 techniques (9 parent, 14 sub-techniques)*

| T-Code | Name | Description |
|--------|------|-------------|
| [T1021](https://attack.mitre.org/techniques/T1021) | Remote Services | Adversaries may use [Valid Accounts](https://attack.mitre.org/techniques/T1078) to log into a service that accepts remote connections, such as telnet, SSH, and VNC. The adversary may then perform... |
| [T1021.001](https://attack.mitre.org/techniques/T1021/001) | ↳ Remote Desktop Protocol | Adversaries may use [Valid Accounts](https://attack.mitre.org/techniques/T1078) to log into a computer using the Remote Desktop Protocol (RDP). The adversary may then perform actions as the logged-on... |
| [T1021.002](https://attack.mitre.org/techniques/T1021/002) | ↳ SMB/Windows Admin Shares | Adversaries may use [Valid Accounts](https://attack.mitre.org/techniques/T1078) to interact with a remote network share using Server Message Block (SMB). The adversary may then perform actions as the... |
| [T1021.003](https://attack.mitre.org/techniques/T1021/003) | ↳ Distributed Component Object Model | Adversaries may use [Valid Accounts](https://attack.mitre.org/techniques/T1078) to interact with remote machines by taking advantage of Distributed Component Object Model (DCOM). The adversary may... |
| [T1021.004](https://attack.mitre.org/techniques/T1021/004) | ↳ SSH | Adversaries may use [Valid Accounts](https://attack.mitre.org/techniques/T1078) to log into remote machines using Secure Shell (SSH). The adversary may then perform actions as the logged-on user. SSH... |
| [T1021.005](https://attack.mitre.org/techniques/T1021/005) | ↳ VNC | Adversaries may use [Valid Accounts](https://attack.mitre.org/techniques/T1078) to remotely control machines using Virtual Network Computing (VNC). VNC is a platform-independent desktop sharing... |
| [T1021.006](https://attack.mitre.org/techniques/T1021/006) | ↳ Windows Remote Management | Adversaries may use [Valid Accounts](https://attack.mitre.org/techniques/T1078) to interact with remote systems using Windows Remote Management (WinRM). The adversary may then perform actions as the... |
| [T1021.007](https://attack.mitre.org/techniques/T1021/007) | ↳ Cloud Services | Adversaries may log into accessible cloud services within a compromised environment using [Valid Accounts](https://attack.mitre.org/techniques/T1078) that are synchronized with or federated to... |
| [T1021.008](https://attack.mitre.org/techniques/T1021/008) | ↳ Direct Cloud VM Connections | Adversaries may leverage [Valid Accounts](https://attack.mitre.org/techniques/T1078) to log directly into accessible cloud hosted compute infrastructure through cloud native methods. Many cloud... |
| [T1072](https://attack.mitre.org/techniques/T1072) | Software Deployment Tools | Adversaries may gain access to and use centralized software suites installed within an enterprise to execute commands and move laterally through the network. Configuration management and software... |
| [T1080](https://attack.mitre.org/techniques/T1080) | Taint Shared Content | Adversaries may deliver payloads to remote systems by adding content to shared storage locations, such as network drives or internal code repositories. Content stored on network drives or in other... |
| [T1091](https://attack.mitre.org/techniques/T1091) | Replication Through Removable Media | Adversaries may move onto systems, possibly those on disconnected or air-gapped networks, by copying malware to removable media and taking advantage of Autorun features when the media is inserted... |
| [T1210](https://attack.mitre.org/techniques/T1210) | Exploitation of Remote Services | Adversaries may exploit remote services to gain unauthorized access to internal systems once inside of a network. Exploitation of a software vulnerability occurs when an adversary takes advantage of... |
| [T1534](https://attack.mitre.org/techniques/T1534) | Internal Spearphishing | After they already have access to accounts or systems within the environment, adversaries may use internal spearphishing to gain access to additional information or compromise other users within the... |
| [T1550](https://attack.mitre.org/techniques/T1550) | Use Alternate Authentication Material | Adversaries may use alternate authentication material, such as password hashes, Kerberos tickets, and application access tokens, in order to move laterally within an environment and bypass normal... |
| [T1550.001](https://attack.mitre.org/techniques/T1550/001) | ↳ Application Access Token | Adversaries may use stolen application access tokens to bypass the typical authentication process and access restricted accounts, information, or services on remote systems. These tokens are... |
| [T1550.002](https://attack.mitre.org/techniques/T1550/002) | ↳ Pass the Hash | Adversaries may “pass the hash” using stolen password hashes to move laterally within an environment, bypassing normal system access controls. Pass the hash (PtH) is a method of authenticating as a... |
| [T1550.003](https://attack.mitre.org/techniques/T1550/003) | ↳ Pass the Ticket | Adversaries may “pass the ticket” using stolen Kerberos tickets to move laterally within an environment, bypassing normal system access controls. Pass the ticket (PtT) is a method of authenticating... |
| [T1550.004](https://attack.mitre.org/techniques/T1550/004) | ↳ Web Session Cookie | Adversaries can use stolen session cookies to authenticate to web applications and services. This technique bypasses some multi-factor authentication protocols since the session is already... |
| [T1563](https://attack.mitre.org/techniques/T1563) | Remote Service Session Hijacking | Adversaries may take control of preexisting sessions with remote services to move laterally in an environment. Users may use valid credentials to log into a service specifically designed to accept... |
| [T1563.001](https://attack.mitre.org/techniques/T1563/001) | ↳ SSH Hijacking | Adversaries may hijack a legitimate user's SSH session to move laterally within an environment. Secure Shell (SSH) is a standard means of remote access on Linux and macOS systems. It allows a user to... |
| [T1563.002](https://attack.mitre.org/techniques/T1563/002) | ↳ RDP Hijacking | Adversaries may hijack a legitimate user’s remote desktop session to move laterally within an environment. Remote desktop is a common feature in operating systems. It allows a user to log into an... |
| [T1570](https://attack.mitre.org/techniques/T1570) | Lateral Tool Transfer | Adversaries may transfer tools or other files between systems in a compromised environment. Once brought into the victim environment (i.e., [Ingress Tool... |

---

### Collection

*41 techniques (17 parent, 24 sub-techniques)*

| T-Code | Name | Description |
|--------|------|-------------|
| [T1005](https://attack.mitre.org/techniques/T1005) | Data from Local System | Adversaries may search local system sources, such as file systems, configuration files, local databases, virtual machine files, or process memory, to find files of interest and sensitive data prior... |
| [T1025](https://attack.mitre.org/techniques/T1025) | Data from Removable Media | Adversaries may search connected removable media on computers they have compromised to find files of interest. Sensitive data can be collected from any removable media (optical disk drive, USB... |
| [T1039](https://attack.mitre.org/techniques/T1039) | Data from Network Shared Drive | Adversaries may search network shares on computers they have compromised to find files of interest. Sensitive data can be collected from remote systems via shared network drives (host shared... |
| [T1056](https://attack.mitre.org/techniques/T1056) | Input Capture | Adversaries may use methods of capturing user input to obtain credentials or collect information. During normal system usage, users often provide credentials to various different locations, such as... |
| [T1056.001](https://attack.mitre.org/techniques/T1056/001) | ↳ Keylogging | Adversaries may log user keystrokes to intercept credentials as the user types them. Keylogging is likely to be used to acquire credentials for new access opportunities when [OS Credential... |
| [T1056.002](https://attack.mitre.org/techniques/T1056/002) | ↳ GUI Input Capture | Adversaries may mimic common operating system GUI components to prompt users for credentials with a seemingly legitimate prompt. When programs are executed that need additional privileges than are... |
| [T1056.003](https://attack.mitre.org/techniques/T1056/003) | ↳ Web Portal Capture | Adversaries may install code on externally facing portals, such as a VPN login page, to capture and transmit credentials of users who attempt to log into the service. For example, a compromised login... |
| [T1056.004](https://attack.mitre.org/techniques/T1056/004) | ↳ Credential API Hooking | Adversaries may hook into Windows application programming interface (API) functions and Linux system functions to collect user credentials. Malicious hooking mechanisms may capture API or function... |
| [T1074](https://attack.mitre.org/techniques/T1074) | Data Staged | Adversaries may stage collected data in a central location or directory prior to Exfiltration. Data may be kept in separate files or combined into one file through techniques such as [Archive... |
| [T1074.001](https://attack.mitre.org/techniques/T1074/001) | ↳ Local Data Staging | Adversaries may stage collected data in a central location or directory on the local system prior to Exfiltration. Data may be kept in separate files or combined into one file through techniques such... |
| [T1074.002](https://attack.mitre.org/techniques/T1074/002) | ↳ Remote Data Staging | Adversaries may stage data collected from multiple systems in a central location or directory on one system prior to Exfiltration. Data may be kept in separate files or combined into one file through... |
| [T1113](https://attack.mitre.org/techniques/T1113) | Screen Capture | Adversaries may attempt to take screen captures of the desktop to gather information over the course of an operation. Screen capturing functionality may be included as a feature of a remote access... |
| [T1114](https://attack.mitre.org/techniques/T1114) | Email Collection | Adversaries may target user email to collect sensitive information. Emails may contain sensitive data, including trade secrets or personal information, that can prove valuable to adversaries. Emails... |
| [T1114.001](https://attack.mitre.org/techniques/T1114/001) | ↳ Local Email Collection | Adversaries may target user email on local systems to collect sensitive information. Files containing email data can be acquired from a user’s local system, such as Outlook storage or cache files.... |
| [T1114.002](https://attack.mitre.org/techniques/T1114/002) | ↳ Remote Email Collection | Adversaries may target an Exchange server, Office 365, or Google Workspace to collect sensitive information. Adversaries may leverage a user's credentials and interact directly with the Exchange... |
| [T1114.003](https://attack.mitre.org/techniques/T1114/003) | ↳ Email Forwarding Rule | Adversaries may setup email forwarding rules to collect sensitive information. Adversaries may abuse email forwarding rules to monitor the activities of a victim, steal information, and further gain... |
| [T1115](https://attack.mitre.org/techniques/T1115) | Clipboard Data | Adversaries may collect data stored in the clipboard from users copying information within or between applications. For example, on Windows adversaries can access clipboard data by using... |
| [T1119](https://attack.mitre.org/techniques/T1119) | Automated Collection | Once established within a system or network, an adversary may use automated techniques for collecting internal data. Methods for performing this technique could include use of a [Command and... |
| [T1123](https://attack.mitre.org/techniques/T1123) | Audio Capture | An adversary can leverage a computer's peripheral devices (e.g., microphones and webcams) or applications (e.g., voice and video call services) to capture audio recordings for the purpose of... |
| [T1125](https://attack.mitre.org/techniques/T1125) | Video Capture | An adversary can leverage a computer's peripheral devices (e.g., integrated cameras or webcams) or applications (e.g., video call services) to capture video recordings for the purpose of gathering... |
| [T1185](https://attack.mitre.org/techniques/T1185) | Browser Session Hijacking | Adversaries may take advantage of security vulnerabilities and inherent functionality in browser software to change content, modify user-behaviors, and intercept information as part of various... |
| [T1213](https://attack.mitre.org/techniques/T1213) | Data from Information Repositories | Adversaries may leverage information repositories to mine valuable information. Information repositories are tools that allow for storage of information, typically to facilitate collaboration or... |
| [T1213.001](https://attack.mitre.org/techniques/T1213/001) | ↳ Confluence | Adversaries may leverage Confluence repositories to mine valuable information. Often found in development environments alongside Atlassian JIRA, Confluence is generally used to store... |
| [T1213.002](https://attack.mitre.org/techniques/T1213/002) | ↳ Sharepoint | Adversaries may leverage the SharePoint repository as a source to mine valuable information. SharePoint will often contain useful information for an adversary to learn about the structure and... |
| [T1213.003](https://attack.mitre.org/techniques/T1213/003) | ↳ Code Repositories | Adversaries may leverage code repositories to collect valuable information. Code repositories are tools/services that store source code and automate software builds. They may be hosted internally or... |
| [T1213.004](https://attack.mitre.org/techniques/T1213/004) | ↳ Customer Relationship Management Software | Adversaries may leverage Customer Relationship Management (CRM) software to mine valuable information. CRM software is used to assist organizations in tracking and managing customer interactions, as... |
| [T1213.005](https://attack.mitre.org/techniques/T1213/005) | ↳ Messaging Applications | Adversaries may leverage chat and messaging applications, such as Microsoft Teams, Google Chat, and Slack, to mine valuable information. The following is a brief list of example information that may... |
| [T1213.006](https://attack.mitre.org/techniques/T1213/006) | ↳ Databases | Adversaries may leverage databases to mine valuable information. These databases may be hosted on-premises or in the cloud (both in platform-as-a-service and software-as-a-service environments).... |
| [T1530](https://attack.mitre.org/techniques/T1530) | Data from Cloud Storage | Adversaries may access data from cloud storage. Many IaaS providers offer solutions for online data object storage such as Amazon S3, Azure Storage, and Google Cloud Storage. Similarly, SaaS... |
| [T1557](https://attack.mitre.org/techniques/T1557) | Adversary-in-the-Middle | Adversaries may attempt to position themselves between two or more networked devices using an adversary-in-the-middle (AiTM) technique to support follow-on behaviors such as [Network... |
| [T1557.001](https://attack.mitre.org/techniques/T1557/001) | ↳ LLMNR/NBT-NS Poisoning and SMB Relay | By responding to LLMNR/NBT-NS network traffic, adversaries may spoof an authoritative source for name resolution to force communication with an adversary controlled system. This activity may be used... |
| [T1557.002](https://attack.mitre.org/techniques/T1557/002) | ↳ ARP Cache Poisoning | Adversaries may poison Address Resolution Protocol (ARP) caches to position themselves between the communication of two or more networked devices. This activity may be used to enable follow-on... |
| [T1557.003](https://attack.mitre.org/techniques/T1557/003) | ↳ DHCP Spoofing | Adversaries may redirect network traffic to adversary-owned systems by spoofing Dynamic Host Configuration Protocol (DHCP) traffic and acting as a malicious DHCP server on the victim network. By... |
| [T1557.004](https://attack.mitre.org/techniques/T1557/004) | ↳ Evil Twin | Adversaries may host seemingly genuine Wi-Fi access points to deceive users into connecting to malicious networks as a way of supporting follow-on behaviors such as [Network... |
| [T1560](https://attack.mitre.org/techniques/T1560) | Archive Collected Data | An adversary may compress and/or encrypt data that is collected prior to exfiltration. Compressing the data can help to obfuscate the collected data and minimize the amount of data sent over the... |
| [T1560.001](https://attack.mitre.org/techniques/T1560/001) | ↳ Archive via Utility | Adversaries may use utilities to compress and/or encrypt collected data prior to exfiltration. Many utilities include functionalities to compress, encrypt, or otherwise package data into a format... |
| [T1560.002](https://attack.mitre.org/techniques/T1560/002) | ↳ Archive via Library | An adversary may compress or encrypt data that is collected prior to exfiltration using 3rd party libraries. Many libraries exist that can archive data, including... |
| [T1560.003](https://attack.mitre.org/techniques/T1560/003) | ↳ Archive via Custom Method | An adversary may compress or encrypt data that is collected prior to exfiltration using a custom method. Adversaries may choose to use custom archival methods, such as encryption with XOR or stream... |
| [T1602](https://attack.mitre.org/techniques/T1602) | Data from Configuration Repository | Adversaries may collect data related to managed devices from configuration repositories. Configuration repositories are used by management systems in order to configure, manage, and control data on... |
| [T1602.001](https://attack.mitre.org/techniques/T1602/001) | ↳ SNMP (MIB Dump) | Adversaries may target the Management Information Base (MIB) to collect and/or mine valuable information in a network managed using Simple Network Management Protocol (SNMP). The MIB is a... |
| [T1602.002](https://attack.mitre.org/techniques/T1602/002) | ↳ Network Device Configuration Dump | Adversaries may access network configuration files to collect sensitive data about the device and the network. The network configuration is a file containing parameters that determine the operation... |

---

### Command And Control

*45 techniques (18 parent, 27 sub-techniques)*

| T-Code | Name | Description |
|--------|------|-------------|
| [T1001](https://attack.mitre.org/techniques/T1001) | Data Obfuscation | Adversaries may obfuscate command and control traffic to make it more difficult to detect.(Citation: Bitdefender FunnyDream Campaign November 2020) Command and control (C2) communications are hidden... |
| [T1001.001](https://attack.mitre.org/techniques/T1001/001) | ↳ Junk Data | Adversaries may add junk data to protocols used for command and control to make detection more difficult.(Citation: FireEye SUNBURST Backdoor December 2020) By adding random or meaningless data to... |
| [T1001.002](https://attack.mitre.org/techniques/T1001/002) | ↳ Steganography | Adversaries may use steganographic techniques to hide command and control traffic to make detection efforts more difficult. Steganographic techniques can be used to hide data in digital messages that... |
| [T1001.003](https://attack.mitre.org/techniques/T1001/003) | ↳ Protocol or Service Impersonation | Adversaries may impersonate legitimate protocols or web service traffic to disguise command and control activity and thwart analysis efforts. By impersonating legitimate protocols or web services,... |
| [T1008](https://attack.mitre.org/techniques/T1008) | Fallback Channels | Adversaries may use fallback or alternate communication channels if the primary channel is compromised or inaccessible in order to maintain reliable command and control and to avoid data transfer... |
| [T1071](https://attack.mitre.org/techniques/T1071) | Application Layer Protocol | Adversaries may communicate using OSI application layer protocols to avoid detection/network filtering by blending in with existing traffic. Commands to the remote system, and often the results of... |
| [T1071.001](https://attack.mitre.org/techniques/T1071/001) | ↳ Web Protocols | Adversaries may communicate using application layer protocols associated with web traffic to avoid detection/network filtering by blending in with existing traffic. Commands to the remote system, and... |
| [T1071.002](https://attack.mitre.org/techniques/T1071/002) | ↳ File Transfer Protocols | Adversaries may communicate using application layer protocols associated with transferring files to avoid detection/network filtering by blending in with existing traffic. Commands to the remote... |
| [T1071.003](https://attack.mitre.org/techniques/T1071/003) | ↳ Mail Protocols | Adversaries may communicate using application layer protocols associated with electronic mail delivery to avoid detection/network filtering by blending in with existing traffic. Commands to the... |
| [T1071.004](https://attack.mitre.org/techniques/T1071/004) | ↳ DNS | Adversaries may communicate using the Domain Name System (DNS) application layer protocol to avoid detection/network filtering by blending in with existing traffic. Commands to the remote system, and... |
| [T1071.005](https://attack.mitre.org/techniques/T1071/005) | ↳ Publish/Subscribe Protocols | Adversaries may communicate using publish/subscribe (pub/sub) application layer protocols to avoid detection/network filtering by blending in with existing traffic. Commands to the remote system, and... |
| [T1090](https://attack.mitre.org/techniques/T1090) | Proxy | Adversaries may use a connection proxy to direct network traffic between systems or act as an intermediary for network communications to a command and control server to avoid direct connections to... |
| [T1090.001](https://attack.mitre.org/techniques/T1090/001) | ↳ Internal Proxy | Adversaries may use an internal proxy to direct command and control traffic between two or more systems in a compromised environment. Many tools exist that enable traffic redirection through proxies... |
| [T1090.002](https://attack.mitre.org/techniques/T1090/002) | ↳ External Proxy | Adversaries may use an external proxy to act as an intermediary for network communications to a command and control server to avoid direct connections to their infrastructure. Many tools exist that... |
| [T1090.003](https://attack.mitre.org/techniques/T1090/003) | ↳ Multi-hop Proxy | Adversaries may chain together multiple proxies to disguise the source of malicious traffic. Typically, a defender will be able to identify the last proxy traffic traversed before it enters their... |
| [T1090.004](https://attack.mitre.org/techniques/T1090/004) | ↳ Domain Fronting | Adversaries may take advantage of routing schemes in Content Delivery Networks (CDNs) and other services which host multiple domains to obfuscate the intended destination of HTTPS traffic or traffic... |
| [T1092](https://attack.mitre.org/techniques/T1092) | Communication Through Removable Media | Adversaries can perform command and control between compromised hosts on potentially disconnected networks using removable media to transfer commands from system to system.(Citation: ESET Sednit... |
| [T1095](https://attack.mitre.org/techniques/T1095) | Non-Application Layer Protocol | Adversaries may use an OSI non-application layer protocol for communication between host and C2 server or among infected hosts within a network. The list of possible protocols is extensive.(Citation:... |
| [T1102](https://attack.mitre.org/techniques/T1102) | Web Service | Adversaries may use an existing, legitimate external Web service as a means for relaying data to/from a compromised system. Popular websites, cloud services, and social media acting as a mechanism... |
| [T1102.001](https://attack.mitre.org/techniques/T1102/001) | ↳ Dead Drop Resolver | Adversaries may use an existing, legitimate external Web service to host information that points to additional command and control (C2) infrastructure. Adversaries may post content, known as a dead... |
| [T1102.002](https://attack.mitre.org/techniques/T1102/002) | ↳ Bidirectional Communication | Adversaries may use an existing, legitimate external Web service as a means for sending commands to and receiving output from a compromised system over the Web service channel. Compromised systems... |
| [T1102.003](https://attack.mitre.org/techniques/T1102/003) | ↳ One-Way Communication | Adversaries may use an existing, legitimate external Web service as a means for sending commands to a compromised system without receiving return output over the Web service channel. Compromised... |
| [T1104](https://attack.mitre.org/techniques/T1104) | Multi-Stage Channels | Adversaries may create multiple stages for command and control that are employed under different conditions or for certain functions. Use of multiple stages may obfuscate the command and control... |
| [T1105](https://attack.mitre.org/techniques/T1105) | Ingress Tool Transfer | Adversaries may transfer tools or other files from an external system into a compromised environment. Tools or files may be copied from an external adversary-controlled system to the victim network... |
| [T1132](https://attack.mitre.org/techniques/T1132) | Data Encoding | Adversaries may encode data to make the content of command and control traffic more difficult to detect. Command and control (C2) information can be encoded using a standard data encoding system. Use... |
| [T1132.001](https://attack.mitre.org/techniques/T1132/001) | ↳ Standard Encoding | Adversaries may encode data with a standard data encoding system to make the content of command and control traffic more difficult to detect. Command and control (C2) information can be encoded using... |
| [T1132.002](https://attack.mitre.org/techniques/T1132/002) | ↳ Non-Standard Encoding | Adversaries may encode data with a non-standard data encoding system to make the content of command and control traffic more difficult to detect. Command and control (C2) information can be encoded... |
| [T1205](https://attack.mitre.org/techniques/T1205) | Traffic Signaling | Adversaries may use traffic signaling to hide open ports or other malicious functionality used for persistence or command and control. Traffic signaling involves the use of a magic value or sequence... |
| [T1205.001](https://attack.mitre.org/techniques/T1205/001) | ↳ Port Knocking | Adversaries may use port knocking to hide open ports used for persistence or command and control. To enable a port, an adversary sends a series of attempted connections to a predefined sequence of... |
| [T1205.002](https://attack.mitre.org/techniques/T1205/002) | ↳ Socket Filters | Adversaries may attach filters to a network socket to monitor then activate backdoors used for persistence or command and control. With elevated permissions, adversaries can use features such as the... |
| [T1219](https://attack.mitre.org/techniques/T1219) | Remote Access Tools | An adversary may use legitimate remote access tools to establish an interactive command and control channel within a network. Remote access tools create a session between two trusted hosts through a... |
| [T1219.001](https://attack.mitre.org/techniques/T1219/001) | ↳ IDE Tunneling | Adversaries may abuse Integrated Development Environment (IDE) software with remote development features to establish an interactive command and control channel on target systems within a network.... |
| [T1219.002](https://attack.mitre.org/techniques/T1219/002) | ↳ Remote Desktop Software | An adversary may use legitimate desktop support software to establish an interactive command and control channel to target systems within networks. Desktop support software provides a graphical... |
| [T1219.003](https://attack.mitre.org/techniques/T1219/003) | ↳ Remote Access Hardware | An adversary may use legitimate remote access hardware to establish an interactive command and control channel to target systems within networks. These services, including IP-based keyboard, video,... |
| [T1568](https://attack.mitre.org/techniques/T1568) | Dynamic Resolution | Adversaries may dynamically establish connections to command and control infrastructure to evade common detections and remediations. This may be achieved by using malware that shares a common... |
| [T1568.001](https://attack.mitre.org/techniques/T1568/001) | ↳ Fast Flux DNS | Adversaries may use Fast Flux DNS to hide a command and control channel behind an array of rapidly changing IP addresses linked to a single domain resolution. This technique uses a fully qualified... |
| [T1568.002](https://attack.mitre.org/techniques/T1568/002) | ↳ Domain Generation Algorithms | Adversaries may make use of Domain Generation Algorithms (DGAs) to dynamically identify a destination domain for command and control traffic rather than relying on a list of static IP addresses or... |
| [T1568.003](https://attack.mitre.org/techniques/T1568/003) | ↳ DNS Calculation | Adversaries may perform calculations on addresses returned in DNS results to determine which port and IP address to use for command and control, rather than relying on a predetermined port number or... |
| [T1571](https://attack.mitre.org/techniques/T1571) | Non-Standard Port | Adversaries may communicate using a protocol and port pairing that are typically not associated. For example, HTTPS over port 8088(Citation: Symantec Elfin Mar 2019) or port 587(Citation: Fortinet... |
| [T1572](https://attack.mitre.org/techniques/T1572) | Protocol Tunneling | Adversaries may tunnel network communications to and from a victim system within a separate protocol to avoid detection/network filtering and/or enable access to otherwise unreachable systems.... |
| [T1573](https://attack.mitre.org/techniques/T1573) | Encrypted Channel | Adversaries may employ an encryption algorithm to conceal command and control traffic rather than relying on any inherent protections provided by a communication protocol. Despite the use of a secure... |
| [T1573.001](https://attack.mitre.org/techniques/T1573/001) | ↳ Symmetric Cryptography | Adversaries may employ a known symmetric encryption algorithm to conceal command and control traffic rather than relying on any inherent protections provided by a communication protocol. Symmetric... |
| [T1573.002](https://attack.mitre.org/techniques/T1573/002) | ↳ Asymmetric Cryptography | Adversaries may employ a known asymmetric encryption algorithm to conceal command and control traffic rather than relying on any inherent protections provided by a communication protocol. Asymmetric... |
| [T1659](https://attack.mitre.org/techniques/T1659) | Content Injection | Adversaries may gain access and continuously communicate with victims by injecting malicious content into systems through online network traffic. Rather than luring victims to malicious payloads... |
| [T1665](https://attack.mitre.org/techniques/T1665) | Hide Infrastructure | Adversaries may manipulate network traffic in order to hide and evade detection of their C2 infrastructure. This can be accomplished by identifying and filtering traffic from defensive... |

---

### Exfiltration

*19 techniques (9 parent, 10 sub-techniques)*

| T-Code | Name | Description |
|--------|------|-------------|
| [T1011](https://attack.mitre.org/techniques/T1011) | Exfiltration Over Other Network Medium | Adversaries may attempt to exfiltrate data over a different network medium than the command and control channel. If the command and control network is a wired Internet connection, the exfiltration... |
| [T1011.001](https://attack.mitre.org/techniques/T1011/001) | ↳ Exfiltration Over Bluetooth | Adversaries may attempt to exfiltrate data over Bluetooth rather than the command and control channel. If the command and control network is a wired Internet connection, an adversary may opt to... |
| [T1020](https://attack.mitre.org/techniques/T1020) | Automated Exfiltration | Adversaries may exfiltrate data, such as sensitive documents, through the use of automated processing after being gathered during Collection.(Citation: ESET Gamaredon June 2020) When automated... |
| [T1020.001](https://attack.mitre.org/techniques/T1020/001) | ↳ Traffic Duplication | Adversaries may leverage traffic mirroring in order to automate data exfiltration over compromised infrastructure. Traffic mirroring is a native feature for some devices, often used for network... |
| [T1029](https://attack.mitre.org/techniques/T1029) | Scheduled Transfer | Adversaries may schedule data exfiltration to be performed only at certain times of day or at certain intervals. This could be done to blend traffic patterns with normal activity or availability.... |
| [T1030](https://attack.mitre.org/techniques/T1030) | Data Transfer Size Limits | An adversary may exfiltrate data in fixed size chunks instead of whole files or limit packet sizes below certain thresholds. This approach may be used to avoid triggering network data transfer... |
| [T1041](https://attack.mitre.org/techniques/T1041) | Exfiltration Over C2 Channel | Adversaries may steal data by exfiltrating it over an existing command and control channel. Stolen data is encoded into the normal communications channel using the same protocol as command and... |
| [T1048](https://attack.mitre.org/techniques/T1048) | Exfiltration Over Alternative Protocol | Adversaries may steal data by exfiltrating it over a different protocol than that of the existing command and control channel. The data may also be sent to an alternate network location from the main... |
| [T1048.001](https://attack.mitre.org/techniques/T1048/001) | ↳ Exfiltration Over Symmetric Encrypted Non-C2 Protocol | Adversaries may steal data by exfiltrating it over a symmetrically encrypted network protocol other than that of the existing command and control channel. The data may also be sent to an alternate... |
| [T1048.002](https://attack.mitre.org/techniques/T1048/002) | ↳ Exfiltration Over Asymmetric Encrypted Non-C2 Protocol | Adversaries may steal data by exfiltrating it over an asymmetrically encrypted network protocol other than that of the existing command and control channel. The data may also be sent to an alternate... |
| [T1048.003](https://attack.mitre.org/techniques/T1048/003) | ↳ Exfiltration Over Unencrypted Non-C2 Protocol | Adversaries may steal data by exfiltrating it over an un-encrypted network protocol other than that of the existing command and control channel. The data may also be sent to an alternate network... |
| [T1052](https://attack.mitre.org/techniques/T1052) | Exfiltration Over Physical Medium | Adversaries may attempt to exfiltrate data via a physical medium, such as a removable drive. In certain circumstances, such as an air-gapped network compromise, exfiltration could occur via a... |
| [T1052.001](https://attack.mitre.org/techniques/T1052/001) | ↳ Exfiltration over USB | Adversaries may attempt to exfiltrate data over a USB connected physical device. In certain circumstances, such as an air-gapped network compromise, exfiltration could occur via a USB device... |
| [T1537](https://attack.mitre.org/techniques/T1537) | Transfer Data to Cloud Account | Adversaries may exfiltrate data by transferring the data, including through sharing/syncing and creating backups of cloud environments, to another cloud account they control on the same service. A... |
| [T1567](https://attack.mitre.org/techniques/T1567) | Exfiltration Over Web Service | Adversaries may use an existing, legitimate external Web service to exfiltrate data rather than their primary command and control channel. Popular Web services acting as an exfiltration mechanism may... |
| [T1567.001](https://attack.mitre.org/techniques/T1567/001) | ↳ Exfiltration to Code Repository | Adversaries may exfiltrate data to a code repository rather than over their primary command and control channel. Code repositories are often accessible via an API (ex: https://api.github.com). Access... |
| [T1567.002](https://attack.mitre.org/techniques/T1567/002) | ↳ Exfiltration to Cloud Storage | Adversaries may exfiltrate data to a cloud storage service rather than over their primary command and control channel. Cloud storage services allow for the storage, edit, and retrieval of data from a... |
| [T1567.003](https://attack.mitre.org/techniques/T1567/003) | ↳ Exfiltration to Text Storage Sites | Adversaries may exfiltrate data to text storage sites instead of their primary command and control channel. Text storage sites, such as <code>pastebin[.]com</code>, are commonly used by developers to... |
| [T1567.004](https://attack.mitre.org/techniques/T1567/004) | ↳ Exfiltration Over Webhook | Adversaries may exfiltrate data to a webhook endpoint rather than over their primary command and control channel. Webhooks are simple mechanisms for allowing a server to push data over HTTP/S to a... |

---

### Impact

*33 techniques (15 parent, 18 sub-techniques)*

| T-Code | Name | Description |
|--------|------|-------------|
| [T1485](https://attack.mitre.org/techniques/T1485) | Data Destruction | Adversaries may destroy data and files on specific systems or in large numbers on a network to interrupt availability to systems, services, and network resources. Data destruction is likely to render... |
| [T1485.001](https://attack.mitre.org/techniques/T1485/001) | ↳ Lifecycle-Triggered Deletion | Adversaries may modify the lifecycle policies of a cloud storage bucket to destroy all objects stored within. Cloud storage buckets often allow users to set lifecycle policies to automate the... |
| [T1486](https://attack.mitre.org/techniques/T1486) | Data Encrypted for Impact | Adversaries may encrypt data on target systems or on large numbers of systems in a network to interrupt availability to system and network resources. They can attempt to render stored data... |
| [T1489](https://attack.mitre.org/techniques/T1489) | Service Stop | Adversaries may stop or disable services on a system to render those services unavailable to legitimate users. Stopping critical services or processes can inhibit or stop response to an incident or... |
| [T1490](https://attack.mitre.org/techniques/T1490) | Inhibit System Recovery | Adversaries may delete or remove built-in data and turn off services designed to aid in the recovery of a corrupted system to prevent recovery.(Citation: Talos Olympic Destroyer 2018)(Citation:... |
| [T1491](https://attack.mitre.org/techniques/T1491) | Defacement | Adversaries may modify visual content available internally or externally to an enterprise network, thus affecting the integrity of the original content. Reasons for... |
| [T1491.001](https://attack.mitre.org/techniques/T1491/001) | ↳ Internal Defacement | An adversary may deface systems internal to an organization in an attempt to intimidate or mislead users, thus discrediting the integrity of the systems. This may take the form of modifications to... |
| [T1491.002](https://attack.mitre.org/techniques/T1491/002) | ↳ External Defacement | An adversary may deface systems external to an organization in an attempt to deliver messaging, intimidate, or otherwise mislead an organization or users. [External... |
| [T1495](https://attack.mitre.org/techniques/T1495) | Firmware Corruption | Adversaries may overwrite or corrupt the flash memory contents of system BIOS or other firmware in devices attached to a system in order to render them inoperable or unable to boot, thus denying the... |
| [T1496](https://attack.mitre.org/techniques/T1496) | Resource Hijacking | Adversaries may leverage the resources of co-opted systems to complete resource-intensive tasks, which may impact system and/or hosted service availability. Resource hijacking may take a number of... |
| [T1496.001](https://attack.mitre.org/techniques/T1496/001) | ↳ Compute Hijacking | Adversaries may leverage the compute resources of co-opted systems to complete resource-intensive tasks, which may impact system and/or hosted service availability. One common purpose for [Compute... |
| [T1496.002](https://attack.mitre.org/techniques/T1496/002) | ↳ Bandwidth Hijacking | Adversaries may leverage the network bandwidth resources of co-opted systems to complete resource-intensive tasks, which may impact system and/or hosted service availability. Adversaries may also use... |
| [T1496.003](https://attack.mitre.org/techniques/T1496/003) | ↳ SMS Pumping | Adversaries may leverage messaging services for SMS pumping, which may impact system and/or hosted service availability.(Citation: Twilio SMS Pumping) SMS pumping is a type of telecommunications... |
| [T1496.004](https://attack.mitre.org/techniques/T1496/004) | ↳ Cloud Service Hijacking | Adversaries may leverage compromised software-as-a-service (SaaS) applications to complete resource-intensive tasks, which may impact hosted service availability. For example, adversaries may... |
| [T1498](https://attack.mitre.org/techniques/T1498) | Network Denial of Service | Adversaries may perform Network Denial of Service (DoS) attacks to degrade or block the availability of targeted resources to users. Network DoS can be performed by exhausting the network bandwidth... |
| [T1498.001](https://attack.mitre.org/techniques/T1498/001) | ↳ Direct Network Flood | Adversaries may attempt to cause a denial of service (DoS) by directly sending a high-volume of network traffic to a target. This DoS attack may also reduce the availability and functionality of the... |
| [T1498.002](https://attack.mitre.org/techniques/T1498/002) | ↳ Reflection Amplification | Adversaries may attempt to cause a denial of service (DoS) by reflecting a high-volume of network traffic to a target. This type of Network DoS takes advantage of a third-party server intermediary... |
| [T1499](https://attack.mitre.org/techniques/T1499) | Endpoint Denial of Service | Adversaries may perform Endpoint Denial of Service (DoS) attacks to degrade or block the availability of services to users. Endpoint DoS can be performed by exhausting the system resources those... |
| [T1499.001](https://attack.mitre.org/techniques/T1499/001) | ↳ OS Exhaustion Flood | Adversaries may launch a denial of service (DoS) attack targeting an endpoint's operating system (OS). A system's OS is responsible for managing the finite resources as well as preventing the entire... |
| [T1499.002](https://attack.mitre.org/techniques/T1499/002) | ↳ Service Exhaustion Flood | Adversaries may target the different network services provided by systems to conduct a denial of service (DoS). Adversaries often target the availability of DNS and web services, however others have... |
| [T1499.003](https://attack.mitre.org/techniques/T1499/003) | ↳ Application Exhaustion Flood | Adversaries may target resource intensive features of applications to cause a denial of service (DoS), denying availability to those applications. For example, specific features in web applications... |
| [T1499.004](https://attack.mitre.org/techniques/T1499/004) | ↳ Application or System Exploitation | Adversaries may exploit software vulnerabilities that can cause an application or system to crash and deny availability to users. (Citation: Sucuri BIND9 August 2015) Some systems may automatically... |
| [T1529](https://attack.mitre.org/techniques/T1529) | System Shutdown/Reboot | Adversaries may shutdown/reboot systems to interrupt access to, or aid in the destruction of, those systems. Operating systems may contain commands to initiate a shutdown/reboot of a machine or... |
| [T1531](https://attack.mitre.org/techniques/T1531) | Account Access Removal | Adversaries may interrupt availability of system and network resources by inhibiting access to accounts utilized by legitimate users. Accounts may be deleted, locked, or manipulated (ex: changed... |
| [T1561](https://attack.mitre.org/techniques/T1561) | Disk Wipe | Adversaries may wipe or corrupt raw disk data on specific systems or in large numbers in a network to interrupt availability to system and network resources. With direct write access to a disk,... |
| [T1561.001](https://attack.mitre.org/techniques/T1561/001) | ↳ Disk Content Wipe | Adversaries may erase the contents of storage devices on specific systems or in large numbers in a network to interrupt availability to system and network resources. Adversaries may partially or... |
| [T1561.002](https://attack.mitre.org/techniques/T1561/002) | ↳ Disk Structure Wipe | Adversaries may corrupt or wipe the disk data structures on a hard drive necessary to boot a system; targeting specific critical systems or in large numbers in a network to interrupt availability to... |
| [T1565](https://attack.mitre.org/techniques/T1565) | Data Manipulation | Adversaries may insert, delete, or manipulate data in order to influence external outcomes or hide activity, thus threatening the integrity of the data.(Citation: Sygnia Elephant Beetle Jan 2022) By... |
| [T1565.001](https://attack.mitre.org/techniques/T1565/001) | ↳ Stored Data Manipulation | Adversaries may insert, delete, or manipulate data at rest in order to influence external outcomes or hide activity, thus threatening the integrity of the data.(Citation: FireEye APT38 Oct... |
| [T1565.002](https://attack.mitre.org/techniques/T1565/002) | ↳ Transmitted Data Manipulation | Adversaries may alter data en route to storage or other systems in order to manipulate external outcomes or hide activity, thus threatening the integrity of the data.(Citation: FireEye APT38 Oct... |
| [T1565.003](https://attack.mitre.org/techniques/T1565/003) | ↳ Runtime Data Manipulation | Adversaries may modify systems in order to manipulate the data as it is accessed and displayed to an end user, thus threatening the integrity of the data.(Citation: FireEye APT38 Oct 2018)(Citation:... |
| [T1657](https://attack.mitre.org/techniques/T1657) | Financial Theft | Adversaries may steal monetary resources from targets through extortion, social engineering, technical theft, or other methods aimed at their own financial gain at the expense of the availability of... |
| [T1667](https://attack.mitre.org/techniques/T1667) | Email Bombing | Adversaries may flood targeted email addresses with an overwhelming volume of messages. This may bury legitimate emails in a flood of spam and disrupt business operations.(Citation:... |

---

*Data source: MITRE ATT&CK® Enterprise v2.0*

