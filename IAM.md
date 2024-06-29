## IAM (Identity Access Management)

- Globally resilient service, persistent across all regions for account
- DB that holds access identities
- Restrictions around billing control and account closure, otherwise IAM identities can do everything a root user can do.

### 3 different types of identity objects
 - **User**: Represent humans or applications that need access to your account.
 #### e.g. access to create/terminate EC2 instances, backup application

 - **Group**: Collection of related users that will inherit permissions
 #### e.g. dev team, finance or HR

 - **Role**: Can be used by AWS Services, or for granting external access to your account. Typically used when the number of points of access needed is uncertain.
 #### e.g. can be used to give an EC2 instance access to an account


 ### IAM Policy (Policy Document)
 - Used to allow or Deny access to AWS services when attached to users, groups or roles.

 ### 3 main responsibilities of IAM
 - ID Provider (IDP): Create, modify and delete identities
 - Authenticate: Authenticate/Prove who the user is
 - Authorize: Allow or Deny access to resources

### Important to remember
 - No cost associated with IAM
 - Limits to how many IAM users, groups and roles you can create
 - Global service/ Global resilience
 - **ALLOW** or **DENY** its identities on its AWS account
 - No **direct** control on external accounts or users
 - Identity Federation and MFA

