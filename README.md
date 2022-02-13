# AWS-Static Website Hosting!
STATIC WEBSITE HOSTING  With S3 , IAM Policies , CDN - Cloudfront.

# Project Objectives
1) S3 bucket creation
2) S3 bucket configuration
3) Website distribution via CloudFront
4) Access website via web browser

# Creation of S3 Bucket
1) Bucket Name - staticwebproject
2) AWS Region  - Asia Pacific (Mumbai)
3) Object Owneership - ACL Disabled
4) Block Public Access settings for this bucket -  Unchecked -  So We can access this Bucket
5) Bucket Versioning -  Disable
6) Default Encryption - Disable

# Bucket Permissions

Bucker Policy 

{
  "Version":"2012-10-17",
  "Statement":[
    {
      "Sid":"AddPerm",
      "Effect":"Allow",
      "Principal": "*",
      "Action":["s3:GetObject"],
      "Resource":["arn:aws:s3:::your-website/*"]
    }
  ]
}

Granting access for Pulbic access through Bucket Policy.

# Configuring S3 Bucket

Properties -> Static Website Hosting -> Enable.

# CDN - CLoudfront

Distributed S3 Bucket via CloudFront.

Url - > https://d2ytl54sq0i9y9.cloudfront.net/index.html



