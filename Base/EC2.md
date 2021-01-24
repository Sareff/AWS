202101201238
Tags: #z #aws #lessons 

---
# Elastic Cloud Computing

EC2 - it is a virtual cluster of computers that AWS gives you in real time trough the Internet. You can decide it's amount of GPUs, CPUs, RAM, Disk-space and so on by choosing [[Instance type]]. '

You can also decide the method of deploying your instance by choosing it's [[Launch type]].

Every instance you can create is based on virtual image of operational system with some basic applications (e.g. Linux, Windows, MacOS) - it's called [[AMI]]. 

Instances have two types of permanent memory - [[Internal storage]] and [[EBS]].

If you want to manage properly your EC2 instance traffic, there is crucial AWS tool that will help you - [[Security Groups]].

All activity with EC2 instances takes place in the console. In this console you can also manage your [[EBS]] volumes, [[AMI]]s and [[ELB]] with [[ASG]].

Every instance has it's own IP of two types - **private** and **public**. It's provided by another AWS service called [[VPC]].

---
### Zero-Links
- [[00 AWS]]
---
### Links
- [[AWS]]
- [[Instance type]]
- [[Launch type]]
- [[AMI]]
- [[Security Groups]]
- [[EBS]]
- [[ELB]]
- [[ASG]]
- [[VPC]]