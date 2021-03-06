# Configuration Management Policy

Ovation standardizes and automates configuration management through the use of Salt scripts and AWS Elastic Beanstalk deployment environments, as well as documentation of all changes to production systems and networks. Salt and Elastic Beanstalk automatically configure all Ovation systems according to established and tested policies, and is used as part of our Disaster Recovery plan and process.

## Applicable Standards from the HITRUST Common Security Framework

* 06 - Configuration Management

## Applicable Standards from the HIPAA Security Rule

* 164.310(a)(2)(iii) Access Control & Validation Procedures

## Configuration Management

1. Salt and/or AWS Elastic Beanstalk environments are used to standardize and automate configuration management.
2. OSSEC is used to scan systems every 2 hours and on reboot. These scans capture file system changes and also unauthorized or malicious software.
3. No systems are deployed into Ovation environments without approval of the Ovation Chief Architect.
4. All changes to production systems, network devices, and firewalls are approved by the Ovation Chief Architect before they are implemented. Additionally, all changes are tested before they are implemented in production.
5. An up-to-date inventory of systems is maintained using AWS and Catalyze dashboards. All systems are categorized as production and utility to differentiate based on criticality.
6. Clocks are synchronized across all systems using NTP. Modifying time data on systems is restricted.
7. All front end functionality (developer dashboards and portals) is separated from backend (database and app servers) systems by being deployed on separate servers.
8. All software and systems are tested using unit tests and end to end tests.
9. All committed code is reviewed using pull requests (on Github) to assure software code quality and proactively detect potential security issues in development.
10. Ovation utilizes development and staging environments that mirror production to assure proper function.
12. Ovation schedules production deployments every four weeks or on an as-needed basis. In all cases, all Customers are notified of production deployments at least 14 days in advance of deployment.
13. All formal change requests require unique ID and authentication.
14. All configuration changes to development, staging or production systems are logged and auditable.
