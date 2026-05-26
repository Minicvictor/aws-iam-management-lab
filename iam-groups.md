## IAM Groups Created

### Developers
- **Attached Policy**: `ReadOnlyAccess` (AWS Managed)
- **Permissions**: Can view all AWS resources but cannot create, modify, or delete them
- **Use Case**: Developers and QA who need visibility without risk of changing infrastructure

### Administrators
- **Attached Policy**: `AdministratorAccess` (AWS Managed)
- **Permissions**: Full access to all AWS services and resources
- **Use Case**: Senior admins and lab testing. Not recommended for production without restrictions
