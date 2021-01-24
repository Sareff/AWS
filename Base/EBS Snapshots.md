202101211928
Tags: #z #aws #lessons

---
# EBS Snapshots

EBS Snapshot - it's a backup of your EBS Volume taken point-in-time.

They are **incremental** (save only changed blocks after most recent snapshot). It’s much more desirable if you take a snapshot of the volume at rest (not a lot of traffic to be handled). 

Snapshots are stored in [[S3]] (but you can’t directly see them). It’s recommended to detach volume before you take it's snapshot. The maximum amount of snapshots per account is ==**100.000**==. 

You can copy snapshots across [AZ](Availability%20Zones.md Zone>) or [Region](Regions) (not EBS volumes themselves). And also you can make [[AMI]] from snapshot. EBS volumes restored by snapshots needed to be pre-warmed (using ```fio``` or ```dd``` command). 

Snapshots can be automated using [[Amazon Data Lifecycle Manager]].

---
### Zero-Links
- 
---
### Links
- [[EBS]]