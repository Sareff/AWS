202101212004
Tags: #z #aws #lessons

---
# EBS RAID Configuration

**RAID** (англ. Redundant Array of Independent Disks — избыточный массив независимых дисков)

EBS is already **redundant**. But if you want to increase your IOPS, or mirror your EBS just in case? You can mount volumes in RAID. There is RAID 0, 1, 5, 6 (the last two are not recommended for EBS according to AWS documentation).

RAID 0 for performance – there is one logical volume and two EBS volumes (just for example). The data is distributed between this two volumes. That means that we’re now have more capacity in total, and more IOPS as well, but on the other hand, if one of the disks fails, all data is failed. The use cases would be an application that requires a lot of IOPS and doesn't need fault-tolerance, or a data base that has replica already.

RAID 1 is the opposite to RAID 0. It is designed to increase fault tolerance. Like in the previous example, suppose we have a logical volume and two EBS volumes. The data now will be mirrored between them. So if one of the disks fails, the data is secure.

---
### Zero-Links
- [[00 Computer Science]]
---
### Links
- [[EBS]]