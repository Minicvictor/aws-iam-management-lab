## Least Privilege Principle

The principle of least privilege states that users, systems, and processes should have only the minimum permissions necessary to perform their required tasks.

### Why It Matters
- **Reduces Risk**: Limits damage if credentials are stolen or misused
- **Prevents Accidents**: Stops users from deleting or modifying resources unintentionally  
- **Simplifies Auditing**: Easier to review and justify permissions during audits
- **Improves Compliance**: Meets requirements for frameworks like SOC 2, ISO 27001

### How It Was Applied in This Lab
- `dev-user` received only `ReadOnlyAccess` through group membership. This allows viewing EC2, S3, and other services without risk of changes.
- `admin-user` has `AdministratorAccess` but is protected by MFA to reduce risk.
- We avoided using the AWS root account for daily tasks.
- We avoided attaching admin permissions to `dev-user`.

### Better Practice for Production
Instead of `AdministratorAccess`, create custom IAM policies that allow only specific actions on specific resources. Example: allow `s3:GetObject` and `s3:ListBucket` on a single S3 bucket.
