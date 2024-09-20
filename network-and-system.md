# Network and System Security Policy

## Data Handling Policy

### Types of Data

The following types of data are stored, processed, and/or transmitted on system components that are owned, operated, maintained, and controlled by Screendesk:

- Sensitive: Applies to the most sensitive business information, to which access is strictly limited (e.g., passwords, encryption keys)
- Confidential: Applies to less sensitive business information, which is intended for use solely by Screendesk and/or its customers (e.g., screen recordings, customer support data)
- Public: Applies to all other information that does not clearly fit into the above classifications

### Retention

Screendesk retains Sensitive and Confidential data only for as long as necessary to fulfill its purposes unless otherwise required by law or to meet legal and customer contractual obligations. To support compliance with these obligations, the CTO reviews Screendesk's data retention practices on an annual basis.

### Disposal

Screendesk securely disposes of Sensitive and Confidential data following defined processes once it is no longer necessary for legal, regulatory, or business requirements or it has reached the end of its retention period.

The following methods are used for both hard copy and electronic data:

- Purging and deleting data from all system components using a secure wipe program in accordance with industry-accepted standards for secure deletion
- Destroying any sensitive data that is in a hard copy format (e.g., cross-shredding)

For electronic media stored on system components that are no longer in use, data is disposed of through secure deletion methods.

Instances of customer data disposal are tracked via a ticketing system to document the steps taken to complete the removal.

## Information Security Policy

Screendesk maintains reasonable technical, organizational, and physical security measures to protect the security of Sensitive and Confidential data in transit, at rest, and in storage from unauthorized access or unlawful disclosure.

Critical security controls include, but are not limited to, the following:

- Encryption in transit: Sensitive and Confidential data transfers are sent via a secure transfer system that is transport layer security (TLS) 1.2 or higher.
- Encryption at rest: All Screendesk servers, workstations, and laptops use advanced encryption standard (AES) 256 disk encryption.
- Outbound files: A secure file transfer platform is used to transfer files outside of the Screendesk network.
- Inbound files: During transfer, all files sent into the Screendesk network are verified that they are free of corruption and that the files originated from a known source.
- Database: Screendesk application databases that are externally accessible by web traffic are encrypted and provide a level of identification security using an application-specific protocol such as HTTPS. Sensitive and Confidential data in Screendesk databases is also encrypted from the customer's side before being inserted into the database.
- Data segregation: Sensitive and Confidential data remains in either the on-premises deployment of Screendesk's products or secure cloud environments (Render.com and Amazon S3).
- Data storage: Sensitive and Confidential data is only stored in approved systems, databases, and endpoints (e.g., laptops).
- Cloud storage: Secure and Confidential data is stored in a secure, dedicated cloud environment behind a firewall.
- Production and test environments: Screendesk sanitizes all production data before use in non-production environments, as applicable.
- Incident management: Screendesk maintains a process for identifying, managing, and resolving privacy incidents in accordance with the Screendesk Incident Management Policy.