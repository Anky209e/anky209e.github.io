---
title: Shared Responsibility Model:AWS
date: 2022-06-15 1:25PM
categories: [AWS,Cloud,Notes]
tags: [aws,regions,infrastructure,online]
---
***

# **What is AWS Shared Responsibility Model?**
### Amazon distinguishes between the security and reliability of the cloud, which is its responsibility, and the security and reliability of what’s in the cloud, which is up to you, the customer

### AWS is also on the hook for patching, encrypting (where relevant), and maintaining the operating systems and virtualization software running its physical servers and for the software running its managed services.

### *But what exactly is "managed" and "unmanaged" services?*

![srm](https://d1.awsstatic.com/security-center/Shared_Responsibility_Model_V2.59d1eccec334b366627e9295b304202faf7b899b.jpg)

# **Managed Resources**
### A managed cloud service will “hide” all or some of the underlying configuration and administration work needed to keep things running, leaving you free to focus on the “business” end of your project. For example, an application running on an EC2 instance might need a database in the backend. You could install and configure a MySQL database engine on the instance itself, but you’d be responsible for patches, updates, and all the regular care and feeding (not to mention letting it out for its morning walks).

# **Unmanaged Resources**
### The most obvious example of an unmanaged AWS service is EC2. When you launch an EC2 instance, you’re expected to care for the operating system and everything that’s running on it exactly the way you would for a physical server in your onpremises data center.Still, even EC2 can’t be said to be entirely unmanaged since the integrity of the physical server that hosts it is, of course, the responsibility of AWS.

# **Service Health Status**
### As part of its end of the bargain, AWS makes regularly updated, region-by-region reports on the status of its services publicly available. Any service outages that could affect the performance of anyone’s workload will appear on [Amazon’s Service Health Dashboard](https://status.aws.amazon.com) often within a minute or two of the outage hitting.

# **AWS Acceptable Use Policy**
### Because they’re so easy to scale up, cloud computing services are powerful tools for accomplishing things no one had even dreamed of just a decade ago. But for that same reason,they’re also potential weapons that can be used to commit devastating crimes.
### [The AWS Acceptable Use Policy](https://aws.amazon.com/aup) makes it abundantly clear that it does not permit the use of its infrastructure in any illegal, harmful, or offensive way. Amazon reserves the right to suspend or even terminate your use of its services should you engage in illegal, insecure, or abusive activities (including the sending of spam and related mass mailings). *Even running penetration testing operations against your own AWS infrastructure can cause you trouble if you don’t get explicit permission from Amazon in advance.*

> Learn more about [AWS Shared Responsibility Model](https://aws.amazon.com/compliance/shared-responsibility-model/)