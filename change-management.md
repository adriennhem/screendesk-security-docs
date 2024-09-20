### Pre-Implementation Testing (continued)

time. Validation efforts in this environment consist of automated functionality and security testing.

### Approval

Screendesk seeks to produce new releases swiftly yet with the oversight necessary to promote quality and assure adequate controls:

- Before pushing a release to production, the CTO must approve changes classified as having a major impact.
- Any visible changes to end-user-facing documents and interfaces are automatically cataloged and require manual review and approval.
- All changes in implementation or configuration require approval by the other team member who did not implement the change.
- A successful execution, completed during the pre-implementation testing phase, is required for releasing a feature in production.

### Staging Deployment

After obtaining final approval, the change is deployed to a staging environment whose configuration fully mimics the production environment. Multiple changes may be bundled automatically into a single deployment to facilitate rapid development and iteration.

Validation is achieved in this environment by a successful deployment of all requested changes, followed by automated testing that simulates user behavior. Successful completion of all staging tests automatically initiates deployment to the production environment.

### Production Deployment and Communication

Once a staging deployment has been successful, an identical deployment is initiated in the production environment.

- If the deployment succeeds with no errors, the change request is marked as successfully merged, the Git version control system is updated to reflect the changes, and Engineering is notified of the change.
- If the deployment encounters an error, any changes are automatically rolled back and the implementer is notified of the failure. Once a defect has been repaired or a feature has been fully realized by Engineering, Product members associated with the change request are notified that the change is complete, and the system of record is updated.

### Rollback Procedures

Screendesk's ability to execute rollback procedures depends on the change(s) that need to be rolled back. If a rollback is possible, Engineering is able to address an issue in near real time by reverting to a previous version of the product.

### Continuous Improvement

Although the System Change Management Policy presents the change management process linearly, Screendesk accumulates feedback throughout the system development process, reviews and prioritizes requested changes, and reflects those changes as incremental improvements to the product.

## Inventory Management Policy

Screendesk's management maintains a system asset inventory that does the following:

- Accurately reflects the organization's production systems
- Includes all system components
- Does not duplicate components that appear in multiple systems
- Maintains enough information to track and report on assets – in particular, marking relevant assets as "critical" and verifying that they meet security baseline requirements
- Indicates whether assets store or access Sensitive and/or Confidential data
- Notes any approved deviations to current deployed configurations
- Assigns ownership of system components and documents assignees' acknowledgment of ownership
- Documents accountability information, including responsibility and ownership, by name, position, or role

## Change Communication

Screendesk communicates any major changes to the system to authorized internal users (e.g., feature releases). For major system changes, Screendesk follows these steps:

1. Obtains final approvals from authorized staff
2. Deploys the feature in either the organization's internal production environment or in a customer's environment (in conjunction with the customer's personnel)
3. Sends release notes that describe the functionality introduced with the release, provide examples of how to use the new functionality, note fixes to material bugs identified during prior releases, and list known limitations