---
title: Regions:AWS Global Infrastructure
date: 2022-06-15 12:40PM
categories: [AWS,Cloud,Notes]
tags: [aws,regions,infrastructure,online]
---
***

# **Regionally Based Services**

### When you request an instance of an AWS service, the underlying hardware of that instance will be carved out of a server running in one—and only one—AWS Region. This is true whether you’re talking about an Elastic Compute Cloud (EC2) virtual machine instance, its Elastic Block Store (EBS) storage volume, a bucket within Simple Storage Service (S3), or a new Lambda “serverless” function. In all those cases, although that anyone anywhere in the world can be given access to your resources, their underlying physical host can exist in no more than one region.

### Of course, that’s not to say you can’t choose to run parallel resources in multiple regions—or that there aren’t sometimes edge-case scenarios where it makes sense to do so. But you must always be aware of the region that’s active for any resource launch you’re planning.

### Through no fault of the AWS designers, it’s surprisingly easy to accidentally launch a new resource into the wrong region. Checking your current region should become a second-nature reflex—much like the quick mirror checks (we hope) you regularly perform while you’re driving a car

# **Globally Based Services**

### Remember that absolute, immutable, and fundamental law we mentioned a bit earlier about all AWS resources existing in one and only one region? Well, rest assured, dear friend, that it is indeed absolutely, immutably, and fundamentally true. Except where it isn’t. You see, some AWS resources are not visibly tied to any one region. Even if those resources are, technically, running on hardware that must exist within a single region, AWS presents them as global. As a rule, their global status will generally make sense from a structural perspective. Here are some examples of global services:

* AWS Identity and Access Management (IAM) is the service for managing the way access to your account resources is achieved by way of users and groups, roles, and policies.
* Amazon CloudFront is the content delivery network you can use to lower access latency for your application users by storing cached versions of frequently requested data at AWS edge locations.

# **Service Endpoints**

### To work with or access the resources you’re running within AWS Regions, you’ll have to know how they’re identified. Your developers or administrators will, for instance, want to connect with resources through their application code or shell scripts. For such access, they’ll often authenticate into your account and list and administrate resources and objects by referring to the endpoint that’s specific to a particular region and service.

### For example, the correct endpoint for an EC2 instance in the us-east-1 (Northern Virginia) region would be ```ec2.us-east-1.amazonaws.com```
> For up-to-date list of endpoints visit [here](https://docs.aws.amazon.com/general/latest/gr/rande.html)
