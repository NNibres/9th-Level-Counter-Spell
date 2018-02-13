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
| Risk Name | Description | Plan |
| ------------- |-------------| -----|
| 1. Penetration Testing Tools| We have chosen an array of penetration testing tools to use for the CoRA application. But there are still numerous problems we can encounter throughout the project. Application availability problems, user account lockout and others can occur due to the tests themselves. Another possible issue is being able to utilize these tools properly to find vulnerabilities on the CoRA application.  | Our plan is monitor this risk throughout the testing and look for any possible issues that could be mitigated. |	
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
| Pen-Testers | Nathaniel Dobesh, Jacob Miranda, Alsalt Alkharusi|
|Documenters | Nikko Nibres, Alsalt Alkharusi, Nathaniel Dobesh |

## Project Methodology

### Literature Review

For this project, there will be penetration testing conducted on the CoRA website. The purpose of the website is to correlate the bones found in the warzone and areas of conflict and map them back to fallen heroes. The information related to the fallen heroes is located in a database.

Now in order to conduct the penetration testing, there has to be a certain plan put into place. The idea of penetration testing is not a foreign concept in this day and age. Many companies, large and small use professional hackers or penetration testers to find issues with their system. This same idea is how the team will be tackling this problem. The main piece of literature that directly influences our team, is a book called The Hacker Playbook 2. This book layouts step-by-step how penetration testing is implemented in the real world. These steps go in the following order: The Setup, Scanning the Network, Exploiting Scanner Findings, Manual Web Application Findings, Moving Through the Network, Social Engineering, Attacks that Require Physical Access, Evading AV, and Reporting. 

This project may not require all of these steps in order to achieve our goal. The customer is requiring us to find vulnerabilities in the system that the developers have not found out about. Since this a closed system for now that could be deployed to a larger environment, some areas will not be explored. For example, our team will likely have no need to look into social engineering. This is the practice of manipulating people to gain access to the system. Since this a closed system, and does not have anywhere to social engineer our ways into the system, it will not be necessary to use this methodology. 

On the other hand, we will be using methods like scanning the network, to find out about other avenues that the customer make have not considered at first. For instance, the web application will typically have it’s traffic sent through either port 80 (HTTP) or 443 (HTTPS). It may not be aware to the customer that another port is opened to the Internet, like port 22 (SSH) where potential attackers could enter the system. 

Kim, P. (2015). The hacker playbook 2 practical guide to penetration testing. North Charleston, SC: CreateSpace by Amazon Distribution GmbH.

### Technical Plan

The plan that our team will follow will directly correlate to the plan that The Hacker Playbook 2 describes. Essentially, there are three main focuses for this project where different members of our team will be assigned to. Those three main focuses include the actual penetration testing, scripting, and documentation. 

Penetration testing is the process of finding the vulnerabilities in the system, in our case it is the CoRA web application. There are numerous different avenues to which one can find different access points to infiltrate the system. The Hacker Playbook 2 lays out in stages how to conduct penetration testing on a system. First comes the setup, where one would gain the necessary tools to that will aid the tester in gaining access to the system. The book informs the user of all software needed, for multiple different operating systems, how to get them, and if there are any paywalls involved with the software mentioned. For example, Nathan Dobesh will be a part of the penetration testing group and his operating system of choice will be Linux (Ubuntu). The book even tells what commands are needed to be entered to get the tools. Once the penetrating system is setup, then begins the actual process of penetration testing. First, we scan the network, followed by the utilization of the findings from the scans to gain access to the system. It is to our benefit that part of the book focuses on manual web application penetration testing. This will be where the bulk of our testing will come from. 

As the penetration testers find the different vulnerabilities in the system it is then the job of the scripters to take the findings and automate them. The team will use this to show the customer our findings; also this will verify our findings to show that they are reproducible. The customer and developers can use the scripts to their benefit to make their system protected from such attacks in the future. The customer has shown us the environment in which he would like us to script in. The team will be using PHP as the main scripting language while using a framework called Laravel Dusk. The IDE solution that we will be using will be PHPStorm. To make the scripting even easier for us, the customer has directed us to use a command line environment in order to test our scripts which is called Laravel Homestead.

The final part of our plan is documentation. This part of the process is not exclusive to one specific part of the project. In fact, as the penetration testers find a new vulnerability with the system, it is up to the documenters to write down what was found, how it was found, when, etc. When it comes to scripting, in-code comments and documentation will need to be written to explain our process at this stage of the project. 

