202101251522
Tags: #z #aws #lessons #qt 

---
# S3 Versioning

Versioning by it means is a keeping several versions of an [[Objects|object]] in the same [[Buckets|buckets]].

By enabling versioning while creating a bucket (or adding this function later in configuration) you can upload same file several times with small changes and every its iteration will be versioned (1, 2, 3, and so on…). 

Versioning allows you protect yourself against unintended deletes and also make it easier to roll back to the previous version of the file. Any file that doesn't have a version yet, will have version ==**"null"**==. 

![[S3 Versioning.png]]

---

#### Quick Tip

> Disabling (Suspend) Versioning doesn't delete previous versions. 
> 
> Also by doing it you aren't actually disable versioning at all - it can't be possible by any circumstances, because once you enabled versioning, it will be PERMANENT for your bucket.

---
### Zero-Links
- 
---
### Links
- [[S3]]
- [[Objects]]
- [[Buckets]]