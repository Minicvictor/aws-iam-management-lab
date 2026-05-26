
# AWS IAM Management Lab

## Objective
Practice identity and access management in AWS IAM by creating users, groups, policies, and testing the least privilege principle.

## Steps Performed
1. Created 2 IAM users: `dev-user` and `admin-user`
2. Created 2 IAM groups: `Developers` and `Administrators`
3. Attached the `ReadOnlyAccess` AWS managed policy to the Developers group
4. Attached the `AdministratorAccess` AWS managed policy to the Administrators group
5. Added `dev-user` to the Developers group
6. Added `admin-user` to the Administrators group
7. Enabled MFA using an authenticator app for `admin-user`
8. Tested sign-in and permissions for both users using the account sign-in URL
9. Captured screenshots for verification

See the `screenshots/` folder for evidence of each step.

## Challenges Encountered
- **Challenge**: Accidentally gave `AdministratorAccess` to both users initially.  
  **Fix**: Removed the policy from `dev-user` and retested to confirm read-only access worked.
- **Challenge**: MFA setup failed on first attempt due to time drift on my phone.  
  **Fix**: Synced time in Google Authenticator and re-entered the codes.
  

## Cleanup
Deleted test users and groups after completing the lab to avoid unnecessary charges and security risk.
