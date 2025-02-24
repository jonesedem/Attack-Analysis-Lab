# Attack-Analysis-Lab
 This project focuses on investigating malicious activity using the ANY.RUN online malware hunting service and the Mitre ATT&CK Matrix.

## Objective:
This project focuses on investigating malicious activity using the ANY.RUN online malware hunting service and the Mitre ATT&CK Matrix.

## Tools:
- **ANY.RUN**: An interactive malware sandbox for dynamic analysis.
- **Mitre ATT&CK Matrix**: A knowledge base of adversary tactics and techniques.

## Lab Breakdown:
1. **Part 1:** Investigate Indicators of Compromise (IOCs) using ANY.RUN.
2. **Part 2:** Analyze malicious activities and determine tactics and techniques using Mitre ATT&CK.
3. **Part 3:** Examine additional malicious activities and their associated dangers.

## How to Use:
Each part is separated detailing each phase of the lab analysis.

## License:
This project is for educational purposes only.

# Part 1: Investigate IOCs
### The table below contains the list of the IOCs (hash values) and the analysis results (whether they are malicious, suspicious, or benign).

## Hash Analysis Results:

| MD5 Hash                                 | Malicious / Suspicious / Benign | Associated Filename |
|------------------------------------------|---------------------------------|---------------------|
| 2fd03624e271ec70349ce56fb30f563b        | Malicious                       | wireframe.exe       |
| c419df63e0121d72411285780c2fc6cc        | Suspicious                      | Updreg.EXE          |
| 3acf52e5a62d50bdcedcb89174bf5492        | Benign                          | BACs_Payment2847.html |
| 766b774626947000e67e0b318f558e94        | Malicious                       | gh2st.exe           |
| 422a6ca28a7e4d8e5e498523c6f049f4        | Malicious                       | file1.exe           |
| b497845beb135740e6caed03a2020036        | Suspicious                      | winlogon.exe        |

# Part 2: Investigate the Malicious Activity
### This part includes the details of the investigation process for the malicious activity using the ANY.RUN sandbox. It includes the process tree, reports, and relevant findings. 

### First Malicious Activity: wireframe.exe

### Process Tree:
- **wireframe.exe**
- **cmd.exe**
- **timeout.exe**
- **NvidiaGPU.exe**

### SHA256 Value: 
9C83A89EA0E56D5AF9AA37D2DABED20B2412DB8C9694A13128EA173A73557487

### Identified Danger:
ASYNCRAT detected.

## ATT&CK Matrix:
- **Malicious Activities Detected:** 4 tactics, 5 techniques, and 16 events are related to this malicious activity
- **Tactics:** Execution, Persistence, Privilege Escalation, Discovery
- **Techniques:** Boot or Logon Autostart Execution

# Part 3: Investigate the More Malicious Activity

### This part contains a detailed report of the second malicious hash analysis, including process trees, report details, and ATT&CK matrix analysis.

### Second Malicious Activity: gh2st.exe

### Process Tree:
- **gh2st.exe**
- **cmd.exe**

### SHA256 Value: 
88DD2037D0C43ABACEBAD866DF3F8CCD2EE7D64B01405AA6756A3A1C2FAC28FA

### Identified Dangers:
- Steals credentials from Web Browsers
- Connects to CnC server
- REDLINE detected

## ATT&CK Matrix:
- **Malicious Activities Detected:** 3 tactics, 7 techniques, and 245 events are related to this malicious activity
- **Tactics:** Credential access, Discovery, and Collection
- **Techniques:** Credential from Password Stores, Unsecured Credentials, Software Discovery, and Email Collection
## Second Malicious Activity: file1.exe

### Process Tree:
- **file1.exe**

### SHA256 Value: 
F7B1639B6C4CA677BA279B945A94C5F6D67E6C4C89FD39CD8BE882A8A7CDFCAA

### Identified Dangers:
- Steals credentials from Web Browsers
- Connects to CnC server
- REDLINE detected

## ATT&CK Matrix:
- **Malicious Activities Detected:** 3 tactics, 7 techniques, and 1525 events are related to this malicious activity
- **Tactics:** Credential access, Discovery, and Collection
    
# Reflection Questions

1. **Explain how forensic analysis and incident response is very much like law enforcement trying to solve a criminal case.**

- Similar to police detectives, forensic analysts must collect evidence, validate incidents, and analyze them to identify criminals or malicious actors.

2. **What is Redline?**
   
- RedLine Stealer is a malware that collects sensitive data such as passwords, credit card details, and other personal information from browsers and infected systems.

### Screenshots

<p align="center">
<img src="https://imgur.com/PKuzKIE.png" height="85%" width="85%" alt="Malicious Activity Investigation"/>
</p>
<p align="center">
<img src="https://imgur.com/uYUqamB.png" height="85%" width="85%" alt="Malicious Activity Investigation"/>
</p>
<p align="center">
<img src="https://imgur.com/NY7ii6D.png" height="85%" width="85%" alt="Malicious Activity Investigation"/>
</p>
<p align="center">
<img src="https://imgur.com/4zWDQa5.png" height="85%" width="85%" alt="Malicious Activity Investigation"/>
</p>
<p align="center">
<img src="https://imgur.com/6n1yq5P.png" height="85%" width="85%" alt="Malicious Activity Investigation"/>
</p>

### Resources
<div>
    <img src="https://img.shields.io/badge/-ANY.RUN_Sandbox-00599C?&style=for-the-badge&logo=AnyRun&logoColor=white" />
<img src="https://img.shields.io/badge/-Mitre_ATT&CK_Matrix-242424?&style=for-the-badge&logo=MITRE&logoColor=white" />
</div>

