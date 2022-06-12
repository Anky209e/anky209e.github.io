---
title: Scaliblity and Elasticity in Cloud
date: 2022-06-12 10:05 -500
categories: [AWS,Cloud,Notes]
tags: [aws,cloud,scalablity,elasticity,notes]
---

# **Scaliblity and Elasticity-A brief**
### The world’s largest public cloud providers can accomplish a great deal through combining the wonders of server virtualization with the power that comes from owning vast datacenters filled with racks upon racks of hardware resources. Elasticity and scalability are the two key principles through which a lot of this happens, and understanding exactly what they mean can help you optimize your design choices so you’ll get the most bang for your cloud buck.

### Note that there really are no precise and authoritative definitions for scalability and elasticity in the context of cloud computing—and any definitions you do see are bound to involve at least some overlap. Nevertheless, building some kind of picture in your mind of how these two principles work can be valuable.

# **Scaliblity**
### A scalable service will automatically grow in capacity to seamlessly meet any changes in demand. A well-designed cloud-based operation will constantly monitor the health of its application stack and respond whenever preset performance metrics might soon go unmet.The response might include automatically launching new server instances to add extra compute power to your existing cluster. But it will probably also involve prepopulating those instances with the application data and configuration settings they’ll need to actually serve your application to your clients.

# **Elasticity**
### You can stretch an elastic band far beyond its resting state. But part of what makes it truly elastic is the fact that, when you let go of it, it immediately returns to its original size. The reason the word elastic is used in the names of so many AWS services (Elastic Compute Cloud, Elastic Load Balancing, Elastic Beanstalk, and so on) is because those services are built to be easily and automatically resized

### Generally, you set the maximum and minimum performance levels you want for your application, and the AWS service(s) you’re using will automatically add or remove resources to meet changing usage demands. By way of illustration, a scalable ecommerce website could be configured to function using just a single server during low-demand periods, but any number of additional servers could be automatically brought online as demand spikes. When demand drops back down, unused servers will be shut down automatically.
