202101251523
Tags: #z #aws #concepts #essentials 

---
# Keys

A Key is a unique identifier for an [object](Objects). Every object that stored in the bucket has exactly one singe key. The combination of a bucket, [version ID](<S3 Versioning>), and key allow us to identify every object in S3.

The key by itself is a compose of prefix and the object name (from the last example prefix will me ```my\_folder/another_folder/``` and object name ```my_file.txt```).

For example, the key will be every character after the name of bucket: ```s3://my-bucket/my_file.txt``` - is the key as well as - ```s3://my-bucket/my_folder/another_folder/my_file.txt```.

---
### Zero-Links
- 
---
### Links
- [[Objects]]
- [[S3 Versioning]]