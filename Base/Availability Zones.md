202101201725
Tags: #z #aws #lessons #concepts 

---
# Availability Zones

Each region has multiple, isolated locations called Availability Zones. Inside them we can place our AWS resources such as [[EC2]], [[RDS]] and so on... They are isolated by real geographical location between each other (about 100km), but still are inside one [region](Regions)!

The Availability Zone is represented by a [region](Regions) code followed by a letter identifier. For example ```us-east-1a``` are a Availability Zone inside ```us-east-1``` region which in its turn are datacenter located at N. Virginia. 

This is a scheme: 

![Regions](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/images/aws-az.png)

---
### Zero-Links
-  [[00 AWS]]
---
### Links
- [[AWS]]
- [[Regions]]
- [[VPC]]
- [[Subnets]]