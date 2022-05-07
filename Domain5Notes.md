### How do you Define Security?
- use the security Triad (CIA)
- when you use it you can define

User/Subject and Resources/Object:  Subjects access an object

Subject -> Reference Monitor -> Object (The reference monitor will deny access by default)

Don't just consider technical security/logical security

### Access Control Services:
- Authorization
- Audit
- Accountability
- Identification

1. ID entity attempting access
2. Verify ID
3. Evaluate Rules
4. Log each access attempt
5. Review Logs

In CIA Triad
- Preventative
- Detective
- Corrective
- Directive

Windows uses Discretionary Access Control. Uses Access Control Lists for each object 

Mandatory Access Control:  Classifying your info.  Clearance level for each user (think Bell Lapuda or Biba)

Non-Discretionary Access Control:  Role-Based and Rule Based

Role-Based Access Control:  maps subjecs to objects based on the user's role in the organization.

Rule-Based Access Control:  Based on a list of predefined rules.

Identification Must be
- unique
- content dependent
- Time bound

Identification helps for accountability

Passwords are the cheapest to do but easiest to crack or bypass.
- Passwords need to come with policies for changing, creation, and storage 
- Pin numbers fall into this same category

### Three ways to identify someone
- Something you know (password)
- Something you have (security token)
- Something you are (biometrics)

### Identity Assurance Levels 
- IAL 1:  lowest leve, only requires user to self-assert an identity. 
- IAL 2:  Requires submission of identity documentation and proofing to the Credential Srvice Provider (CSP).  Frequently used in employment situations.
- IAL 3:  Requires physical presence and formal review.

Tokens:
- Synchronous  depends on timing
- Asynchronous:  depends on a math formula.  you type a number and it gives you one

Biometrics
- most expensive
- Need to look at the convergence of the False Reject Rate (type 1 error) and False accept rate(type 2 error).  False Accept is worse than a False Reject.  
- Crossover error rate is where the two meet. 
- See pages 122 and 123 of 11th Hour for the different types

### Single Sign On Methods
- Kerberos.  Uses a Key Distribution Server and a Ticket Granting Server
  - sends username only to the authentication server.  Server sends back text that can only be decrypted by the password
  - You do not send the password over the wire
- Tacacs and Tacacs2
- Federations:  trust between resources and account domains.  
  - uses pki 
  - think web sites for this one

### Attacking Software
- Denial of Service
- Buffer Overflows
- for Passwords, brute force and the use of rainbow tables

Brute Force is random letters, numbers, symbols being tried against a password.  Mitigated by complex passwords

Rainbow Tables.  Compares encryption hashes with other ones to find the password

Maintenance Hooks:  A Backdoor made for good use but is being abused

Buffer Overflows:  Manipulating memory

Human Based Attacks
 - most successful in the last few years
 - Guessing what the user may do or uses
 - shoulder surfing
 - dumpster diving
 - outright theft of something
 - social engineering (such as phishing attacks)

Intrusion Detection Systems
 - appliance or software
 - detects traffic in the network and will **notify you**.  It **will not** stop an attack.
 - Snort-is a major application for this (open source)
 - can be signature based or behavior based.  Behavior base builds a baseline and will ID issues after time

Network Based IDS will take info from capturing packets
Host Based takes info from logs 

Logical Security Layer is considered the technical domain

Penetration testing does not involve making any changes or modifications within a network.  Instead it involves determining what vulnerabilities exist so that changes can be made after the fact

Information Classification:  Practice of differentiating between types of information assets and providing some guidance as to how sensitive information will need to be protected.  

When Access Control is based on the content, it is considered content dependent access control

[NIST 800-145](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-145.pdf) defines deployment and definition of Cloud Computing.  

