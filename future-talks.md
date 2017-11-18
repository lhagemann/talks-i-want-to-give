# Future talk ideas

Feedback welcome! Please open an issue or make a pull request.

## Deconstructing Terraform cidrsubnet function
Based on my blog post http://blog.itsjustcode.net/blog/2017/11/18/terraform-cidrsubnet-deconstructed/

This talk would be relatively technical discussing Cloud Platform Networking and subnets. Using examples of Terraform for defining Infrastructure as Code, and demonstrating using the builtin `cidrsubnet()` function to programatically define subnets. 

Potentail for expanding into other Terraform builtin functions.

### Abstract

A practical discussion around utilizing the Terraform tool from Hashicorp to define your cloud network infrastructure. Special attention is given to the useful but ambiguous built-in function `cidrsubnet()`. Using this function wisely allows us to build re-useable modules, abstracting the subnetwork management away from the compute instance provisioing. 


## Polychronic vs Monochronic culture and DevOps
* needs a title for sure
* A monochronic time system means that things are done one at a time and time is segmented into precise, small units. Under this system, time is scheduled, arranged and managed.
* A polychronic time system is a system where several things can be done at once, and wider view of time is exhibited and time is perceived in large fluid sections.
* how to corodinate time sensitive personalities with those who see time as a little more fluid
* take advantage of the strengths in each to build a better culture and produce more work
* build polychronic approach into Agile planning
* for polychronics the 'how it fits into the bigger picture' is more important than 'how long it takes (will take)' to get done.
	* what's the value

## Automating Your Way to the Cloud: Serverless Architecture with Terraform
* Infrastructure is code
* Terraform is multi-cloud enabled
* [New Terraform Oracle BMC provider](https://blogs.oracle.com/developers/terraform-and-oracle-bare-metal-cloud-services) released (not official)

### Abstract
There is no cloud, it's just someone else's computer.

With the industry move away from the datacenter to the cloud, costs, accessibility and speed are balanced against the loss of control, and the need to manage and orchestrate infrastructure in repeatable, automated and auditable manner.  

This presentation will share experiences and lessons learned developing a deployment strategy for a cloud-first service. Our goal: initial production deployment of a Serverless Architected service directly from our CI/CD pipeline, with no manual intervention in resource deployment. 

Through this talk attendees will be introduced to [Terraform](http://terraform.io), a tool that defines cloud infrastructure in configuration files that can be shared, edited, reviewed, and versioned. 

Using Jenkins as a build tool and Terraform modules for infrastructure codification, we are able to repeatedly build and destroy our service for testing purposes and ship updates through continuous deployment.

### Introduction
This presentation is intended for Beginner and Intermediate level software developers, and technical managers who are interested in speeding up the time to deployment for cloud based services. 

In the area of software automation, the mantra of Infrastructure is Code, is often spouted, but rarely followed. In this presentation I will walk through how a cloud-first service differs in deployment strategy from traditional deployments. 

With a Serverless Architecture, the testing and validation of code modifications in a CI/CD pipeline necessitate deploying a testbed infrastructure for automated testing prior to deploying changes into production. This differs from the usual functional test runs due to the need to deploy test-run specific infrastructure. As these are "one-use" resources, ensuring they are properly destroyed after test runs is a crucial part of controlling costs. Using an orchestration tool such as Terraform allows for automating these tasks. 

This presentation will include architecture considerations, deployment strategy and testing practices that support rapid iterations and fit into a Continuous Integration / Continuous Deployment pipeline strategy.

## Introducing Chat to the Enterprise
A culture and tooling talk. Many organizations have decades of reliance on email for communication. Even if these orgs have a long experience with distributed team locations, the synchronous nature of Chat is lost. It is sometimes hard for enterprise orgs to view Chat as a collaboration tool and not just an extension of Instant Messenger or text. 

We'll talk about some of things an individual contributor or a decision influencer can do to ease the transition to chat for Enterprise.

* Participation is crucial to buy in. If you are on the team that introduces Chat to an org, it is incumbent upon you to ensure the Chat system is active. 
* Cat Facts & Karma may be entertaining, but they do nothing to suggest to the enterprise that chat is a valid alternative to email for business communications
* `@here` and `@all` should be used sparingly. Turn them off in Org-wide channels. 
* Bring ChatOps out of the DevOps realm and into the more general channels  ... Food Truck bot, or Weather bot or "What's on Tap" bot, to get people used to the idea of using chat to query for common questions
* automated FAQ: Sick of answering the same question all the time? Trigger an auto response on the key phrase (or error message) which links to your wiki page with the answer



## Less fleshed out ideas

* The pain points if early adoption of immature tools
	* Oracle Cloud Infrastructure -- moving target
	* Terraform -- rapid feature modifications
	* No common patterns agreed upon by the community
* git training for the CLI impaired

