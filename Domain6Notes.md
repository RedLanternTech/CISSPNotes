Security Assessment and Testing

Need to test administrative and technical (logical) controls

Need to make sure it covers everything
- Management commitment
- Policy
- Administrative Controls
- technical

It cannot disturb the production environment

**Always have a plan for when doing testing**

May not test everything but identify systems that are critical

Always maintain the CIA Principal

Do not have a technical report.  Always translate reports to discuss risk

Method for creating the report
1. Collect Data
2. Store the data
3. Organize the Data
4. Analyze the data
5. Report on the data
6. Rank and define your vulnerabilities

Perform a Security Assessment when
- you first deploy new systems
- when new vulnerabilities are identified
- a security breach occurs
- routinely 

Fine-tune reports for Management.  
 - Nessus is a tool that can be used for vulnerability assessment
 - OpenVAS as well
 - OWASP Zap for Web applications

There are a variety of tools that do vulnerability scanning
- **don't use dark web tools at a professional level**
- Always use Professional tools

Penetration Testing
- simulates an attack
- less common but more intensive
- difference between a penetration test and a real attack is intent
- You must have a clearly defined scope before doing a penetration test

Reports from a Penetration Test Should include
- steps undertaken
- weaknesses identified
- recommendations

Penetration Testing Steps
1. Recon
2. Scanning
3. Exploitation
4. Maintaining Access 
5. Reporting

Types of Tests:
- Black Box:  you have no information about the target, most effective
- White Box:  you have all the information about the target
- Grey Box:  Balance between the two

### CMM - Capability Maturity Model 
1. Initial-Processes are unpredictable 
2. Managed - Processes characterized for the project are reactive
3. Define - Processes are proactive 
4. Quantitative - Processes are measured and controlled 
5. Optimized - Focus on process improvement
=======
## FR Secure notes

- Scope:  What are we testing and why.
 - You need to know what your boundaries are
- Assset Management is the key to good vulnerability scanning 
- Auditing, you have to pull information from everyone. 
- You need to have a Business Impact Analysis for your systems and the criticality of your systems when doing vulnerability testing
- CVSS scores do not take into account any compensating controls in your environment. 
- Think about increased traffic and a potential ddos.  Properly configure the scans.
- scans are idealy done durring low user activity.

## Pen Testing Steps from CISSP Book 
1. Planning
2. Recon
3. Scanning 
4. Vulnerability assessment 
5. Exploitation 
6. Reporting (Most Important Part.  Tells Owners how you owned the system, and recommended mitigation)

Read the PenTesters Framework for more information. 

**Make sure to always have your scope letter, even if you are doing digital pen testing**

- Pen Testers should Assure Confidentiality, Data Integrity, and System Integrity 
- When you are doing pen testing, someone should know about it or it could launch a full incident 

**assessing the effectiveness**

### Three Types of Controls
- Administrative 
- Physical 
- Technical 

## Software Testing Methods 
- Static testing:  looking within the code while its not running 
- Dynamic testing:  looking while its executing 
- Whitebox:  You get access to all the code 
- black box:  given no details
- traceability matrix: map customers requirements 
- Fuzzing:  just throw random stuff at the program 

Misuse Case Testing

Abuse Cases:  Looking to abuse system escalation privlidges, etc. 


