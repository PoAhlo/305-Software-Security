# 305-Software-Security
Repository for SNHU CS-305: Software Security

#### Briefly summarize your client, Artemis Financial, and their software requirements. Who was the client? What issue did they want you to address?
Artemis Financial is a financial consulting company that develops individualized financial plans for savings, retirement, investments, and insurance for their patrons. They came to my company, Global Rain, in hopes to modernize their their web-based software and apply the most current and effective software security. They wanted to secure their RESTful APIs.

#### What did you do particularly well in identifying their software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall wellbeing?
I feel that I consistently could identify when input wasn't validated.  Input validation is essential to preventing injection attacks, and it can be helpful to be able to give users feedback if they don't enter data correctly.  Secure coding as a whole is important because you protect your data and organization from attacks.  Software security adds a layer of protection over the company, giving executives peace of mind that the software is not a weak point of the company. 

#### What about the process of working through the vulnerability assessment did you find challenging or helpful?
I found it particularly difficult determining false positives.  I discovered that you can use dependency:analyze to determine which dependencies were unused.  However, I found it tedious to go through each vulnerability and still not be able to be 100% sure whether or not the vulnerable feature is being used.

#### How did you approach the need to increase layers of security? What techniques or strategies would you use in the future to assess vulnerabilities and determine mitigation techniques?
There were a few ways that layers of security were added.  Most notably, data was encrypted using SHA-256.  To do this, I used the Google Guava dependency.  As for vulnerability assessment, I can see myself using Maven's dependency check in the future.  I understand how that works, and I have improved at identifying false positives (although I know I still miss some).  

#### How did you ensure the code and software application were functional and secure? After refactoring code, how did you check to see whether you introduced new vulnerabilities?
I simply ran the code to verify that the code was functional.  I didn't run into any issues with syntax or logic errors during this project.  I also didn't have any input in my code to validate, so there weren't any introduced security issues.  I reran the dependency check to verify that no vulnerabilites were introduced.  I actually introduced a vulnerability at first, which was mitigated by updating Google Guava.

#### What resources, tools, or coding practices did you employ that you might find helpful in future assignments or tasks?
I used Trello to create a Kanban board for my assignments.  This has proved very helpful in managing my time.  I also see myself using the dependency check and the NVE database in the future.  

#### Employers sometimes ask for examples of work that you have successfully completed to demonstrate your skills, knowledge, and experience. What from this particular assignment might you want to showcase to a future employer?
I now understand how to identify vulnerable dependencies and many different kinds of code vulnerablities.  More importantly, I learned how to mitigate these vulnerabilities.  
