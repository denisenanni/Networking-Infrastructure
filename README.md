# Networking-Infrastructure


## Cloud Formation
Tool in AWS for managing, configuring and deploying infrastructure (pushes code along with the necessary server configurations).
It uses a declarative language to deploy networking infrastructures using the AWS CLI. 
It allows you to model your entire infrastructure in a text file and provision AWS resources based on the scripts you write.
Templates are written using JSON or YAML.
A stack is a group of resources. These are the resources that you want to deploy, and that are specified in the YAML or JSON file.

## AWS Command Line Interface 

The AWS CLI allows you to access and control services running in your AWS account from the command line. To use the CLI, download, install, and configure it.

## How to run Cloud Formation

In the terminal, to use your yml code to request the resources, type the following in the same directory as your yml file:

```bash
aws cloudformation create-stack 
--stack-name YOUR_STACK_NAME<br>         --> name you want to give to your stack
--region us-west-2                       --> the region in which you want to deploy the infrastructure
--template-body your-file.yml            --> the file containing the script  
```

The infrastructure is graphically representerd in the .jpg file.


## Glossary

## Continuous Integration Continuous Deployment (CI/CD)
Tracks the development workflow from testing through production. Continuous integration is process flow of testing any change made to a development flow, while continuous deployment tracks those changes through to staging and production systems.

## Virtual Private Cloud (VPC)
A pool of networked cloud resources. It can span more than one availability zone. It is the smallest unit of resource.

## Subnets
A subnet is a subset of the overall VPC network and it only exists in a single availability zone, unlike its parent network, the VPC.
Subnets can be public or private. Public subnets are accessible to external users. Private subnets are only accessed internally by other resources within your cloud container. Routing rules are used to define access to all resources placed inside that subnet.

## Internet Gateway
An internet gateway is a resource that enables inbound and outbound traffic from the internet to your VPC (you won't need it for a private VPC).









