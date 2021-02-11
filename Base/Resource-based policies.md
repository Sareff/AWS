202102111733
Tags: #z #aws #concepts

---
# Resource-based policies

Resource-based policies are JSON policy documents that you attach to a resource such as an Amazon S3 bucket. These policies grant specific permissions to a specific service and under what circumstances these permissions would be granted. Resource-based policies are inline based policies [^1].  There are no managed resource-based policies.

![[Identity and Resource -based policies.png | 450]]

The IAM service support only one type of resource-based policy called a role *trust policy*, which is attached to an IAM role.

[^1]: policies that attach only to one identity and deletes only with it

---
### Zero-Links
- 
---
### Links
- [[IAM Policies and Permissions]]