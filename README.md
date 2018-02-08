# 9th-Level-Counter-Spell
CYBR Capstone Project - CoRA Security Testing
## Executive Summary
### Problem Statement
The University of Nebraska at Omaha ISQA department is currently in the works of developing a new application for the Department of Defense. The PHP-based web application will examine human bones that have been scattered in an underwater area and determine if each part can be grouped up to form a full skeleton. This application is called CoRA (Commingled Remains Analytics). CoRA employs standard user roles and rights grouping mechanisms in order to provide proper authentication and authorization for the application. 

The application needs to meet NIST and DoDI application security standards, so the goal of this project is to use automated methods to perform security testing on CoRA. This involves developing test cases and using various scripts to test the application for security vulnerabilities. We are to note down our findings and report them to our client from the ISQA department so that their team can perform and change requests to the application as needed. The findings need to be documented and reproducible in such a way that future students involved in the CoRA project can be brought up to speed quickly on the security testing procedures for future iterations of the application.
### Problem Merit
This project is important for this team not only for the practical applications but also for families affected by the loss of their loved ones in war. CoRA’s recovery of those remains can be that added measure of closure for people left behind by these fallen warriors. Securing the application ensures that measure of closure can be fulfilled.
### Project Goals
* Set up testing environments
* Developing test cases for the application
* Employing test cases to develop PHP test scripts for automatic security testing of CoRA
* Report findings to client, along with scripts and documentation



## Project Timeline
![alt text](https://github.com/NNibres/9th-Level-Counter-Spell/blob/master/Images/Timeline1.PNG)
![alt text](https://github.com/NNibres/9th-Level-Counter-Spell/blob/master/Images/Timeline2.PNG)
![alt text](https://github.com/NNibres/9th-Level-Counter-Spell/blob/master/Images/Timeline3.PNG)

## Risk List Ranked by Risk Level

| Risk List | Description | Chosen option |
| ------------- |-------------| -----|
| 1. Penetration Testing Tools| We have chosen an array of penetration testing tools to use for the CoRA application. But there are still numerous problems we can encounter throughout the project. Application availability problems, user account lockout and others can occur due to the tests themselves. Another possible issue is being able to utilize these tools properly to find vulnerabilities on the CoRA application.  | Our plan is monitor this risk throughout the testing and look for any possible issues that could be mitigated.  |	
| 2.Requirements fail to align with systems  |  The CoRA requirements fail to align with other systems (e.g. they duplicate functionality). This risk could potentially impact our objective because the requirements may cause issues with the systems we use and create complications and delay. | Our plan is to mitigate this risk and make sure that the tools and systems used in the project are aligned with the CoRA requirements. |
| 3. Learning curves lead to delay | Our project team would need to acquire new skills for the project and there's a possible risk that productivity will be low. Given that PHP is the scripting language we have to use for the CoRA application to make test cases could cause some delay and affect the project timeline. | Our plan is to mitigate this risk as much as possible and make sure that we are on top of things and put extra hours on the learning objectives if needed. | 
| 4. Under Communication| Communication is crucial when it comes to project management. Under communication is a risk that could potentially cause issues with our project expectations, project timeline, project changes and team members expectations. | Our plan is to monitor this risk and make sure everyone is on the same page on the project. |
| 5. System Outages |  System outages could happen throughout the project. Critical systems such as the test environments could go down which may cause loss of important project components including test scripts and documentation.  |  Our plan is to monitor this risk and make sure all scripts and documentations are saved properly. |		

## Resources & Technology needed:
1) Github: The first tool that we will use while working in our project is Github. We will use Github to upload our work and the work could be some tests, user cases, scripts, results and many other things. This Github repository can be viewed by the students, instructor, as well as the client later on. Moreover, the whole group is going to work on this tool since all the work has to be uploaded to Github.
 
2) Burp suite: The second tool that we will use is called Burp suite. Burp suite is a java-based penetration-testing tool that is used widely by information security professionals to identify any vulnerability that can be used by attackers to attack a particular system. We are planning to use this tool to do some penetration testing on Cora to identify any vulnerabilities.
 
3) Zap: The third tool that we are going to use is Zap. OWASP ZAP is an open source web application that is used by both beginners to application security as well as professionals in penetration testing; this tool is used for network scanning. We will use this tool for the same purpose as burp suite.
 
4) VM: The fourth tool that we are going to use is a virtual machine. In the VM we going to do all penetration testing, create scripts and test them, so basically we are going to do most of the work if not all of it in VM.   
 
5) Phpstorm:  Another tool we will use is called Phpstorm. This tool provides an editor for PHP, HTML, and java script; it also contains error prevention and automated refactoring for PHP and java script code.  We are already working on this tool and it took a while for us to set it up, but it is now working and we have started working on it.
 
6) Laravel Homestead: This tool is a great tool that contains pre-packaged vagrant box, which provides an environment for developing without requiring to install PHP, a web server, and any other server software tools on local machine, so it saves time, offer, and it is a great tool that contains tools needed for development.

7) Dusk: This tool is used for application testing, it is based on the open source tools ChromeDriver and Facebook Php-webdriver which makes it simple to use without the need to experience the long and intense procedure of setting up selenium.

| Role      | Group Members                                 |
| ----------| ----------------------------------------------|
| Scripters | Nikko Nibres, Michael Sullivan, Jacob Miranda |
| Pen-Testers | Nathaniel Dobesh, Jacob Miranda             |
|Documenters | Nikko Nibres, Alsalt Alkharusi, Nathaniel Dobesh |


