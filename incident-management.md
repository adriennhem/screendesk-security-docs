# Incident Management Policy

Screendesk distinguishes between security events and security incidents as follows:

- Security event: A suspicious activity that deviates from normal behavior but does not appear to compromise any system resources. Security events include phishing emails, changes in login permissions, spikes in incoming traffic, and similar situations. Events may be elevated to incidents if determined by authorized personnel.
- Security incident: A suspicious or malicious activity that compromises a system resource and is being used for unauthorized purposes. Security incidents include data breaches, a successful distributed denial-of-service (DDOS) attack, or similar situations where the incident is so large that it may involve a legal team, public disclosure, or a failure to meet contractual commitments with customers.

## Incident Management Roles and Responsibilities

The Incident Response Team (IRT) has clear roles and responsibilities for adequately preparing for and responding to any incident. The IRT follows the necessary steps, processes, and procedures to address an incident as well as to understand what actions (if any) to take with law enforcement agencies, local/federal/state agencies, the media, and any other third parties considered to be within scope.

Given Screendesk's small size, the IRT consists of both employees, with the CTO (Adrien Nhem) serving as the primary responsible party. The IRT is responsible for the following:

- Declaring a security incident
- Leading the incident response process after the incident is declared through a postmortem
- Determining what other teams or individuals are required to contribute to the response process
- Coordinating investigation and remediation efforts
- Keeping stakeholders informed
- Performing an annual test of the Incident Response program through a tabletop exercise

## Incident Response Procedures

These procedures outline the steps necessary to address security and performance related events and incidents in order to ensure the confidentiality, integrity, and availability of Screendesk's platform and supporting systems. The IRT should follow the appropriate procedure based on the incident severity ranking:

- Low: Indicates attempted suspicious activity that did not compromise the network (e.g., a port scan or a failed intrusion attempt). Low severity is treated as a security event.
- Medium: Indicates suspicious activity that deviates from normally observed behavior and, depending on the use case, may be indicative of a resource compromise. Medium severity is treated initially as a security event but may be elevated to a security incident.
- High: Indicates the resource in question (e.g., an EC2 instance or a set of IAM user credentials) is compromised and is being used for unauthorized purposes. High severity is a true security incident.

### Medium and Low Event Procedure

1. Initial response: IRT reports incident to all internal staff
2. Investigation: Investigates the issue
3. Internal notification: Notifies all staff via appropriate communication channels

### High Security Incident Procedure

1. Initial response: IRT reports incident to all internal staff
2. Documentation: Raises a ticket in ticketing system and update as needed
3. Investigation: Investigates the issue
4. Internal notification: Notifies all staff via appropriate communication channels
5. External notification: Determines if notification to customers and authorities is necessary and, if so, sends notification

## Business Continuity and Disaster Recovery (BC/DR) Plan Testing

Screendesk tests its business continuity (BC) capabilities on at least an annual basis.

The IRT is responsible for overseeing the execution and documentation of the annual BC/DR Plan test. Screendesk employs a tabletop exercise to simulate an unexpected service disruption to the product platform. Testing assesses the adequacy of Screendesk's BC/DR plans and associated procedures to do the following:

- Restore product accessibility
- Communicate with internal and external parties
- Recover data
- Support capacity needs for information processing, telecommunications, and environmental support in specified contingency conditions

Screendesk documents the results of the annual BC/DR Plan test through a post-simulation report that details the following:

- A description of the simulated service disruption
- A summary of Screendesk's BC response actions
- Any identified issues and findings resulting from the BC/DR Plan test, including suggested updates
- Screendesk's performance against KPIs

## Backup

Screendesk performs backups of Sensitive, Confidential, and Public data for all in-scope production systems, including infrastructure and data stores necessary to maintain service level agreements (SLA) with customers.

Screendesk configures its cloud service providers (Render.com and Amazon S3) to perform backups of all data stored in the cloud. CSP backups are performed using the CSP's automated backup tool.

Backups are stored in a secure remote location at a sufficient distance to escape damage from a disaster at the main site of processing. Data will be retained for a period determined by business needs and regulatory requirements.

Backups are tested annually by the Engineering team to ensure that they can be restored and relied upon in an emergency. As part of testing, management determines their ability to meet the company's restoration time requirements.