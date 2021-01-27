202101241635
Tags: #z #aws #lessons #qt 

---
# RDS Read Replicas

RDS Read Replicas - a method to provide [[High Availability]] and [[Perfomance]] to RDS DB Instances. 

You can create up to 5 Cross/Within AZ, or Cross Region Read Replicas. Replications is always ==**asynchronous**==, so reads are eventually consistent (If read replica reads data before it was changed in main DB, replica will return old data). Replicas can be **promoted to their own DB**.

> Use case: 
> Suppose you have a production DB that is taking a normal load. But you need to run a reporting application to run some analytics. If you chose main data base for it, more likely DB would be overload. So, to avoid such situations you must create a Read Replica to run the new workload there.

![[Read Replicas Disaster Recovery.png|500]]

---

#### Quick Tip
>RDS Read Replicas take a fee when data goes from different AZ, to avoid this, you can create Main and Read DB in same AZ. It will **reduce you cost dramatically**.

---
### Zero-Links
- 
---
### Links
- [[RDS]]
- [[AWS Best Practices]]
- [[Availability Zones]]