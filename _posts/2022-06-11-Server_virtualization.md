---
title: Server Virtualization
date: 2022-06-11 12:00 -042
categories: [AWS,Cloud,Notes]
tags: [aws,cloud,virtualmachines,notes]
---
***
# Server Virtualization in Cloud Computing.
### The secret sauce that lets cloud providers give their customers on-demand compute resources in such a wide range of configurations is virtualization. When you request a virtual machine (VM) with a particular processor speed, memory capacity, and storage size, AWS doesn’t send some poor engineer running through the halls of its data center looking for an available machine with exactly that profile. Rather, as you can see illustrated in Image below, AWS carves the necessary resources from larger existing devices.

![server_virtual_image](https://www.researchgate.net/profile/Saravanan-P/publication/339749899/figure/fig1/AS:866155900174336@1583519067300/Figure1-Architecture-of-Server-Virtualization.ppm)

### A 5 TB storage drive could, for instance, be divided into dozens of smaller virtual volumes, each associated with a different virtual server (or instance). And the resources of a single physical server could be invisibly shared between multiple instances. The operating systems installed on each of those instances could run, blissfully unaware that they’re actually only masters over a small subset of a much larger server environment.
***
# Advantages of virtualization.
## Speed

##### Defining, purchasing, provisioning, testing, and launching a new physical server can take months. Even a simple reboot can keep you waiting for a couple of minutes. The time lag between requesting a new cloud-based VM and logging in and getting to work can be seconds, but never more than a few minutes. Restarting a VM can some- times happen faster than you can type your login details.

## Efficiency

##### It’s rare to find a nonvirtualized physical server that utilizes anywhere near 100 percent of its capacity. More likely, either it’ll spend its time running mostly empty or it’ll be badly overused while you wait for more capacity to come online. Multiple virtual machines, on the other hand, can be tightly packed onto a physical server running a hypervisor (a common technology for hosting VMs). When space opens up on one server, you can quickly fill it with another virtual workload.