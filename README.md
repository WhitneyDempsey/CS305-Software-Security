CS 305: Software Security 

This repository contains my Artemis Financial Practices for Secure Software Report and a reflection on my work in CS 305. 

Client and Software Requirements 

Artemis Financial is a financial consulting company that develops individualized financial plans for its customers. The company wanted to improve the security of its web application and protect sensitive financial information. My work focused on adding secure communication through HTTPS, implementing a checksum to demonstrate data integrity, and assessing the application for security vulnerabilities.

Identifying Vulnerabilities and Coding Securely 

I did well at combining automated dependency scanning with manual code review. OWASP Dependency-Check helped identify known vulnerabilities in third-party libraries, while manual review helped me examine the code and configuration changes directly. I also distinguished existing dependency findings from potential issues introduced by my changes 
Secure coding helps protect customer information, maintain trust, and reduce the likelihood for service disruptions and costly security incidents. For a financial company, these protections support both its daily operations and its reputation. 

Challenges and Helpful Parts of the Assessment 

One challenging part was interpreting dependency-check findings. A scan result requires further review to understand whether the vulnerability applies to the application and how it should be addressed. Working through these findings helped me understand why security assessment involves judgment as well as automated tools. I also learned to consider how updating a framework could address several vulnerable dependencies together. 

Adding Layers of Security 

I added layers of security by configuring HTTPS with a certificate and keystore, implementing SHA-256 checksum generation, and reviewing the application though dependency scanning and manual inspection. I kept the keystore password outside the source code by using an environment variable. 

In future projects, I would continue using dependency scanning and manual review alongside the vulnerability assessment process. I would prioritize mitigation based on severity, potential impact, exposure, and whether the affected functionality is used by the application. 

Verifying Functionality and Security 

After refactoring, I ran the application and checked the HTTPS endpoint in the browser to verify that it displayed my unique data and generated SHA-256 checksum. I reviewed the certificate and HTTPS configuration and ran OWSAP Dependency-Check to assess the dependencies after my changes. Manual review provided another check on the modified code and configuration. 

These checks helped me evaluate whether the application still worked and whether my changes introduced additional security concerns. They also reinforced that a working application can still have dependency vulnerabilities that require further attention.

Useful Tools and Practices 

The tools I used included Java, Spring Boot, Eclipse, Maven, Java Keytool, OWASP Dependency-Check and Java's MessageDigest class. Helpful practices included keeping passwords out of source code, documenting changes with screenshots, reviewing automated findings, and checking the final submission files. 

I also learned to very the contents of the final ZIP against the working project. This helps ensure that the submitted files contain the implementation I actually tested. 

Demonstrating My Skills 

This report demonstrates my ability to apply security concepts to a Java web application and explain the results. It provides examples of configuring HTTPS, generating a certificate, implementing SHA-256 hashing, and reviewing dependency vulnerabilities. I could show future employers both the technical work and my ability to document security decisions, testing, and remaining concerns. 
