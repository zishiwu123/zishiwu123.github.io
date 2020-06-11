---
layout: post
title: "Deploying a Machine Learning Project to AWS - Part 1"
date: 2020-06-10 09:41:00 -0000
categories: data-science
---
Recently, I figured out how to deploy a machine learning project written in
Python to an Amazon Web Service (AWS) EC2 instance. A member of the Real Python
community asked if I had created a tutorial on this. I thought it would be a
great idea to have a tutorial on this since this is something that students in
a statistics or machine learning class may have never done before. I have been
received so much help from the Real Python community and online tutorials that
I want to give back and share my knowledge.

I'm going to assume that readers of this tutorial have already created an AWS
account. When we login to AWS, the first thing we see is the AWS management
console. AWS provides many different services, but to keep things simple, we
will only use the EC2 service. For this tutorial, we will set up an EC2
instance that runs an Ubuntu 18.04 LTS server.

<!-- ![AWS Management Console]({{ site.url }}/assets/images/1-aws-console.png) -->
![AWS Management Console](/assets/images/1-aws-console.png)

Setup instructions are below.