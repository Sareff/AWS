202101211942
Tags: #z #aws #lessons #practice 

---
# EBS Encryption

EBS Encryption is a method of protecting your [[EBS|EBS Volume]] by using one of the most popular cryptographic cipher - **AES-256**.

When you encrypt [[EBS|EBS Volume]], all data (and data from [[EC2]] to volume), all future [[EBS Snapshots|snapshots]] will be encrypted as well. 

Encryption and Decryption are handled transparently. Encryption has a minimal impact on latency. 

EBS Encryption leverages keys from [[KMS]] (AES-256). Copying an unencrypted  [[EBS Snapshots|snapshot]]  allows encryption.  [[EBS Snapshots|Snapshots]] of encrypted volumes are encrypted.

---
### Zero-Links
- 
---
### Links
- [[EBS]]