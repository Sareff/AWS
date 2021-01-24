202101201249
Tags: #z #aws #lessons

---
# Amazon Machine Images

AMI is a virtual image of information to run EC2 instance. 

AMI is locked by account / [region](Regions) (not Availability Zone, THE REGION)

### AMI Copy

You can share an AMI with another AWS account. Sharing an AMI doesn't affect the ownership of the AMI. If you copy an AMI that has been shared with your account, you are the owner of the target AMI in your account.

To copy an AMI that was shared with you from another account, the owner of the source AMI must grant you read permissions for the storage that backs the AMI, either the associated [[EBS]] snapshot (for an Amazon EBS-backed AMI) or an associated [[S3]] [bucket](Buckets) (for an instance store-backed AMI).

#### Limits
You can't copy an encrypted AMI. If the underlying snapshot and encryption key were shared with you, you can copy the snapshot while re-encrypting it, and there for you are a new owner of AMI.

You can't copy an AMI with associated “billingProduct” code that was shared with you. This includes Windows AMIs and AMIs from the AWS Marketplace. To copy such snapshot, launch EC2 instance in your account using the shared AMI ant then create an AMI from the instance.

---
### Zero-Links
- 
---
### Links
- [[EC2]]