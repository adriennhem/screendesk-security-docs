# Access Control Policy

Access controls establish standards and procedures for preventing unauthorized access to information assets.

## Principle of Least Privilege

Access rights to Screendesk system components are limited to authorized personnel and are based on a user's role and responsibilities. Access rights to Screendesk system components must adhere to the concept of least privilege at all times.

The principle of least privilege grants users the bare minimum level of access to operating systems that is needed to perform their role or carry out their job responsibilities. Screendesk applies least privilege to its systems to add an additional layer of security over the data and information that a user handles and to reduce the risk of users abusing their access privileges.

## Privileged Users

Privileged users are those with elevated or superuser access to in-scope systems and system components that is granted according to business needs. At Screendesk, the CTO (Adrien Nhem) serves as the primary privileged user, responsible for ensuring that the access rights for all users (including the CEO and any future employees or contractors) are commensurate with:

- The user's role and responsibilities within Screendesk (this principle is known as role-based access control)
- The concept of least privilege and separation of rights based on job duties

## Provisioning Users

When an employee or contractor joins Screendesk, they are given the appropriate tools and access to Screendesk systems. During the process of onboarding, employees are assigned unique identifications (ID) and are sent the organization's policies. Employees must acknowledge having read and received the policies before being granted access to the information systems and networks needed to carry out their roles and responsibilities.

Users for all in-scope systems and system components are provisioned using all applicable provisioning and de-provisioning tools as necessary. This includes access to:

- Render.com (cloud provider)
- Amazon S3 (for storing recordings)
- Any other critical systems used in Screendesk's operations

## User Identifications

When a new user is onboarded, they are assigned a unique Screendesk employee ID. This ID defaults to the user's first name in lowercase text. If that ID already exists, then the ID will be the user's first and last name.

Employees are strictly prohibited from sharing IDs or from using another user's ID, regardless of whether the other user has granted permission.

## User Access

Once an ID has been assigned to a new user, a formal access request must be submitted to and approved by the CTO. When the access request is approved, the new user is given access to their Screendesk email, internal resources, and any other elevated permissions that their role requires them to have.

This same process is applied when existing employees require additional levels of access.

## Deprovisioning Users

For any modifications to or removal of access, a formal access request is required to ensure these actions are documented and completed in a timely manner. Terminated employees have access revoked within twenty-four (24) hours of termination.

## Access Review Policy

All employee access to production systems is reviewed by the CTO at least quarterly to confirm the access of each employee is appropriate and complies with the principles of least privilege and separation of duties.

The access review and any modifications to system access are formally documented and tracked.

## Identification and Authentication Policy

All users are authenticated through unique IDs and passwords or through authorized secure shell (SSH) keys in order to access Screendesk's information systems and networks.

Screendesk uses automated access control systems to restrict user access to its network and data. These automated access controls require users to authenticate before they may access any of the following:

- Screendesk's network
- Screendesk's source code
- Screendesk's and its customer data
- Other restricted data

All users must use multi-factor authentication (MFA) measures to ensure that access to in-scope system components are protected at all times.

## Password Policy

Passwords are a critical component of information security. Passwords protect user accounts and must be configured according to Screendesk's password policies. Screendesk requires users to create and use complex passwords.

Passwords must be safeguarded, and owners should not share them with other users. Passwords used by all users must meet or exceed all stated Screendesk policies for password complexity requirements.

### Password Complexity

Screendesk requires that all passwords meet or exceed all of the following guidelines:

- Contain at least twelve (12) alphanumeric characters
- Contain both upper and lowercase letters
- Contain at least one number
- Contain at least one special character (e.g., $%^&*()_+|~-=\`{}[]:";'<>?,/).

Weak passwords are prohibited. Weak passwords have the following characteristics:

- Contain less than twelve characters
- Can be found in a dictionary, including foreign language, or exist in a language slang, dialect, or jargon
- Contain personal information such as birthdates, addresses, phone numbers, or names of family members, pets, friends, etc.
- Contain work-related information such as building names, system commands, sites, companies, hardware, or software

### Invalid Password Lockouts

Parameters regarding account lockout policies and password resets are enforced with system settings. Only the CTO is allowed to make any changes to the password complexity rules and lockout policies.

## Remote Access to Production Systems

All access to Screendesk system components initiated outside the organization's trusted network infrastructure is considered "remote access." Remote access to production systems is restricted to authorized employees with a valid MFA token.

All users must use approved technologies, such as internet protocol security (IPSec) and/or secure socket layer (SSL) virtual private networks (VPN) for remote access. These approved protocols are to be used along with MFA and additional supporting measures such as secure shell keys (SSH).