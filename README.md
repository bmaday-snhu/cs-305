# cs-305
Software Security 2026


**Briefly summarize your client, Artemis Financial, and its software requirements. Who was the client? What issue did the company want you to address?**

Artermis Financial is a financial services provided helping clients with wealth management. The company has a customer face webapp that needed to be safe and secure for use by their clients and comply with all current industry best practices and government reulations.

**What did you do well when you found your client’s software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall well-being?**

One thing I did well was examine the codebase and use case across all the possible dimensions of threats. Using the Vulnerability Assessment Process Flow Diagram I could go through the eight areas of concern. This was not only for the webapp but also for storing customer data at rest for long periods of time. It is important to code securely from a regulatory, financial, and business perspective. You want to avoid lawsuits from clients, actions from governments, and of course build a reputation you can be trusted with your clients data.

**Which part of the vulnerability assessment was challenging or helpful to you?**

The hardest part was the dependency scanning. Being able to wade through hundred of CVEs looking for false positives, false negatives, and legitimate issues was sometimes more an art than a science. You also have to deal with out of date packages and vulnerability reposittory. Understanding the difference between dependency scanning and static analysis took a bit to discern the pros and cons of each.

**How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?**

Adding TSL/HTTPS was one of the biggest improvements along with dependency scanning. TSL ensured that data in transit is protected which is a basic industry requirement for any financial institution and essential to protecting data. I believe with dependency scanning I'd integrate it into the CICD workflow so that vulnerabilities are found early and often and can be addressed by the developers closet to the code. This helps with false negatives and positives.

**How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?**

I refactored the code to add SHA-256 check sum capabilities. I checked for new vulnerabilities by rescanning the codebase package dependencies to ensure I did not use packages that had vulnerabilities.

**What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?**

Using frameworks for common tasks in whatever software developer toolkit is essential. For example, using standard library tools to create SHA-256 encryptions, or handle certificates with keytool, ensured I was able to implement industry practices easily without having to make my own. Reading the documentation for the SDK you're using is useful so you're aware of what is available to you.

**Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?**

I'd point them to the breadth of the examination. Being secure happens along a lot of threat vectors and it's important to demonstrate you have a good understanding of when to use different techniques like encryption, input sanitization, endpoint security, and authentication vs authorization.  Showing future employers a holistic approach to security should inspire confidence in my knowledge and expierence.
