Security Operations
- Maintain operational resilience
- protect valuable assets
- effective security services management

Least Privilege 
- give the user exactly what they need to do the job, no more
- cannot set and forget privileges, must always be followed up and audited
 
 Separation of Duties
 - take two people to do a task.  Think launching nuclear missiles

Job Rotation/Tour of Duty Jobs
- avoids abuse of privileges
- cross-trains people to do a job so one person doesn't know it
- Mandatory vacations also apply here

# FRSecure notes

- SecOps - is about the day to day operations and maintenance of the information security process. 

## Understanding and complying with investigations 

#### Four Types of evidence by which facts can be proven or disproven at trial 
- Real evidence - physical evidence, material items, can be held and touch.  
- Demonstrative evidence;
- Documentary evidence 
- Testimonial evidence 
- [FindLaw Real and Demonstrative Evidence](https://www.findlaw.com/criminal/criminal-procedure/real-and-demonstrative-evidence.html)

- integrity of the evidence is critical
- **DOCUMENT EVERYTHING**  If your going to fast to document everything, you are going too fast.
- document dates, times, physical locations, logical locations
- **Never Tamper** with the original versions of anything.  **ALWAYS** make a write-block, make bit-level copies, and investigate on the copies.  
- every second must be accountable
- chain of custody must be maintained 
- ISO/IEC 27037:2012 
- [NIST 800-86](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-86.pdf)
- avoid subjective interpretation

## Admissibility of Evidence
- accuracy 
- Authenticity 
- Comprehensibility 
- Convincing 
- Objective 
- Admissible 
- [Admissible Evidence](https://www.law.cornell.edu/wex/admissible_evidence)

## Investigative techniques 
- Data capture 
- Interviews 
- Interrogations 
- External requests

## Patch Management 
- Activity of detecting vulnerabilities 
- Patch Publication:  when a vendor puts out a patch 
- Evaluation:  always evaluate a patch.  Always evaluate cost vs benefit when looking at a patch.  Installing a patch may induce a greater risk. 
- Testing:  ensure a patch wont cause a problem.
- Rollback:  know a way out
- Documentation: know who did what.  

## Change Management 
- ITIL has good guidelines and change management controls
- With emergency changes, documentation is done later 

## Backup Strategy 
- always make sure you a doing a cost-benefit analysis 
- for a good backup,go with 3-2-1 Rule.  3 copies of data should be kept, two stored locally and one stored offsite.  
- the same security controls on the systems, should be on the backups as Well 
- always check the backups integrity and that they are working 
 
 ### cloud 
 - loss of physical control over data needs to be evaluated against cost savings 
 
## Disaster Recovery Process 
- BIA:  Buisness Impact Analysis 
- BC:  Business Continuity 
- DR:  Disaster Recovery 
- BCDR:  Combining the process areas of business continuity and disaster recovery.  
- RTO's and RPO's must be defined.  
- Recovering cross-functional organization processes requires the participation of a cross-functional team. 

### Reponse 
- **Health, Life Saftey trumps all.  All your plaining should be around this**
- Coordinated response:  You want a disaster recovery plan and business continuity plan 
- clear and consistent communications:  have plans in place
- document everything 

- having job rotation and cross-training can support cotingency operations so someone can take multiple roles. 

### Restoration 
- Primary Site and Secondary Site.  used to avoid confusion between old and new facilities 
- goal of **recovery** is the resumption of critical business functions 
- goal of **restoration**** is to return to normal service levels 
- The more you know, the safer you will be 
- Make sure personal understand how to respond. 

- always perform a review after a disaster.  Call a postmortem, after action report, retrospective, or lessons learned 

- Always test your plans, keep them simple. 
  - Table Top 
  - simulation 
  - Parallel 
  - Full interuption (tested as if a real disaster had occurred).  Insanely expensive, just don't do it or do it on a subsystem at a time
- CISSPs are there to help develop the plans but may not impliment or run them. 

## Physical Security 
For the CISSP, you no longer need to know the different types of fire extinguishers 

You do need to know what type of fire suppression to put into a data center 

Know that you need to have a travel restriction in some cases.  Don't want all the key people on the same plane.  

Duress - where a person is forced to do something against their will Blackmail and being held hostage are extream examples. 


