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

[NIST SP 800-27](https://csrc.nist.gov/publications/detail/sp/800-27/rev-a/archive/2004-06-21) **This is the one to know**

Security Foundations:  Establishes security policy as a design function

Risk Based:  Reduce Risk to acceptable levels, get a risk acceptance list.  assumes external systems as insecure

Look for questions on what control is cost effective

Trusted Computer Base:  defined in Orange Book.  "a combination of hardware, software, and controls that work together to form a trusted base to enforce your security policy" (Sybex)

Trusted Computer Base Vulnerabilities
- Backdoors and Trapdoors
- Maintenance Hook:  Implemented for a good cause but misused.  Think Devs that create backdoors
- TOC/TOU:  attack that tries to get advantage from workstations to backend servers.  Manipulating data between the two
- Buffer Overflow:  manipulating memory
- Covert Channels:  traffic has been manipulated (man in the middle attack)

## Security Models:  You don't actually implement them, they are a concept.

Bell-LaPradula:  Confidentiality.  **No Read Up, No Write Down**
Biba:  Integrity.  **No Write Up, No Read Down**
Clark-Wilson:  Integrity.  User uses a computer program to access data
Brewer-Nash (aka Chinese Wall):  For conflict of interests.  Basically you build a wall between information.  Control will be taken based on decisions.