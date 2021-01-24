202101241635 
Tags: #z #aws #lessons #concepts

---
# RDS Multi-AZ

Multi-AZ, or Multi [Availability Zone](<Availability Zones>) - the method of providing RDS users [high availability](<High Availability>) and [failover](Failover) support. Multi-AZ deployments for **MariaDB, MySQL, Oracle, and PostgreSQL** DB instances use Amazon's failover technology.

Multi AZ standby RDS DB is always ==**synchronous**==. So, suppose we have same [[DNS]] to receive requests. Over the [[DNS]] we have two DB – first is our **Main DB**, and second is our **Standby DB**. Both of them are in different [AZs](<Availability Zones>). While first DB is okay, second DB continue synchronize data. If first DB fails, the second start to maintain requests and also become a new Main DB (promoted). 

> Note: The Read Replicas can be setup as Multi AZ for Disaster Recovery (DR).

![[Multi-AZ.png]]

---
### Zero-Links
- 
---
### Links
- [[RDS]]
- [[Availability Zones]]
- [[AWS Best Practices]]