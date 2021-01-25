202101251522
Tags: #z #aws #lessons

---
# S3 Versioning



By enabling versioning while creating a bucket (or added this function later in configuration) you can upload same file several times with small changes and every its iteration will be versioned (1, 2, 3, and so on…). 

Versioning allows you protect yourself against unintended deletes and also make it easier to roll back to previous version of the file. Any file that doesn't have a version yet, will have version ‘null’. Disabling Versioning doesn't delete previous versions.

---
### Zero-Links
- 
---
### Links
- [[S3]]
- [[Objects]]
- [[Buckets]]