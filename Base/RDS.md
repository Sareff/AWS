202101241626
Tags: #z #aws #lessons 

---
# Relational Database Service

RDS, as it's mentioned in its name are Relational Database that runs in AWS and managed fully by them. All you have to do is create and use it. With RDS you can create such databases: 

- PostgreSQL 
- MySQL
- MariaDB
- Oracle
- Microsoft SQL Server
- [[Aurora]] (AWS Proprietary DB)

RDS has some advantage over EC2 with DB on it. First of all:
1. RDS fully automated and OS patching by AWS. 
2. RDS has monitoring dashboard, backups, [Multi-AZ](<RDS Multi-AZ>), [Scaling capabilities](<RDS Autoscaling>), [EBS storage](EBS), **BUT**, in exchange, you can’t [[SSH]] into RDS instance.

But, on the other hand, RDS have similar capabilities with EC2, such as: [[RDS Encryption]]

RDS have two **main methods** to increase its availability and fault tolerance: [[RDS Multi-AZ]] and [[RDS Read Replicas]]. 

---
### Zero-Links
- [[00 AWS]]
---
### Links
- [[AWS]]
- [[EBS]]
- [[ASG]]