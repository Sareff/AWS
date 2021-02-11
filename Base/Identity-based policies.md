202102101148
Tags: #z #aws #concepts 

---
# Identity-based policies

Identity-based policies are JSON permissions policy documents that control what actions, with what resources, and under what conditions, identity [^1] are able to perform.

There is three main categories of Identity-based policies:
- **Managed policies** - Single policies that can be attached to multiple identities in AWS account. Divides in two:
	- **AWS Managed policies** - Managed policies that are created by AWS.
	- **Customer managed policies** - Managed policies that you create and manage in your AWS account. These policies are way more deep in customization that AWS's ones.
- **Inline policies** - Policies that you add directly to a specific single identity. These policies maintain a strict one-to-one relationship between a policy and an identity.

[^1]: Users, Groups, and Roles.

---
### Zero-Links
- 
---
### Links
- [[IAM Policies and Permissions]]