202101212008
Tags: #z #aws #lessons #qt

---
# Identity and Access Management

AWS Identity and Access Management (IAM) enables you to manage access to AWS services and resources most securely. There is only three conceptual things - **Users**, **Groups** and **Roles**. And **Policies** inside every of them.

- **Users** for a physical person who use AWS;
- **Groups** for consolidation Users by any kind of specific qualities;
- **Roles** for AWS internal resources, such as EC2 instance and so on.
- **Policies** (JSON Documents) for definition what they can and cannot do.

IAM is one of services that has **a Global View** (not belong for any Region or AZ)

#### Quick Tip:
> It’s best to give users the **minimal** amount of permissions they need to perform their job (least privilege principles).

---
### Zero-Links
- [[00 AWS]]
---
### Links
- [[AWS]]
- [[EC2]]
- [[S3]]
- [[RDS]]