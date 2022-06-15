# Domain 1 Notes

# Ethical Codes
Know all 4 tenants and the order of the ISC2 Code of Ethics
[ISC2 Code of Ethics](https://www.isc2.org/ethics)
- Protect society, the common good, necessary public trust, and confidence, and the infrastructure.
- Act honorable, honestly, justly, responsibly, and legally.
- Provide diligent and competent service to principals
- Advance and protect the profession
**PAPA** 

The first approach should be risk management

Security Governance should align and enable the business to achieve its goals.  Security needs to 
 - create value
 - enable the business

**Complexity is the worst enemy of security**

## CIA Triad

C - Confidentiality 

I - Integrity

A - Availability

Added by NIST
- Accountablility 
- Assurance

### Opposite of CIA
D - Disclosure

A - Alteration

D - Destruction

Also know [RFC 1087](https://datatracker.ietf.org/doc/html/rfc1087)
RFC1087 Characterizes unethical behavior as:
- seeks to gain unauthorized access to the resources of the internet
- disrupts the intended use of the Internet
- wastes resources (people, capacity, computer) though such actions,
- destroys the integrity of computer-based information,
- compromises the privacy of users

## Assets and threats
Asset- anything of value that can be compromised (physical, information, reputation)

Threat - any event or action that can potentially cause harm

Attack - Intentional act of attempting to bypass one or more security services

Vulnerability (or weakness) - condition that leaves the system and assets open to harm

Exploit - technique that takes advantage of an attack

Risk - likelihood of a threat occurring.  The cost of what the company will lose

Control - counter-measure that you put in place

When we talk about security, we talk about technical security, administration security, and physical security

Not all vulnerabilities have a threat.  When Identifying vulnerabilities, we need to id the threats

Incidents - when you have a security breach.  Policy Violations are an incident

Defense in depth:  Don't depend on one thing, multiple layers if one fails

Due Care - you were following the best standards.  Responsible. Did you make an effort?  Can you show you are making progress?

Due Diligence:  you did your research to make an informed decisions.  Proving Due Care.  ensuring behavior

 - You need to be aware of weakness and vulnerabilities (Due Diligence)
 - Need to take action to secure (Due Care)
 - **Due Diligence shows prudent executive leadership, due care shows judicious security operations**

Liability - who is responsible for damage

Least Privilege-only enough permissions to perform their job

Need to know-Even though someone has clearance, they do not get access to all items at that level

Privacy is only related to confidentiality


You need to know the laws and regulations to make informed decisions.  
- Consult with the Legal Department or a lawyer to determine how laws and regulations impact security operations
- Ignorance of the law is not an excuse. 
- Major Laws are HIPPA (for medical records privacy), GDPR (EU law regulating how personal data is handled).

You need to have Senior Management Support.  This is the most important item to get buy-in to security.
Always run a risk assessment.


PII once exposed may not be recoverable, can be used for extortion, fraud, identity theft


Sarbans-Oxley, HIPPA, require a code of ethics.  

Documentation:
- needed and required for security documentation.
- important to have a framework to your security

Most important document is to have one for information handling (per something I wrote down :-( )

# Types of Documents
- Policy:  high level statement of management intentions.  **Always Start With Policy.**
- Standard:  Required implementation or use of tools
- Procedure:  Step by step on how to do something
- Baseline:  Minimum security required for a system or process
- Guidelines:  Recommendations or suggestions.  This is the only one that is optional.  

Risk = Threats * Vulnerability or Risk = probability * impact

Qualifying Risk
1. Gather Asset Information, including logical assets, digital assets, and reputation
2. Identify the Vulnerabilities
3. Perform a Threat Assessment
4. Probability Quantification or how often does the threat happen
5. Probability Qualification.  This is not a solid number
6. Financial Impact Evaluation
7. Determine the proper counter measures or accept the risk

# Risk Management Principles

**Risk Cannot Be Eliminated**

- Mitigation of the risk
- Acceptance of the risk
- Transfer the risk - think insurance
- Avoid the risk

Asset Valuation
- Asset Management System
- Delphi Method - expert opinion and survey
- Insurance valuation
- Accounting System

Tangible and Untangle Assets go into Asset Valuation (AV)

Exposure Factor (EF) - a percentage of the amount of loss if a specific threat or vulnerability is exploited.

Risk = Threat * Vulnerability

Asset Value (AV)

Exposure Factor (EF)

Single-loss Expectancy (SLE)

Annual Rate of occurrence (ARO)

Annualized Loss Expectancy (ALE)

Total Cost of Ownership (TCO)

See Page 25 and 26 of 11th hour cissp on how to run the formula and a good example.  The Questions at the end of chapter 1 are great

A vulnerability can be real or theoretical.

- Perform Risk Analysis
- List Risk identified
- Determine Probability 
- Prioritize Risk

- Quantitative:  mathematical estimate, hard numbers.  
- Qualitative:  best guess, statements and valuations.  about impact, vulnerability, and threats.

Business Continuity Plan- Non technical.  Needs to be reviewed once a year.
Disaster Recovery Plan - Technical.  Not every business needs a disaster recovery plan.


NIST SP 800-34.  
1. Develop the Policy Statement
2. Conduct a business impact analysis (BIA)
3. Identify Preventative Controls
4. Develop REcovery Strategies
5. Develop an IT Contingency Plan
6. Plan for Testing, Training and Exercise
7. Plan for Maintenance.  

**People are the Most Important Asset**
- Ensure human health
- Maintain delivery to customers
- Provide a safe workplace.

Business Impact Analysis
- Most important doc in the Business Continuity Plan
- Lists the most important functions of the business
- Includes Estimates of Tolerable Downtime

- Maximum Tolerable Downtime (MTD):  Acceptable downtime.  This comes from Management (not the tech team)
- Recovery Time Objectives:  How long it takes to get back up.
- Recovery Point Objective:  Amount of time we need to take bak ups
- Mean Time to Failure:  Time between failure in any system (MTTF)
- Mean Time to Repair:  Average time to repair (MTTR)
- MTTF needs to be increased while MTTR needs to be decreased

## Business Continuity Plan Team's Responsibilities
- People Come First.  Needs to be in the BCP
- Review the BCP
- Plan needs to be tested
- **Everything needs a plan**

## Disaster Recovery Plan

Priority Levels
- Short Term - Mirroring site
- Mid Term - Rebuilding
- Long Term - Rebuilding

Determine type of backups
- Differential
- Incremental

Alternate Sites
- Hot Site(Mirrored):  Site that is fully equipped and synced.  
- Warm Site:  Does not have the data but has the equipment
- Cold Site:  Can be up in a week, needs hardware and data.
- Portable:  Think of a van with equipment
- Mutual Aid Agreement:  arrangement with another business to take over functions.  Also Called a reciprocal agreement

**When Restoring a Site, Critical Applications Should Come Online First**

Recovery Team:  Implements the procedures and controls when it comes to a disaster recovery process
 - Goal is to meet the Recovery Time Objective (RTO) without exceeding the Maximum Tolerable Downtime (MTD)

Salvage Team:  Team Responsible for restoring the original site

Employees can be a bigger threat than outside individuals.
- potential targets for social engineering
- need controls
- need to be aware of hiring and firing procedures

Data Owners determine need to know information for each job role
- not right to give your employees all access to everything
- need a list from the data owner of who can access what

- Recovery Controls:  Backups and Redundancy
- Compensating Controls:  For when an existing system can't meet requirements
- Detective Controls:  to be able to find out when something happens

Job Sensitive Profile:  What access is needed.  Administrators use this to assign permissions.

Employee Agreement.  Employees Should Sign:
- a NDA form
- Code of Conduct
- Ethics Agreement
- Conflict of Interests Agreement

Employee Policies
- Separation of Duties
- Need to Know 
- Least Privilege
- Job Rotation
- Mandatory Vacations (at Least 10 Days)
- Regular Password and Access Control Updates
- Frequent review of user privileges
- Need to know the work an employee is doing

Help Employee's Understand
- Risk
- Importance for company
- security policies

ISO 27001 - States people need to do regular security awareness training.

Termination Procedures:  
- Always terminate the account
- Give them just 15 minutes to get items
- You can have Friendly Terminations or Unfriendly Terminations

Determine important company functions

## Random Notes for Domain One

Configuration Management - know what has been changed and see what has been changed (Github, Auvik,)

Patch Management 

Clipping Levels - level of error to suspect something suspicious

Audit Events from time to time

**Unauthorized Access is a security violation**

Incident Response:  Proper Action to be taken in an incident

## Cyphers

Stream Based Cyphers:  Each digit is encrypted one at a time

Block-Based Cyphers:  Blocks of text

CBC:  Like block-based but uses an initialization vector

Information Security is not an IT Issue, its a business issue.  

Ultimately, its the board of directors who are responsible (or the top executive's)

Information Security should improve efficiency.  

Security needs to be allgined with the business goals
 - ask:  who, what why, when, where, how 
 - or ask why 6 times

**Everyone has a role in IT Security**

## Frameworks to know
**Don't build your own**

NIST 800-53

NIST Cyber Security Framework

CISSecurity Critical Security Controls v7.1

SSAE 18 SOC2

SOC3:  Light version of SOC2

### PCI 3.2.1 Major Requirement Categories
- Build and Maintaint a Secure Network and Systems
- Protect Cardholder Data
- Maintain a Vulnerability Management Program
- Impliment Storng Access Control Measures
- Regularly Monitor and Test Networks
- Mainaint an Information Security Policy

[Source](pcisecuritystandards.org)

## ISO Standards to Know
27002 - Guidelines for organizational security standards.  Includes selecting, implementation, and management of controls

27017 - controls applied to the provision and use of cloud storage

27018 - Protecting PII

27034-1 - Application Security

31000 - Risk Management

## NIST Risk Management Framework 
1. Prepare to execute the RMF
2. Categorize Information Systems 
3. Select Security Controls 
4. Implement Security Controls 
5. Assess Security Controls 
6. Authorize Information System (with senior management)
7. Monitor Security Controls 
