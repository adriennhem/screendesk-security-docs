# Monitoring Policy

## Event Monitoring Policy

Screendesk implements comprehensive auditing and monitoring controls to identify and capture the following events:

- All authentication and authorization activities by all users and their associated accounts (e.g., successful and unsuccessful login attempts)
- Any access to or creation, modification, or deletion of Sensitive or Customer data
- All actions taken by privileged users
- Malicious activity

Screendesk monitors system components to capture these events with specialized software such as File Integrity Monitoring (FIM), Host-based Intrusion Detection Systems (HIDS), and/or change detection software programs. Notifications are set up to alert the CTO if immediate action needs to be taken.

The CTO is responsible for monitoring and communicating changes and events.

## Performance and Utilization Monitoring Policy

Screendesk monitors system components (e.g., servers) for appropriate performance and utilization by taking the following measures:

- Process monitoring: Screendesk monitors all critical processes and provides alerting and notification measures when processes fail.
- Network interface monitoring: Screendesk monitors the overall health and status of the network interface.
- CPU utilization: Screendesk identifies current, real-time capacity of the central processing unit (CPU) and sends alerts and notifications if capacity is over limits and/or assets are underutilized.
- Memory utilization: Screendesk identifies current, real-time memory usage and sends alerts and notifications if memory usage is high and/or if memory availability is low.
- Disk utilization: Screendesk identifies current, real-time disk space and sends alerts and notifications if disk space is low.

## Logging and Reporting Policy

Along with capturing all necessary events described in the Event Monitoring Policy, Screendesk implements protocols to log, store, and review all required events and their associated attributes as necessary.

### Logging

Screendesk uses capturing and forwarding protocols (e.g., Syslog) and/or specialized software applications or other technology as necessary to protect the confidentiality, integrity, and availability of audit trails and their respective log reports that are produced by monitoring activities.

### Review

The CTO reviews all applicable user permissions and related output (e.g., log reports) to identify any issues or concerns and report them immediately to appropriate personnel.

### Reporting

Any anomalies, such as unauthorized configuration changes in the logs, are escalated in accordance with the Incident Management Policy.