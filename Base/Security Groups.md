202101201630
Tags: #z #aws #lessons #essentials 

---
# Security Groups

Security groups - it is some kind of firewall, that you must assign to your cloud resource (instance, database and so on) to allow traffic from specific port inbound and outbound.  

Security Groups regulate:

- Access to Ports
- Authorized IP ranges – IPv4 and IPv6
- Control of inbound network (from other to the instance)
- Control of outbound network (from the instance to other)

Security Groups are locked down to a [region](Regions) / [[VPC]] combination

Example:
![[Inbound SG rules.png]]
![[Outbound SG rules.png]]

---
### Zero-Links
- 
---
### Links
- [[EC2]]
- [[RDS]]
- [[ELB]]
- [[AWS]]
- [[VPC]]