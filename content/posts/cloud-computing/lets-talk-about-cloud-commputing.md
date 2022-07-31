---
title: "Let's talk about cloud computing!"
date: 2022-07-31T01:27:04+05:30
draft: false
---


---
Hello reader! There is a new type of cloud in our world now. 
This cloud serves the software industry, is expected to never rain, never exhaust itself.

![Cloud computers](/posts/cloud-computing/images/funny-cloud.png)

Before you get stuck like the pilot above, let's collect some information on the `what, why, and how to build or use this cloud?`

---

## Progress in software usage

**Unprecedented!**

Think about the number of computers in the year 2000 to the year 2022.
It has increased manifolds. 
From one computer in some offices to laptops, smart devices used by every individual. 
Now, there are server farms across the world like agricultural farms.

**Software development is one of the main pillars of this development.** 
People have built applications to solve issues in every walk of human life.

Online retail, travel, food, education, banking, law, research, entertainment, content creation, animation, social media, information, business insights to automated software development itself, machine learning, artificial intelligence and the list goes on... 

> This high level of software acceptability is possible due to 
> - software ease of use
> - performance and speed
> - fast upcoming features
> 
> All of this is backed by readily available compute power, cheap storage system and faster software development lifecycle.
---

## Towards cloud computing

*Consider banking as an example.*

Traditionally, in the **no-computer era**, there used to be staff who maintained people's accounts and transactions on paper. 
The account usage was limited to the speed of bank staff and bank's geographical location.
Think about the time, where to withdraw any amount, one need to visit the specific branch and do the transaction.

Some companies understood this problem, **built banking software** and sold it to the banks. 
Banks bought the software license.

**Setup in house server rooms**, hired IT staff to make all this operational.

Over time, the **bank's need increased** to the extent that there are millions more accounts and unlimited transactions at any instant. 
With online payment systems like Paytm, PhonePe, the banks now need to support transactions anytime, anywhere.
   
To perform transactions and maintain consistency, obviously there are software improvements, 
but the **hardware requirements are equally big now!**

> Where and how an international bank will maintain its customer data and 
> serve requests from any part of the world with similar latency, be it in India or America.

The same goes for any other platform today, 
eg: watching content on YouTube or Netflix, it does not matter where the video is stored, 
the download speed cannot go beyond a certain limit that the user goes away.

---
### Why cloud?
Most businesses today need similar growth, that is:
1. `Faster SDLC` - Fast for them to build software without worrying about buying and setting up their own infrastructure. Use ready made solutions.
2. `Low operational cost` - Avoid capital expense of setting up an on premise data center.
3. `High scalability` - To span across the world.
4. `High performance, low latency` - Consistent Service level Agreement like 30 seconds response time for a web request anywhere.
5. `Reliability` - During system failure, software failures and disasters in a region.


These requirements are extremely hard to be fulfilled by an in-house server room.
Companies need their hardware to be set up and located geographically. 
This is the problem solved by **Cloud Computing.**

