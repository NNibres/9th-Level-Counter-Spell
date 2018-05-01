# 9th-Level-Counter-Spell | CYBR Capstone Project - CoRA Security Testing

## Executive Summary
### Problem Statement
The University of Nebraska at Omaha ISQA department is currently in the works of developing a new application for the Department of Defense. The PHP-based web application will examine human bones that have been scattered in an underwater area and determine if each part can be grouped up to form a full skeleton. This application is called CoRA (Commingled Remains Analytics). CoRA employs standard user roles and rights grouping mechanisms in order to provide proper authentication and authorization for the application.

The application needs to meet NIST and DoDI application security standards, so the goal of this project is to use automated methods to perform security testing on CoRA. This involves developing use cases and creating automated test scripts to verify the application meets the authentication and authorization policies. We are to note down any defects found during testing and report them to our client from the ISQA department so that their team can perform and change requests to the application as needed. The automated scripts need to be documented and robust in such a way that future students involved in the CoRA project can be brought up to speed quickly on the testing procedures for future iterations of the application.

### Problem Merit
This project is important for this team not only for the practical applications but also for families affected by the loss of their loved ones in war. CoRA’s recovery of those remains can be that added measure of closure for people left behind by these fallen warriors. Securing the application ensures that measure of closure can be fulfilled.

## Project Goals
Set up testing environments
Develop use cases for the application
Develop automated PHP test scripts for automatic security testing of CoRA
Report findings to client, along with scripts and documentation

## Project Methodology
### Literature Review
For this project, we used PHP test scripts on the CoRA website. The purpose of the website is to correlate the bones found in a warzone and areas of conflict and map them back to fallen heroes. The information related to the fallen heroes is located in a database.

Initially, the team had planned to conduct two separate types of testing on the site: 1) manual vulnerability findings via scanners and automated reconnaissance (penetration testing), and 2) PHP scripts to test the access that varying types of users had to different pages and functions of the site. The team originally was using Peter Kim’s Hacker Playbook as a resource for the first partition of security testing (the pen-testing). We used the Laravel Dusk website, online crowd sources, and the client as resources for the second partition of the project.

Kim, P. (2015). The hacker playbook 2 practical guide to penetration testing. North Charleston, SC: CreateSpace by Amazon Distribution GmbH.

### Technical Plan


The scope of the project did adjust when we realized that the project would need to focus much more on the second partition, the PHP automated test scripts. The penetration part of the project didn’t really take off, as the point of the project was not to find intrusion points from outside the site, but more so to find potential scope creeping of user roles. 

This adjustment meant that we could all focus on the scripting process. Essentially, our first step was to setup get familiar with the testing environment (in our case, it’s the Laravel Dusk test framework). From this point we started developing some use cases from a URI routelist that the client provided to us. This gave us a good starting point for potential URI’s a user could navigate to on the CoRA site.

Once we had the test environments setup and the use cases ready, we were able to get started on scripting. Essentially, we developed scripts for each of the possible places that the user could navigate to on the site, testing the different things that the user could see and interact with. We made separate scripts for the different types of users and different pages they were designed to test. We also developed the scripts so that the functions therein could be run separately. Modularity was a pretty important goal we had in mind when developing the scripts. Each script comes with documentation so that the person looking at it will generally know what it does.

## Results/Findings
Overall achievements through the project:
- Created Use Cases for General Authentication Functions
- Created Use Cases for Authorization Scope for Security Roles for Users
- Created Use Cases for Authorization Scope for Organizations
- Created Use Cases for Administrative Functions
- Learned about setting up and utilizing a Selenium-based test environment
- Created about 60 automated test scripts for multiple users under two different organizations
- Further understand the Laravel Dusk framework
- Implement selectors that are commonly used in specific pages
- Report bugs/defects we found during testing

## Install Instructions
### Install Requirements
- Have access to CoRA Test Github Repository from client.
- Access to a testing device capable of downloading software listed in Installation Instructions.

### Installation Instructions
1. Install Vagrant to testing device.
2. Install Virtual Box or similar to testing device.
3. Install PhpStorm from JetBrains.
4. Use Vagrant to install Laravel Homestead virtual machine onto Virtual Box.
5. Configure .yaml file for Homestead
6. Pull CoRA Test repository into PhpStorm from client.
7. Configure .env file in CoRA Test
8. Create PHP Test scripts in CoRA Test

### Getting Started
1. Validate test scripts do not contain any syntax errors.
2. Execute test scripts using the “php artisan dusk” commands
3. Review testing results and/or screenshots from executing tests
