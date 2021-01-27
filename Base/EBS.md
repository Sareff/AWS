202101201848
Tags: #z #aws #lessons

---
# Elastic Block Storage

### What’s an EBS?

An EBS Volume is a network drive you can attach to your instances while they run. It allows your instances to persist (сохранять) data. It’s a network drive (i.e. not a physical drive). It’s **locked** to an [Availability Zone](<Availability Zones>). To move a volume across AZ's, you first need to [[EBS snapshots|snapshot]] it.

Have a provisioned capacity (size in GBs, and IOPS). You get billed for all the provisioned capacity, but in exchange you can increase and decrease capacity ‘on fly’.

You can also [[EBS Encryption|encrypt]] your EBS Volume for more secure use.

EBS Volumes come in 4 types:
- GP2 (SSD): Balance between price and performance.
- IO1 (SSD): Highest-performance SSD for low-latency, high-throughput workloads.
- ST1 (HDD): low cost, but frequently accessed friendly drive.
- SC1 (HDD): lowest cost, so less frequently accessed designed.

Only GP2 and IO1 can be used as a **boot volume**. See more information in [[EBS Volume Types|use cases]]

One of the last thing you can do with EBS is a creation of [[EBS RAID]]

---
### Zero-Links
-  [[00 AWS]]
---
### Links
- [[EC2]]
- [[AWS]]