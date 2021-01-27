202101271131
Tags: #z #aws #lessons #qt

---
# S3 Encryption

There are 4 methods of encrypting objects on S3:

-   **SSE-S3** - encrypts S3 objects using keys handled & managed by AWS
-   **SSE-KMS** - leverage AWS Key Management Service to manage encryption keys
-   **SSE-C** - when you want to manage your own encryption
-   **Client-Side Encryption** - Fully manageable by user encryption process 

The last two methods only provided in a [[AWS CLI|CLI]], in GUI there are only S3 and [[KMS]] methods. (LOL)

---

#### SSE-S3

Objects are encrypted on server side. The encryption type is **AES-256**. To make S3 encrypt your object, you need to upload it in the S3 bucket with a special header:

	"x-amz-server-side-encryption" : "AES256"

#### SSE-KMS

This type of encryption is also server-side, but has some advantages over S3 encryption: It provides us user control and audit trail over encrypted files. For this type of encryption you must set header:

	"x-amz-server-side-encryption" : "aws:kms"

#### SSE-C

Amazon S3 doesn't store the encryption key you provide. To make this method work you must use HTTPS (for more security of course). Encryption key, obviously, must be provided in HTTP headers, for every HTTP request made.

#### Client-Side Encryption

Client must encrypt data by himself before sending it to S3. Also, clients must decrypt data, when retrieving from S3. For this kind of task we can use Amazon S3 Encryption Client. 

---

#### Quick Tip
> Amazon S3 exposes HTTP (not encrypted) and HTTPS (encrypted in flight) as well. HTTPS are more common and recommended

---
### Zero-Links
- 
---
### Links
- [[S3]]
- [[AWS CLI]]
- [[KMS]]