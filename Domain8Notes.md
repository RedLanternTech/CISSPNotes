### System Life Cycle
0. Project Initiation
1. System Concept
2. Planning
3. Requiring Analysis
4. System Design
5. Software Development
6. Integration and Testing
7. Implementation 
8. Operational/Maintenance
9. Disposal

Two Types of Software Design Concepts- Proprietary and Open Source

Types of Disclosure:  Full or Partial

## Software Development Methods
### Waterfall
- Sequential
- Define -> ->Estimating -> Creating -> Testing -> Operation
- When you complete a phase, you start the next one
- you don't go back
- When you finish a phase you don't go back
- This has fallen out of favor in many organizations.  Upside is it has strict control of the process.  

### Sashimi
- Runs in parallel
- All phases run in parallel
- Effective but security becomes a concern

Spiral
- PLan
- Do
- Check
- Act
- This is a quality model
- it is a continuous process

Clean Room
- prevents changes
- Needs more time at the beginning to reduce change

Prototyping
- making samples

Agile
- project management model
- customer is involved in the process
- 12 principles that make it up. 
- not a methodology but a set of ideas.  
- Highest priority is to satisfy the customer though early and continuous deliver.  Get them something useful early in development.  
- Majority of software development is being done this way 
- each iteration has a lesson's learned component. 

Case or Computer Aid Software Engineering
- software helps develop the software

Change Control 
- need to have a proper change request
- request change
- approval
- communicating the change
- documenting the change 
- test and repeat
- implement the change
- report the change

When it comes to web forms (or any type of input), **Always Validate The Input**
- this is true to prevent SQL injection attacks on web forms

Integrity of data in software is needed
- database integrity
- entity integrity
- referential integrity

## FR Secure Start 

- Initiation 
- Development 
- Deployment and Delivery 
- Operations and maintenance 
- Disposal

## DevOps - is the result of siloes.  
- keeps different departments from killing each other. 
- Combine Development and Operations 
- still respects separation of duties, but Development and Operations works together 
- quality is built in and we are all playing for the same team 
- All three groups work together.  

- have a lot of controls around devops.  Important to have good logging and access control.
- will need additional security controls 
- make sure you are enforcing least privlige and separation of duties.  Temporal permissins is important 

## DevSecOps 
- gets security involved 
- Leaning in - over always saying "no".  Be the department of how 
- Use data security science over fear 
- Open contribution & collaboration over security requiements 
- consumable security services with APIs over Mandated Security Control & Paperwork 
- Business Driven Security scores over Rubber stamp security 
- Red & Blue Team Exploit Testing 
- 24/7 Proactive Security Monitoring 
- Shared threat Intelligence 
- Compliance Operations 
- Iteration over Perfection 

- The CISSP will be in the Red Team 

## Maturity Models 
- CMM is the most common.  Use the best practice across successful projects .
- matured into the CMMI run by ISACA 
- initial
- Managed
- Defined
- Quantitatively managed
- Optimizing

### SAMM 
- baking security proccess into an existing SDLC 

- The Theme:  What are we going to do, what is the plan, what are we designing, how do we make it, how do we get it into an operational state 

Change control will trigger a review for potential security impacts

- Includes a Change Management Board 

## Flow of Change Management 
- request
- Analysis and approval 
- Change Development 
- Impliment the Change 
- Test.  Always make sure you have a rollback plan.   
- Postmortem/Lessons Learned/After Action:  Did this work, what is the new state 

## Emergency Change Management. 
- has to happen now 
- need to minimize the delay 
- single member may grant approval 
- Testing and verification proccesses are similarly streamlined 
- go back after the fact and do the regression testing, 
- documentation is still required. 

## Integrated Product Team. 
- collection of multidisciplinary individuals. 

# ID and Identify Security Controls 

- In interpreted languages (Python and Javascript) you can read the source code 

- Libraries - prewriten repositories of common functions, code, classes, scripts, procedures.  It is a collection of functionality to pull from instead of writing from scratch. 
- SDK's speeds developers building programs for specific items but introduces security functions. 
- Pretty much all the code these days comes from libraries. 
- Runetime:  a collection of all hardware and software required to actually run an application.  

## CI/CD 
- Continuous practice of integrating code into a repository 
- we are fixing things quickly and things are up to date. 
- you can bake security testing in. Such as a static code analysis at build and a dynamic code analysis at push to production. 
- CI/CD pipelines will rely heavily on automation.  
- infrastructure as Code.  being able to quickly spin up virtualized sytems using pre-defined templates. 

## SOAR 
- Security Orchestration, Automation, and Response. 
- using known items to automate responses to threats
- the better your inventory, the better SOAR works .

- Orchestration:  soar is going to run analytics, leverage totality of your security tools. 
- Automation:  going to follow playbooks.  
- Response:  automated responses.
- SOAR still requires a human component.  Humans need to respond to the incidents. 
- SOARS get confused with SIEMs.  SIEMs only ingest data, they don't auto respond. 

## Software Configuration Management 
- about managing change and change management in the concept of applying to security 
- ensure configuration changes or cordinatited to not introduce flaws
- uses baselines to set the minimum bar to the least things we have to do 
- Goal is to promote visibility and control over the state of change. Better you manage changes, better you can tie them back to configuration items. 
- Verify you do not violate **CIANA (Confidentiality, Integrity, Authenticity, Non-Repudiation, Authenticity)**  If you are doing this well, a non approved change would be an active threat 

- Code Repositories can help secure code.  Need to be monitored and properly secured. How are you controling access control and communications.  Your repo can be calling other repos.  

## Application Security Testing 
- Static Security testing.  Looking at compiled binaries.  Not run against production typically.  
- Dynamic - Runs at runtime.  Not tied to the IDE, Non-Developers can access the results.  Outside the developers toolset.  
- Interactive Application Security Testing - Pen testing and complex security algorithms, can cause performance issues 
- Runtime Application Self-Protection - executes alongside the application as it runs.  SOAR for security testing basically. 

## Assess the effectiveness of software security 
- Log and automate changes 
- at multiple steps, you need to see that the things you expect to happen are actually happening. 

- Auditing:  is an official inspection of something.  going to follow a standard
- Logging:  is the recording of events.  

- Think about Accountability and Non-Repudiation.  Advisable to use a one-way logging writebox.  No editing after the fact. 

- Logs are generated after the fact.  They tell you what has happened after it is done.  
- look at GreyLog and Splunk for logging.  If doing splunk it is a full time job.  Requires specialized skills.  

- Should be logging events in source code management. Usefull in troubleshooting.  

## Database Terms to Know 
- DBMS:  Database Management System 
- Tables contain attributes known as fields 
- records can be known as tubles 
- Cardinality - the number of rows in a relational database 
- Degree - number of columns 
