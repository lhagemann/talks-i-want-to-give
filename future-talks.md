# Future talk ideas

Feedback welcome! Please open an issue or make a pull request.

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

### Outline for GHC 2017 Software Engineering Foundations focus tract
1. Introduction
2. The Cloud -- it disappears
3. Problem ... deploy into the cloud in a repeatable manner
	a. Differences from a traditional DataCenter deployment
	b. Serverless Architecture, what it is and how we used it.
4. Infrastructure as Code
  a. Repeatability
  b. Audit Trail for Changes
  c. Incorporate into CI/CD pipeline
5. Terraform Introduction
6. Terraform State files
	a. What they are
	b. When they are used
	c. Remote state storage in multi-user environments
7. How We utilized Terraform and Docker in Jenkins to solve our automated deployment challenge
	a. Why Docker?
	b. Jenkins Build pipeline

### Outline for "How To"
1. Introduction
2. Infrastructure as Code
  a. Repeatability
  b. Audit Trail for Changes
  c. Incorporate into CI/CD pipeline
3. If It's Serverless, why are we deploying like we do servers?
	a. Consistent set of tools between environments
	b. It's what we'v got
	c. Known working model
4. The Cloud -- it disappears
5. Terraform Introduction
6. Terraform Examples of Cloud Infrastructure Definitions
	a. AWS
	b. Oracle Bare Metal Cloud
7. Terraform Example of infrastructure management
	a. plan
	b. apply
	c. destroy
8. Adding Terraform Infrastructure to a build pipeline
	a. Jenkins as build tool for CI/CD
		* Why using Docker containers in Jenkins works better than installing tools directly
	b. Using Terraform Docker Image in Jenkins build job
9. Deploying the Lambda Functions themselves
10. Topics we didn't have time for
	a. Multi-cloud deployments
	b. monitoring
	c. self-healing cloud infrastructure

## Introducing Chat to the Enterprise
A culture and tooling talk. Many organizations have decades of reliance on email for communication. Even if these orgs have a long experience with distributed team locations, the synchronous nature of Chat is lost. It is sometimes hard for enterprise orgs to view Chat as a collaboration tool and not just an extension of Instant Messenger or text. 

We'll talk about some of things an individual contributor or a decision influencer can do to ease the transition to chat for Enterprise.

* Participation is crucial to buy in. If you are on the team that introduces Chat to an org, it is incumbent upon you to ensure the Chat system is active. 
* Cat Facts & Karma may be entertaining, but they do nothing to suggest to the enterprise that chat is a valid alternative to email for business communications
* `@here` and `@all` should be used sparingly. Turn them off in Org-wide channels. 
* Bring ChatOps out of the DevOps realm and into the more general channels  ... Food Truck bot, or Weather bot or "What's on Tap" bot, to get people used to the idea of using chat to query for common questions
* automated FAQ: Sick of answering the same question all the time? Trigger an auto response on the key phrase (or error message) which links to your wiki page with the answer


## Infrastructure As Code: What is it good for?
We hear about Infrastructure as Code all the time. We've been hearing about it nearly since the advent of configuration management. As the tooling around automating your infrastructure deployments gain popularity, are we hitting some of the same problems we saw with configuration management? We have this one tool, so is everything a nail?

In this talk I will discuss the difference between Configuration Management and Infrastructure as Code; What advantages you have with Infrastructure as code and when perhaps Infrastructure as Code won't work for you. We will discuss and maybe debate(?) what constitutes Infrastructure, and how you want to manage these maybe not so obvious bits of your infrastructure.

* quiver of tools
* cron jobs
* DNS
* monitoring


## Less fleshed out ideas

* git training for the CLI impaired

