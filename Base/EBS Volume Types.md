202101211909
Tags: #z #aws #lessons #concepts 

---
# EBS Volume Types

Name | Use Cases | Specification
--- | --- | ---
GP2 | Recommended for most workloads<br />System boot volumes<br />Virtual desktops<br />Low-latency interactive apps<br />Development and test environments | 1 GiB – 16 TiB<br />Small gp2 volumes can burst IOPS to 3000<br />Max IOPS is 16.000<br />3 IOPS per GB, means at 5.334 GB we are at the max IOPS 
IO1 | For critical business apps that require sustained IOPS performance, like more than 16.000 IOPS per volume (GP2 limit)<br />Large DBs such as MongoDB, Oracle, PostgreSQL and so on… | 4 GiB – 16 TiB<br />IOPS is provisioned (PIOPS) – Min is 100 – Max is 64.000 (for ‘Nitro’ instances) else Max is 32.000 (other instances)<br />The maximum ratio of provisioned IOPS to requested volume size (in GiB) is 50:1 (50 IOPS for 1 GiB)
ST1 | Streaming workloads<br />Big Data, Log procession, Data warehouses<br />Apache Kafka<br />**Cannot be a boot volume** | 500 GiB – 16 TiB<br />Max IOPS is 500<br />Max Throughput of 500 MiB/s – can burst
SC1 | Throughput-oriented storage for infrequent accessing<br />Scenarios where the lowest storage cost is crucial<br />**Cannot be a boot volume** | 500 GiB – 16 TiB<br />Max IOPS is 250<br />Max throughput of 250 MiB/s – can burst

---
### Zero-Links
- 
---
### Links
- [[EBS]]