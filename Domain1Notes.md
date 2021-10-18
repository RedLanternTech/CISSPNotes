# Domain 1 Notes

The first approach should be risk management

Security Governance should align and enable the business to achieve its goals.  Security needs to 
 - create value
 - enable the business

C - Confidentiality 

I - Integrity

A - Availability

Asset- anything of value that can be compromised (physical, information, reputation)

Threat - any event or action that can potentially cause harm

Attack - Intentional act of attempting to bypass one or more security services

Vulnerability (or weakness) - condition that leaves the system and assets open to harm

Exploit - technique that takes advantage of an attack

Risk - likelihood of a threat occurring.  The cost of what the company will lose

Control - counter-measure that you put in place

When we talk about security, we talk about technical security, administration security, and physical security

Not all vulnerabilities have a threat.  When Identifying vulnerabilities, we need to id the threats

Defense in depth:  Don't depend on one thing, multiple layers if one fails

Due Care - you were following the best standards.  Responsible.

Due Diligence:  you did your research to make an informed decisions.  Proving Due Care

 - YOu need to be aware of weakness and vulnerabilities (Due Diligence)
 - Need to take action to secure (Due Care)

Liability - who is responsible for damage

You need to know the laws and regulations to make informed decisions.  
- Consult with the Legal Department or a lawyer to determine how laws and regulations impact security operations
- Ignorance of the law is not an excuse. 
- Major Laws are HIPPA (for medical records privacy), GDPR (EU law regulating how personal data is handled).

You need to have Senior Management Support.  This is the most important item to get buy-in to security.
Always run a risk assessment.

PII once exposed may not be recoverable, can be used for extortion, fraud, identity theft

# Ethical Codes
Know all 4 tenants and the order of the ISC2 Code of Ethics
[ISC2 Code of Ethics](https://www.isc2.org/ethics)
- Protect society, the common good, necessary public trust, and confidence, and the infrastructure.
- Act honorable, honestly, justly, responsibly, and legally.
- Provide diligent and competent service to principals
- Advance and protect the profession

Also know [RFC 1087](https://datatracker.ietf.org/doc/html/rfc1087)
RFC1087 Characterizes unethical behavior as:
- seeks to gain unauthorized access to the resources of the internet
- disrupts the intended use of the Internet
- wastes resources (people, capacity, computer) though such actions,
- destroys the integrity of computer-based information,
- compromises the privacy of users

Sarbans-Oxley, HIPPA, require a code of ethics.  

Documentation:
- needed and required for security documentation.
- important to have a framework to your security

Most important document is to have one for information handling (per something I wrote down :-( )

# Types of Documents
- Policy:  high level statement of management intentions
- Standard:  REquired implementation or use of tools
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

Quantitative:  mathematical estimate, hard numbers.  
Qualitative:  best guess, statements and valuations.  about impact, vulnerability, and threats.

Business Continuity Plan- Non technical.  Needs to be reviewed once a year.
Disaster Recovery Plan - Technical.  Not every business needs a disaster recovery plan.


NIST SP 800-34.  
1. Develope the Policy Statement
2. Conduct a business impact analysis (BIA)
3. Identify Preventative Controls
4. Develope REcovery Strategies
5. Develope an IT Contingency Plan
6. Plan for Testing, Training and Exercise
7. PLan for Maintenance.  

**People are the Most Important Asset**
- Ensure human health
- Maintain delivery to customers
- Provide a safe workplace.

Business Impact Analysis
- Most important doc in the Business Continuity Plan
- Lists the most important functions of the business
- Includes Estimates of Tolerable Downtime

Maximum Tolerable Downtime (MTD):  Acceptable downtime.  This comes from Management (not the tech team)
Recovery Time Objectives:  How long it takes to get back up.
Recovery Point Objective:  Amount of time we need to take bak ups
Mean Time to Failure:  Time between failure in any system (MTTF)
Mean Time to Repair:  Average time to repair (MTTR)
MTTF needs to be increased while MTTR needs to be decreased

# Business Continuity Plan Team's Responsibilities
- People Come First.  Needs to be in the BCP
- Review the BCP
- Plan needs to be tested
- **Everything needs a plan**

