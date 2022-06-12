---
title: AWS Free Tier
date: 2022-06-12 05:01PM
categories: [AWS,Cloud,Notes]
tags: [aws,freetier]
---
***

# **How AWS Free tier Works?**

### It’s remarkable how much you can do with the Free Tier. Since, for instance, you’re allowed to run a t2.micro Elastic Cloud Compute (EC2) instance—powered by either Linux or Windows—for up to 750 hours per month, you can effectively keep a low-demand website going without interruption for your full first year. In fact, you’d be surprised how much you can get done with such a resource.

### You don’t have to consume those 750 Free Tier EC2 hours by running a single instance 24/7. You could instead choose to experiment with something more complex, such as a high-availability deployment involving running two or four concurrent instances for a few hours to test resilient failover architectures. As long as the total monthly hours of run time don’t exceed 750, your credit card won’t be billed.

# **Tracking Your Free Tier Usage**

### Of course, accidentally leaving AWS resources running—whether you’re enjoying the Free Tier or not—can cost you much more than $1.16. Firing up a synchronously replicated RDS database instance to test your new website backend and then forgetting all about it can easily cost you thousands of dollars a month. You definitely want to keep an eye or two on your account.

### By default, Free Tier–related email alerts are automatically sent whenever account activity approaches or has passed Free Tier limits. Besides turning them off from the Preferences page in the Billing Dashboard in the AWS Management Console, the only thing you can do about alerts is to choose a different email address.

![Billing-1](https://d1.awsstatic.com/getting-started-guides/tutorials/control-your-costs-7.59248cd849dcdbc27abb89a3e598eb819da6305b.png)

![Billing-2](https://d1.awsstatic.com/getting-started-guides/tutorials/control-your-costs-8.04e2a338baf42477330b067b7e1b092682869cb3.png)

![Billing-3](https://d1.awsstatic.com/getting-started-guides/tutorials/control-your-costs-9.76a9dc240822a1758d1e81d474dfd86cc4dc43c7.png)

> Got to [Documentation](https://aws.amazon.com/getting-started/hands-on/control-your-costs-free-tier-budgets/) to learn more.