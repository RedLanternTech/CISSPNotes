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

Tokens:
- Synchronous  depends on timing
- Asynchronous:  depends on a math formula.  you type a number and it gives you one

Biometrics
- most expensive
- Need to look at the convergence of the False Reject Rate (type 1 error) and False accept rate(type 2 error).  False Accept is worse than a False Reject.  
- Crossover error rate is where the two meet. 
- See pages 122 and 123 of 11th Hour for the different types

