# AWS Certified Solutions Architect – Associate (2018) Study Notes

In order to prepare the **AWS Certified Solutions Architect – Associate Feb 2018 Exam**, I made a document with a summary with all the relevant information to study for the exam. The purpose is to share my notes taken while studying for the AWS CSA certification exam.

## Want to contribute?
The current document is far to be finalized. If you see something that is missing (networks, commands, tricks etc.), feel free to start there. Alternatively you can contribute with:

* Cleaning up code and making code more polish
* Giving better explanations
* Spelling/grammar mistakes
* Suggestions
* Anything else not listed here

## Commiting
All commits are welcome, even if they are minor ;)
If you are unfamiliar with Github, you can email me contributions to the <dicarlo.fabrizio@gmail.com> or [@fdicarlo]

[@fdicarlo]: https://twitter.com/fdicarlo.

## Exam Blueprint

[Official Blueprint ](https://d1.awsstatic.com/training-and-certification/docs-sa-assoc/AWS_Certified_Solutions_Architect_Associate_Feb_2018_%20Exam_Guide_v1.5.2.pdf)

| Domain | % of Examination|
|------------- |:-------------:|
| Domain 1: Design Resilient Architectures | 34% |
| Domain 2: Define Performant Architectures | 24% |
| Domain 3: Specify Secure Applications and Architectures | 26% |
| Domain 4: Design Cost-Optimized Architectures | 10% |
| Domain 5: Define Operationally Excellent Architectures | 6% |
| Total | 100%|

Where:

* **Domain 1: Design Resilient Architectures**
    * 1.1 Choose reliable/resilient storage.
    * 1.2 Determine how to design decoupling mechanisms using AWS services.
    * 1.3 Determine how to design a multi-tier architecture solution.
    * 1.4 Determine how to design high availability and/or fault tolerant architectures.
* **Domain 2: Define Performant Architectures**
    * 2.1 Choose performant storage and databases.
    * 2.2 Apply caching to improve performance.
    * 2.3 Design solutions for elasticity and scalability.
* **Domain 3: Specify Secure Applications and Architectures**
    * 3.1 Determine how to secure application tiers.
    * 3.2 Determine how to secure data.
    * 3.3 Define the networking infrastructure for a single VPC application.
* **Domain 4: Design Cost-Optimized Architectures**
    * 4.1 Determine how to design cost-optimized storage.
    * 4.2 Determine how to design cost-optimized compute.
* **Domain 5: Define Operationally-Excellent Architectures**
    * 5.1 Choose design features in solutions that enable operational excellence.

## Regions, Availability zones (AZs), Edge locations

* A **Region** is a physical location in the world which consists of two or more Availability Zones (AZs)

* An **AZ** is one or more discrete data centers, each with redundant power, networking and connectivity, housed in separate facilities. A datacenter is a location where actual physical data resides. A data center typically have 50000 to 80000 physical servers. A single or couple of data centers are clubbed in to one AZ.

* **Edge Locations** are endpoints for AWS which are used for caching content. Typically this consists of CloudFront (Amazon's Content Delivery Network (CDN)). An edge location is where end users access services located at AWS. They are located in most of the major cities around the world and are specifically used by CloudFront (CDN) to distribute content to end user to reduce latency. It is like frontend for the service we access which are located in AWS cloud.

The AWS Cloud infrastructure is built around Regions and Availability Zones (AZs). AWS Regions provide multiple, physically separated and isolated Availability Zones which are connected with low latency, high throughput, and highly redundant networking. These Availability Zones offer AWS customers an easier and more effective way to design and operate applications and databases, making them more highly available, fault tolerant, and scalable than traditional single datacenter infrastructures or multi-datacenter infrastructures. For customers who specifically need to replicate their data or applications over greater geographic distances, there are AWS Local Regions. An AWS Local Region is a single datacenter designed to complement an existing AWS Region. Like all AWS Regions, AWS Local Regions are completely isolated from other AWS Regions. The AWS Cloud spans 55 Availability Zones within 18 geographic Regions and one Local Region around the world.

![region](https://github.com/fdicarlo/aws-csa-2018/blob/master/images/AWS_region.png)
