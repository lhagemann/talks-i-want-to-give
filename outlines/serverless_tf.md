# Serverless Architecture with Terraform Outline

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

