When the test talks about Logical Security, it is also talking about IT Security

Security needs to be considered during all phases of a project.

## Security Engineering Lifecycle
1. Initiation
2. Development/Acquire
3. Implementation
4. Operations/Maintenance
5. Disposal
6. Repeat back at 1

[NIST SP 800-14](https://csrc.nist.gov/publications/detail/sp/800-14/archive/1996-09-03) 

[NIST SP 800-160](https://csrc.nist.gov/publications/detail/sp/800-160/vol-1/final) **This is the one to know**

Security Foundations:  Establishes security policy as a design function

Risk Based:  Reduce Risk to acceptable levels, get a risk acceptance list.  assumes external systems as insecure

**Look for questions on what control is cost effective**

## Privacy by Design
1. Proactive approach
2. Default Setting
3. Embedded in Design
4. Positive Sum Approach:  Needs of everyone involved are met
5. End to End Security - Full life cycle protection
6. Visibility and Transparency 
7. Respect for User Privacy

Trusted Computer Base:  defined in Orange Book.  "a combination of hardware, software, and controls that work together to form a trusted base to enforce your security policy" (Sybex)

Trusted Computer Base Vulnerabilities
- Backdoors and Trapdoors
- Maintenance Hook:  Implemented for a good cause but misused.  Think Devs that create backdoors
- TOC/TOU:  attack that tries to get advantage from workstations to backend servers.  Manipulating data between the two
- Buffer Overflow:  manipulating memory
- Covert Channels:  traffic has been manipulated (man in the middle attack)

## Security Models:  You don't actually implement them, they are a concept.

- Bell-LaPradula:  Confidentiality.  **No Read Up, No Write Down**
- Biba:  Integrity.  **No Write Up, No Read Down**
- Clark-Wilson:  Integrity.  User uses a computer program to access data
- Brewer-Nash (aka Chinese Wall):  For conflict of interests.  Basically you build a wall between information.  Control will be taken based on decisions.

### TCSec
- Orange book is another name
- Created by the NIST, part of the rainbow books
- For evaluating a trusted computer base
- Goes from D (lowest) to A (highest) [Wikipedia](https://en.wikipedia.org/wiki/Trusted_Computer_System_Evaluation_Criteria)
  - D:  Minimal protection
  - C: Discretionary Protection
    - C1-identification and authentication
    - separation of users and data
    - Discretionary Access Control (DAC) capable of enforcing access
    - Required Security Docs and user manuals
    - C2- Controlled Access Protection
      - more finely grained DAC
      - Individual accountability though login procedures
      - Audit trails
      - object reuse
      - resource isolation
  - B:  Mandatory Protection
    - B1 - Labeled Security Protection
      - Informal statement of the security policy model
      - Data sensitive labels
      - Mandatory Access Control (MAC) over selected subjects and objects
      - Label exportation capabilities
      - Some discovered flaws must be removed or otherwise mitigated
      - Design specifications and verification
    - B2 - Structured Protection
      - Security policy model clearly defined and formally documented
      - DAC and MAC enforcement extended to all subjects and objects
      - Covert Storage channels are analyzed for occurrence and bandwidth
      - Carefully structured into protection-critical and non-protection-critical elements
      - Design and implementation enable more comprehensive testing and review
      - authentication mechanisms are strengthened
      - Trusted facility management is provided with administrator and operator segregation
      - Strict configuration management controls are imposed
      - Operator and Administrator roles are separated
    - B3 - Security Domains
      - Satisfies reference monitor requirements (enforces an access control policy over subjects ability to perform operations on objects on a system)
      - Structured to exclude code not essential to security policy enforcement
      - significant systems engineering directed toward minimizing complexity
      - Security administrator role defined
      - Audit security-relevant events
      - Automated imminent intrusion detection, notification, and response
      - Trusted path to the TCB for the user authentication function
      - Trusted system recover procedures
      - Convert timing channels are analyzed for occurrence and bandwidth
    - A - Verified protection
      - A1 - Verified Design
        - Functionally identical to B3
        - Formal design and verification techniques including a formal top-level specification
        - Formal management and distribution procedures
      - Beyond A1
        - System Architecture demonstrates that the requirements of self-protection and completeness for reference monitors have been implemented in the TCB
        - Security Testing automatically generates test-case from the formal top-level specification or formal lower-level specifications
        - Formal specification and verification is where the TCB is verified down to the source code level

### ITSec
- European standard similar to TCSec
- Evaluates functionality and assurance separetly
  - functionality is testing if a system can do something or not
  - assurance is testing if it does it all the time

[Common Criteria - ISO 15408](https://en.wikipedia.org/wiki/Common_Criteria)

- EAL0 - Inadequate assurance
- EAL1 - Functionally Tested
- EAL2 - Structurally tested
- EAL3 - Methodically tested and checked
- EAL4 - Methodically designed, tested, and reviewed
- EAL5 - Semi-formally designed and tested
- EAL6 - Semi formally verfied, designed, and tested
- EAL7 - Formally verified, desinged and tested.

Virtualization
- Convert to isolated systmes
- saves resources

Fault Tolerance
- Allows for quick recovery if a fault occures
- keep data separate from device, no single dependency
- ID your critical devices and have a redundant device
- id your critical data and have it redundant as well
- need to be based on MTD 

Server Fault Tolerance
- Clustering
- Network Load Balancing
- Virtualization
- Redundance and Replication

## Domain 3 Random Notes (probably from the Free Code Camp Video)

Never trust email or cell numbers

Constant training and education for yourself and your user base is always a great option.  

### Cryptography

Cryptography - Provides confidentiality and integrity

All encryption protocols should be public so we know how they work, the secret part is the key

The CISSP will **Never** suggest creating your own protocol

128bit = 2 power of 128

Cryptography takes processing power to work

Substitution - Changing the letters

Transposition - changing the location horizontally and veridically 

Steganography - hiding information in a picture.  Can be detected via  hex editor

Symmetric encryption - one key for encryption and decryption

Block cypher- divide plain text into blocks

stream cypher - one character or byte by byte

Initialization Vector - extra bytes to add randomization.  Gives you an extra so two plain text files will not give the same results.  Think Salt passwords.

Symmetric algorithm issues.  
- N(n-1)/2 where n is the number of users.  
- key management and transportation are issues
- it is easy to user

EEE3 - means text has been encrypted 3 times with 3 different keys

EDE - An encyrption key, then a decryption key.

asymmetric encryption
- Public/Private key encryption
- PGP, SSL/TLS, RSA, El-Gaamel, Ecclesiastes- provides confidentiality, integrity and non-repudiation
- you have to verify who you are to be issued a certificate

Hashing.  Eusing encyrption to verify the integrity of the files

Physical Security:  YOu may have a set of questions on what to use to fight fires (the proper fire suppression tools)

Data Centers
- know where to locate one (not in a basement)
- not on last floor, basement, under bathrooms
- should not have windows.

4 Levels of Protection
- deter
- detect
- delay
- respond

Physical Access Barriers 
- fencing 
- walls 
- doors (memorize the weakest types and strengths).
- windows
- lighting
- bollards

Fences:  Just deterance.  No fence will stop an intruder

Guards are the most expensive physical security

Logs should be kept for all access

**According to the ISC2, personal safety comes first and needs to be in all plans**

Power Issues

 - affect security devices and availability

Fire Suppression

- A:  Common, water, Soda, acid
- B: Liquids - Gas/C02, soda, acid
- C:  Electrical - Gas/C02
- D: Metal - Dry Powder

Fire extinguishers should be kept 50 feet from equipment and towards the door

Halon:  Not used anymore.  Replaced with MF200

Sprinklers
- Wet Pipe:  always contains water, melts at 165F, not good for cold environments
- Dry pipe:  water in tank until clapper valve opens
- Deluge: Spreads a huge amount of water.  Not good for electrical
 
