# 🔐 Mamba Ransomware Analysis Project

## 📋 Overview
Comprehensive reverse engineering and behavioral analysis of a sophisticated **Mamba (HDDCryptor) ransomware variant**. This project demonstrates professional malware analysis skills through static, dynamic, and API-level examination of real-world ransomware implementing full-disk encryption and network propagation capabilities.

## 🎯 Features

### 🔬 Technical Analysis
- **Static Analysis**: IDA Pro disassembly & pseudocode analysis
- **Dynamic Analysis**: Procmon, Procdot, Wireshark monitoring  
- **API-Level Analysis**: API Monitor instrumentation
- **Memory Analysis**: Process exploration during execution

### 🛡️ Security Insights
- **Evasion Techniques**: Service masquerading as "DefragmentService"
- **Propagation Methods**: Network share enumeration & scheduled tasks
- **Safety Mechanisms**: Conditional execution based on file checks
- **Persistence**: Windows service installation with auto-start

## 📊 Deliverables
- 📄 40+ page technical analysis report (industry standard)
- 🎥 5-minute API Monitor demonstration video
- 🖼️ 20+ annotated IDA Pro screenshots with pseudocode
- 📈 Dynamic behavior captures
- 🚨 Indicators of Compromise (IOCs)

## 🛠️ Tools Used
| Tool | Purpose |
|------|---------|
| IDA Pro | Static analysis & disassembly |
| API Monitor | API-level dynamic analysis |
| Procmon | System activity monitoring |
| Procdot | Process relationship visualization |
| Wireshark | Network traffic analysis |
| PEStudio | PE file analysis |
| VirtualBox | Safe execution environment |

## 🔍 Key Findings

### 1. Service Masquerading
Malware creates **"DefragmentService"** instead of obvious malicious names, mimicking legitimate Windows maintenance services.

### 2. Legitimate Tool Abuse  
Leverages **DiskCryptor encryption suite** (`dccon.exe`) rather than custom code.

### 3. Conditional Execution
Safety checks for `C:\DC22\netpass.txt` create branching execution paths.

### 4. Network Propagation
Lateral movement via scheduled tasks and administrative account creation.

### 5. Password-Protected Execution
Requires command-line password argument with immediate termination if not provided.

## 🚀 Quick Start
1. **Review** `analysis-report/cyb633-final-report.pdf`
2. **Watch** `video-demo/api-monitor-demo.mp4` (5 min)
3. **Browse** `screenshots/` for technical evidence
4. **Check** `iocs/` for security outputs

## 📈 Methodology
1. **Static Analysis**: PE examination, IDA disassembly, string extraction
2. **Dynamic Analysis**: Controlled VM execution with monitoring tools  
3. **Correlation**: Cross-validation of static predictions with dynamic observations

## 🎥 Video Demo
5-minute API Monitor demonstration showing:
- Tool configuration for malware analysis
- Real-time API call capture during execution  
- Parameter inspection of critical functions
- Comparison with static analysis predictions

## ⚠️ Safety & Ethics
**Important**: Analysis conducted in controlled, isolated lab environment:
- Air-gapped virtual machines
- Regular snapshot restoration  
- No production network connectivity
- Responsible disclosure considerations

**Warning**: Malware sample **not included** - contains analysis results only.

## 💼 Skills Demonstrated
- **Reverse Engineering**: Assembly analysis, Windows API comprehension
- **Dynamic Analysis**: Process monitoring, API hooking, network analysis  
- **Security Operations**: IOC generation, detection rule creation
- **Technical Communication**: Professional reporting, evidence presentation
- **Research Methodology**: Systematic analysis, evidence correlation

## 📞 Contact
For questions about methodology or cybersecurity opportunities:

**Stanford Junior Takura Zhuwao**  
sjnrzhuwao@gmail.com 
[Portfolio]

---

**Tags**: `#malware-analysis` `#reverse-engineering` `#ransomware` `#cybersecurity`

**Perfect For**: Cybersecurity Analyst, Malware Researcher, Incident Responder, SOC Analyst

---

*Academic project completed for CYB 633 Malware Analysis. Analysis conducted December 2025.*

