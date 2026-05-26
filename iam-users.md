## IAM Users Created

### dev-user
- **Group Membership**: Developers
- **Permissions**: Inherited `ReadOnlyAccess` via group
- **Purpose**: Simulates a developer who needs to view resources for troubleshooting
- **MFA**: Disabled
- **Console Access**: Enabled

### admin-user  
- **Group Membership**: Administrators
- **Permissions**: Inherited `AdministratorAccess` via group
- **Purpose**: Simulates an admin responsible for managing AWS resources
- **MFA**: Enabled using Google Authenticator
- **Console Access**: Enabled
