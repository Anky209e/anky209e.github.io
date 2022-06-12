---
title: Serverless Workloads and AWS Lambda
date: 2022-06-12 09:57 -500
categories: [AWS,Cloud,Notes]
tags: [aws,serverless,workloads,notes,awslambda]
---
***
# Serverless Workloads
### Besides doing an excellent job emulating traditional server behavior, cloud providers can also enable entirely new ways to administrate applications and data. Perhaps the most obvious example is serverless computing.

### Now don’t be fooled by the name. You can’t run a compute function without a computer environment (a “server”) somewhere that’ll host it. What “serverless” does allow is for individual developers to run their code for seconds or minutes at a time on some else’s cloud servers.

### The serverless model—as provided by services like **AWS Lambda—makes** it possible to design code that reacts to external events. When, for instance, a video file is uploaded to a repository (like an AWS S3 bucket or even an on-premises FTP site), it can trigger a Lambda function that will convert the file to a new video format. There’s no need to maintain and pay for an actual instance running 24/7, just for the moments your code is actually running. And there’s no administration overhead to worry about.