> [Cloud Computing](https://en.wikipedia.org/wiki/Cloud_computing)
> 
> The on-demand availability of computer system resources, especially data storage (cloud storage) and computing power, 
> without direct active management by the user.
> Clouds have resources distributed over multiple locations, each location being a **data center**.
> Consumers share resources to save cost.


Geographical coverage of AWS, Azure and Google Cloud from a [source](https://www.atomia.com/2016/11/24/comparing-the-geographical-coverage-of-aws-azure-and-google-cloud/
):
![Data Cenetrs of AWS, Azure and Google Cloud](/posts/cloud-computing/images/datacenters.png)

---


## Cloud providers

Cloud actually is one of the software products. 

It is a platform that allows other applications to run on top of it. 
There are multiple companies who offer cloud services. 

As per [Dgtl Infra reports](https://dgtlinfra.com/top-10-cloud-service-providers-2022/#:~:text=As%20a%20whole%2C%20the%20top,Linode%20(owned%20by%20Akamai)), 
top global cloud service providers in 2022 are:

1. Amazon Web Services (AWS)
2. Microsoft Azure
3. Google Cloud Platform (GCP)
4. Alibaba CLoud
5. Oracle Cloud Infrastructure (OCI)

![Top 10 cloud providers](/posts/cloud-computing/images/providers.png)

### Types of cloud services
The services offered by cloud providers are largely classified into:

1. `Infrastructure as a Service (IaaS)`
    - Basic infrastructure like servers and virtual machines (VMs), storage, networks, operating systems provided from a cloud provider on a pay-as-you-go basis.
    - Eg: Amazon EC2 and S3, Google Compute Engine, Oracle object Storage.


2. `Platform as a Service (PaaS)`
    - An on-demand environment for developing, testing, delivering and managing software applications.
    - Eg: Google Kubernetes Engine that provides Kubernetes as a platform to build microservices, Google App Engine, Heroku.


3. `Serverless`
    - An event driven architecture where you build your application and give it to the cloud provider. When a request comes, this event is responded to by setting up the server machine, deploying the application on it, processing the request, responding and shutting down the server.
    - Resources are only used when needed, not always running. Saves money.
    - Eg: AWS Lambda function, OCI Data Flow, Functions.


4. `Software as a Service (SaaS)`
    - Delivering software applications for direct or customized usage, on demand, on a subscription basis.
    - Eg: Salesforce (CRM), Zoom (meetings app), Shopify (CMS)

Considering different needs of a software to become operational, like networking, storage, data, applications on y-axis, 
below is a diagram from [IBM article](https://www.ibm.com/cloud/learn/paas) illustrating who manages what?

![Managed cloud services](/posts/cloud-computing/images/services.png)

---


## Cloud consumers

The software companies who use the cloud services to build or/and deploy their applications. 
There may be companies who migrate their old applications to cloud or 
companies who are new and start with building [cloud native applications.](https://www.redhat.com/en/topics/cloud-native-apps)

### Types of cloud computing
For the consumers' usage, cloud is available in four forms:
1. `Commercial or Public cloud`
    - Cloud resources hosted publicly over the internet.
    - Shared between consumers.  
    - Owned by the cloud company. Provided by almost all providers.

2. `Dedicated or Private Cloud`
    - Cloud resources maintained on a private network.
    - Used exclusively by a single consumer.
    - May be located on the consumer's on-site datacenter.
    - Eg: [OCI DRCC](https://www.oracle.com/in/cloud/cloud-at-customer/dedicated-region/), Azure Private Cloud.

3. `Hybrid Cloud`
    - Consumers use both public and private clouds offered by one provider.
    - Data and applications move between them.

4. `Multi Cloud`
    - Consumers use cloud services of two or more providers together.
    - Eg: [OCI-Azure Interconnect](https://www.oracle.com/in/cloud/azure/interconnect/), which provides Oracle DB capabilities with operability in Azure cloud.

---
### Onboard applications to cloud
The steps of on-boarding an application to cloud in general are as follows:
1. Based on application system design, get the resource requirements. 
   Eg: VMs, DBs, Cache, LBs, Vaults etc.
2. Estimate the resource usage for a duration. 
   Eg: DB size growth in a month, writes per second etc.
3. Calculate the approximate usage cost with the help of cloud provider's estimation tool. 
   Eg: [AWS pricing calculator](https://calculator.aws/#/)
4. Discuss non-functional features provided by cloud, like security, auditing, monitoring etc.
5. Compare cost and features between different providers. Select one.
    - This step is big and involves lots of discussion.
    - Sometimes businesses reach out and ask many cloud vendors to submit proposals and estimates. 
    - And a bid is done to get the contract.
6. Start with subscription, account creation and development.
---


## Career in cloud computing

> There are two broad categories:
> 1. Developer in cloud provider company: Build & deploy cloud services, onboard consumers, support product.
> 2. Developer in cloud consumer company: Understand the business domain. Build cloud native applications.


The fundamental skills required in both are:
1. **Programming skills**
   - Some common languages are Java, [Python](https://docs.python.org/3/tutorial/).
   - Data Structures, algorithms. Practice problems on Hackerrank, LeetCode etc.
   - Clean code practices, OOPs etc.
   

2. **Application development skills.**
   - Backend, Frontend, SQL Database.
   - Eg: in Java Spring boot and Hibernate are famous, or NodeJs backend.
   - For experienced people, 
     - *Microservices architecture and REST based Apis design.*
     - *NoSQL DBs* 


3. **Containerization and orchestration.**
   - An overview is enough for freshers.
   - [Docker](https://www.udemy.com/course/learn-docker/)
   - [Kubernetes](https://kubernetes.io/docs/concepts/overview/what-is-kubernetes/)


>Below ones are must have skills for **experienced candidates**:

4. **CI/CD.**
   - Build and deploy process, build tools like Maven, SBT etc.
   - Build pipelines, Jenkins, Teamcity.
   - Infrastructure as code, eg: Terraform.

5. **System design**
   - Load balancers, CDNs, Database (SQL, NoSQL), Cache, Query optimization.
   - Think on how to scale the system as load grows. Backup, reliability, low latency etc.
   - Refer [System Design Primer](https://github.com/donnemartin/system-design-primer)
   
6.  **Prior cloud knowledge**
      - Basic 101 of AWS or Azure, etc.
      - Cloud certifications based on role:
        [AWS certifications](https://aws.amazon.com/certification/), 
        [Azure certifications](https://docs.microsoft.com/en-us/certifications/browse/), 
        [OCI certifications](https://education.oracle.com/oracle-certification-path/pPillar_640).
     
7. **Expertise experience**
   - This is based on special requirements in both provider and consumer companies.
   - Eg: if you are applying for a developer in Big Data cloud services, there is expectation to know about basic Big Data technologies, like Hadoop, Spark.
   - Similarly, if you're building an AI system for a consumer, you should have some prior knowledge.


> Talking from the point of view of interviews, I have seen following rounds:
> 
> - Coding
> - Project discussion
> - System design 
>     - For freshers, this includes computer science core subjects. like Database, SQL queries, OS or some basic application design like ticketing system.
> - Specific area of expertise based on role requirements, like AI, Data Science.
>     - For freshers, optional or interest based.
> - Human resource

---

## My experience

I started working in 2016 with [ThoughtWorks Technologies](https://www.thoughtworks.com/) as a software engineer.

My first company training included Git, Jenkins, Junit, Java, OOPs, and clean code practices, Spring Boot and Hibernate. 
This all is basic for building a Java based backend system, deployable in production.

I worked on 4-5 projects in ThoughtWorks and got exposed to Data Engineering skills, like Hadoop, Hive, Spark, AWS and azure based Data Lake and data pipelines.
Finally, in 2020, I was promoted as a Data Engineer based on my project performance.

In 2021, I joined [Oracle Cloud Infrastructure](https://www.oracle.com/in/cloud/) as a Senior Software Engineer for [OCI Data Flow service](https://www.oracle.com/in/big-data/data-flow/), to gain an understanding of building cloud scale products.

> [Apache Spark](https://spark.apache.org/) is a distributed processing engine for large scale data analytics. 
Any spark job execution requires cluster deployment. 
OCI Data Flow is a fully-managed serverless Spark service, where the application creates VMs, 
sets up Spark cluster and executes customer job on demand.

---

#### References
- https://azure.microsoft.com/en-in/resources/cloud-computing-dictionary/what-is-cloud-computing/#cloud-computing-models
- https://www.atomia.com/2016/11/24/comparing-the-geographical-coverage-of-aws-azure-and-google-cloud/
- https://aws.amazon.com/government-education/cloud-101/
