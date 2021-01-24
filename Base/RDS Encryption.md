202101241704
Tags: #z #aws #lessons #practice 

---
# RDS Encryption

RDS can encrypt your DB Instance. When the data is encrypted **at rest** all storage, backups, read replicas, snapshots will also be encrypted.

RDS Encryption use AES-256 as encryption algorithm to encrypt your data (like in [[EBS Encryption]]). After the data is encrypted, AWS handles authentication of access and decryption of your data **transparently**.

If the master DB isn't encrypted, the read replicas cannot be encrypted.

To encrypt unencrypted DB, you should create a snapshot, which will be unencrypted, copy it into an encrypted snapshot and after all of this create new encrypted DB out of encrypted snapshot. (Kill me)

---
### Zero-Links
- 
---
### Links
- [[RDS]]