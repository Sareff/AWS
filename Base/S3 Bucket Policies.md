202101271421
Tags: #z #aws #lessons

---
# Bucket Policies

A bucket policy is a resource-based AWS [[IAM Policies and Permissions|IAM]] policy. You create a bucket policy to grant access to a bucket to other AWS accounts or IAM users access permissions for the bucket and objects in it.

A policy contains this basic set of elements:

- [[Resources]] - The Amazon S3 resources such as buckets, objects, access points and so on, for which you can grant or deny permissions. Use [[ARN]] to identify resource;
- [[Actions]] - For each resource, Amazon S3 support a set of operations. To identify resource operations you need to use keywords;
- [[Effect]] - The _allow_ or _deny_ effect to user's request for specific action. If effect isn't written in policy, the final result would be _deny_ as a default.
- [[Principal]] - The user, account, service or other entity that is the recipient of permission.
- [[Condition]] - The if statement that activates when policy is active.

This is a example of usual bucket policy JSON syntax:

```json
{
    "Version": "2012-10-17",
    "Id": "ExamplePolicy01",
    "Statement": [
        {
            "Sid": "ExampleStatement01",
            "Effect": "Allow",
            "Principal": {
                "AWS": "arn:aws:iam::123456789012:user/Dave"
            },
            "Action": [
                "s3:GetObject",
                "s3:GetBucketLocation",
                "s3:ListBucket"
            ],
            "Resource": [
                "arn:aws:s3:::awsexamplebucket1/*",
                "arn:aws:s3:::awsexamplebucket1"
            ]
        }
    ]
}
```

---
### Zero-Links
- 
---
### Links
- [[S3#Security in S3]]