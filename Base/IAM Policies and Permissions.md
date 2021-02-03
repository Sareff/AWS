202102021741
Tags: #z #aws #lessons #essentials #concepts 

---
# Policies and permissions in IAM

When you want to manage your access to AWS services, you use policies that are attached to [[IAM]] identities (users, groups, roles) or AWS resources. A policy by itself is simply an object inside AWS that, when it associated with identity or resource, defines permissions. AWS evaluates policies only when IAM principal (user or role) makes a request. Permissions in policy determine if the request allowed or denied. Most policies are stored in AWS in JSON documents.

IAM policies define especially permissions for an action, but not the method that you use to perform the operation. For example, if a policy allows the ```GetUser``` action, then an identity with that policy attached can get user information from the AWS Management Console, AWS CLI, AWS API.

### Policy types

This is a policy types, sorted by frequency, that are available for use in AWS:

- [[Identity-based policies]] - Attach managed and inline policies to IAM identity. This type of policy grant permissions to an identity.
- [[Resource-based policies]] - Attach inline policies to resources. The most common examples of such type policy is a [[S3 Bucket Policies]] and IAM role trust policies. Resource-based policies grant permissions to the principal that is specified in the policy.
- [[Permissions boundaries]]
- [[Organizations SCPs]]
- [[Access control lists]]
- [[Session policies]]
	
---
### Zero-Links
- 
---
### Links
- [[IAM]]
- [[JSON Policy Elements]]
- [[S3 Bucket Policies]]