202102021247
Tags: #z #aws #concepts 

---
# Amazon S3 Resources

There is a common Amazon Resource Name (ARN) format to identify resources in AWS:

	arn:partition:service:region:namespace:relative-id

An Amazon S3 ARN **excludes** the AWS [[Regions|Region]] and [[Namespaces|namespace]], but includes the following:

- Partition - ```aws``` is a common partition name. If you're in China this would be ```aws-cn```
- Service - ```s3```.
- Relative ID - it is a ```bucket-name``` or ```bucket-name/object-key```.

Therefore the Amazon S3 ARN for resources will look like:

	arn:aws:s3:::bucket_name/key_name



---
### Zero-Links
- 
---
### Links
- [[S3 Bucket Policies]]
- [[Regions]]
- [[Namespaces]]