
#  CC Notes for MST
> Author : Aaron Augustine

> Star the gist so that I can get a consensus on how many people are using this resource

[Cloud Computing mcqs for CT](https://gist.github.com/GravenHawkX/330f5dcd1afb601b0a7647cac400db29)

## Week 1 
### Lecture 1 

> [Reference Link : Lec 1](https://archive.nptel.ac.in/courses/106/105/106105167/)

Q1. What are the different trends in computing? ==GDUCC==
Ans. There are 5 types of trends in Computing : 
1. Grid Computing
2. Distributed Computing
3. Cluster Computing
4. Utility Computing
5. Cloud Computing

<hr>


Q2. What are Distributed Applications?
Ans. 
* Appliccations that ==consist of a set of process that are distributed acrosss a network of computers== that work as an ensemble to solve a common problem
* Client- Server : ==Resource management is centralized to the server==
* Peer to peer computing : It represents a movement toward ==truly distributed applications==

<hr>



Q3. What are the different types of grids ? ==CDCNU==
Ans. There are 5 different types of drigs

1. Computational Grid : 
	*	Access to pool of processing power for computation intensive computing.
2. Data Grid : 
	* Infra to support *storage*, *discovery*, *handling*, *publication* and *manipulation* of data.
3. Collaboration Grid : 
	* Collaboration on different projects without revealing sensitive information.
4. Network Grid : 
	* Fault-tolerant and high performance comm^n^ services.
5. Utility Grid : 
	* Ultimate form. Data and computation cycles as well as software or any other resource is shared.

<hr>


Q4. What is Grid computing ?
Ans. 
* It is a form of networking.
* Uses the processing cycles of other computers, to solve problems too intensive for a single computer.
* It creates vast IT capabilities by combining various data resources from multiple computers on the network, such as processing, network bandwidth, and storage capacity.

<hr>


Q5. What is Cluster Computing ?
Ans 
* It is a type of parallel or dsitributed Computer system, where inter connected stand alone computers work together as  single computing unit.
* Key components are : ==computers, OS's, middleware, parallel programming env, and applications.==

<hr>


Q6. What are the components of a cluster ?
 Ans. 
 1. Cluster nodes
 2. Cluster Network
 3. Network Characterization

<hr>


Q7. Benefits of cluster computing ? ==SHOSH==
Ans. The benefits of cluster computing are as follows : 
* System Availability : high availability
* Hardware Fault Tolerance : Redundancy for h/w and s/w
* OS and application reliability : Run multiple copies
* Scalability : Adding servers
* High Performance : Running cluster enabled programs

<hr>


Q8. What is cloud computing ?
Ans. It is the delivery of ==on-demand services== over the internet on a ==pay-as-you-go basis==
* It refers to both the software application delivered as a service, as well as the hardware and system software in the data centers that provide these services
* It is a model for enabling ubiquitous, convenient, on-demand network access to a shared pool of configurable resources

<hr>


Q9. What are the key technologies in cloud computing ?
Ans The key technologies in cloud computing are : 
* Virtualization Technology
* Programming Model
* Data Management Technology
* Data Storage Technology

<hr>


Q10. What are the characteristics of Grid computing ?
Ans. 
1. They share more than information
2. Efficient use of resoures at many institutes
3. Join local communities, for research, etc
4. Interactions with underneath layers must be transparent and seamless;
Ex : Physics apps, reator apps, weather forecast, detection and modelling natural disasters, etc

<hr>


Q11 What are the different types of cloud service models ?
Ans. There are 3 types of cloud service models : 
* IaaS : 
	* Infrastructure as a service provides processing, storage, networks and other computing resources. 
	* The customer can deploy and run arbitary software
* SaaS : 
	* The customer is able to use applications running on the cloud infrastructure.
	* These applications are accessible through web browsers, etc
	* Ex : Google spreadsheet ( data is stored on the cloud and not your local device )
* PaaS : 
	* The capability provided to the consumer is to deploy onto cloud infra using programming languages, libraries, etc.

<hr>



Q11. What are the different types of cloud ?
Ans There are 4 different types of cloud : 
1. Private Cloud : Solely for an organization
2. Community Cloud : Shared by multiple organizations
3. Public Cloud : Made for the general public
4. Hybrid Cloud : Composition of two or more clouds

<hr>


Q12. What are the various advantages of virtual machines ?
Ans. The advantages of virtual machines are : 
* Run OS's where hardware is unavailable
* Easier to create new machines
* Software tesitng can be done
* Emulate more machines than physically available
* Run legacy systems
* Debug problems

<hr>


Q13. Difference between Vertical scaling (up) vs Horizontal scaling (out) ?
Ans.
| Vertical Scaling (Up) | Horizontal Scaling (Out) |
|--|--|
|Add more resources to a computation unit | Adding more computational units |
|Move workload to a computation unit with more resources | Splitting workload across multiple computation units |
|--|Database partitioning|
|For smaller scenarios scale up is cheaper|For larger scenarios scale out is the only solution|

<hr>


Q14. What is IaaS?
Ans. 


<hr>


Q15. What is a client server architecture ?
Ans. We have a server and several clients connecting to the server. The server is continually listening on a port. If a client needs the server, it hooks into the port and gets the service.
* Consists of one or more load balanced servers servicing requests sent by clients
* Exchange of messages in ==request-response== fashion
* Client is a often thin ( mobile, laptop, etc ) with low computational capabilities
* Server could bea  load balanced cluster or a standalone machine

<hr>


Q16. What is XaaS?
Ans The combination of service oriented infrastructure and cc realizes XaaS
* X as a service is generalization for cloud related services
* XaaS stands for "everything as a service"
* It refers to an increasing number of services provided over the internet than locally
* It is the essence of CC
Ex : SEaaS ( Security ), DaaS ( Database ), MaaS ( Management ), IaaS( Identity ), BaaS ( Backup ), BPaaS ( Business Process )

<hr>


Q17. What is SaaS ? 
Ans Software as a service ==Characteristics==
* Web access to commercial software
* Software that is deployed on cloud infrastructure is made available to customers
* Users don't have to handle software upgrades
* API's allow the integration of various pieces of software
* Software is in a one-to-many model

Application of SaaS : 
* Communication of organization with outside world ( email, newsletter, campaign software, etc )
* Need for mobile or web access ( mobile sales management software, exam software, CRM software, etc )

<hr>


Q18. What is PaaS?
Ans. It can be defined as  a computing platform that allows the creation of web applications, without needing to maintain the s/w or h/w infrastructure underneath it.
Characteristics of PaaS : 
* Services to develop, test, deploy, host and maintain applications
* Web based UI creation tools help you 

<hr>


Q19. What is virtualization ?
Ans.  Virtualization refers to the act of creatinga  virtual rather than an actual version of something, incluing a computer hardware platform, OS, storage device or network resources.

<hr>


Q20. What are the different type sof virtualization ?
Ans There are 5 different types of virtualziation.
* Software : 
	* This includes OS level virt, Application Virt, Service Virt
* Memory : 
	* Memory virtualization , aggregating ram from different pc's to a single memory pool
	* Virtual memory, giving an application the impression that it has contiguous working meory
* Storage : 
	* Storage virt, is abstracting logical memory from physical memory
	* Distributed file system
	* Virtual File system
	* Virtual disk drive
* Data : 
	* Data Virt, the presentation of data as an abstract layer
* Network : 
	* Network virt, is creation of a virtualized network addressing space within or accross network subnets.
	* VPN

<hr>

Q21 What are the 3 types of server virtualization ?
Ans. The 3 types are : 
* Full virt
	* Uses a special software : Hypervisor
	* It interacts directly with the physical servers CPU and disk space
	* Keeps each virtual server completely independent of the other virtual servers
* Para Virt : 
	* Unlike full virt, guests systems are aware of each other.
	* The hypervisor herer doesn't need as much processing power to manage the guest OS's
* OS-level virt
	* Doesn't use a hypervisor at all, the virtualization capability is part of the Host OS.
	* All the Guest OS's must be the same
* They all share a few common traits
	* The physical server is the host
	* The virtual servers are guests
	* These virt servers behave like physical machines

<hr>

Q. What is XML ? 
Ans. 
* XML is a markup language used to provide information about a document
* Tags are used to give extra info
* HTML tags tell the browser how to display the doc
* XML tags give the reader an idea of what the data means
* It is basically a meta language that allows you to create and format your own tags
* It allows you to put structured data into a file which is :
	* Unambiguous
	* Extensible
	* Platform Independent
	* Easy to Read
* They are used to transfer data from one place to another on the internet

<hr>

Q. What are the advantages of XML ?
Ans.

<hr>

Q. What are the differences between HTML and XML ?
Ans. 
**![](https://lh7-us.googleusercontent.com/yNlOt4sPeEIhId_DuWKJs1h8fjeEUwRaIA8Eyha0F7kjCiX633mtD_AWZCbofPtwXorYM3rDjg-fPLOxESza2xE9uyn-yVlTofe4ifTVXGIbj-0f8Mddd6vVvNsZZksardpDwTBtmCjLWvH9bgavi5I)**

<hr>

Q. What is XML DOM ?
Ans. It is : 
* A standard Object Model for XML
* A strandard programming Interface for XML
* It is platform and language independent
* It ==defines== the ==objects and properties== of all ==XML elements==, and the methods ( interface ) to access them.
* The ==XML DOM== is a standard for how to ==get, change, add or delete== ==XML elements==. 

Advantages : 
* It is platform and language independent
* It is traversible
* It is modifiable

Disadvantages : 
* It consumes more memory if the document structure is large/
* The size affects the operational speed

<hr>

Q.What is JDOM ?
Ans. JDOM or Java Document Object Model is a way to represent an XML document for easy and efficient reading, manipulation and writing.
* Straighforward API
* Lightweight and fast
* Java-optimized

Isn't built on DOM or modeled after DOM
It is an opern source project with Apache-style license
<hr>


Q. What are Web Services ?
Ans. Web services are an XML based phenomena
* They are those services which can be defined and accessed through a standard URI ==( Uniform Resource Identifier )== 
* Works on message exchange protocol which is based on XML
* Take advantage of OOP. Allow developers to build apps from existing software components.
* Communicate via open protocols ( ==HTTP, SMTP==)
* Describes it's messages using XML schema.
* Provide capabilities similar to EDI and are cheaper to implement

XML
* XML is a data transformation language
* It allows for interoperability and helps in applications talking to each other.

<hr>

Q. What is EDI?
Ans. EDI or ==Electronic Data Interchange== : 
* It is a computer to ==computer exchange of business data and documents== b/w companies, using standardized formats.
* ==Business data== comprises of all the information related to a company, such as ==sales data==, ==customer contact info== and ==website traffic stats==.

An example of business data would be :
When you visit a website. what you look at, what colors you prefer and even how long you stay on the website, is captured.


<hr>

Q What is Service Oriented Architecture ?
Ans. IBM made a model to show ==web services interaction==, which consists of relationships between ==3 entities==  :
* **Service Registry/Broker** : Gives support for publishing and Locating services
* **Service Provider** : Provides e-business services or web services
* **Service Requestor** : Finds required services via the service broker

==SOA== is also a generic model describing ==service collaboration==, not specific to web services 

Operations in web service architecture / SOA : 
* **Publish** : Service descriptions need to be published for the service requestor to find them
* **Find** : Service requestor retrieves a service description or queries the service registry to find the required service.
* **Bind** : Service requestor invokes or initiates an interaction with the service.


<hr>

Q. What is SOAP ? What are it's building blocks ?
Ans. Simple Object Access Protocol is basically a ==format for sending messages over the internet, b/w programs==.
* It is ==XML based==, and platform independent
* Simple and extensible
* Uses mainly ==HTTP== ( Contains SOAP message as payload )
* Stateless and one-way

Soap Building blocks are : 
* **Envelope** : Identifies XML doc as SOAP message
* **Header** 
* **Body** : call and response info
* **Fault** : errors that occur while processing message.

<hr>

Q. What is WSDL and what is the WSDL Document structure ?
Ans. Web Service Description Language is the XML vocab standard for defining web services and their capabilities
* Specifies what a request message must contain, and what a response message must look like
* Defines where the service is available and what comm protocol is used to talk to the service.

WSDL Document Structure : 
It is just a simple XML document : 
* **Port Type** : The operations performed by the web service.
* **Message** : The messages used by the web service
* **Types** : The data types used by the web service
* **Binding** : The comm protocols used by the web service

<hr>

Q. What is UDDI ? 
Ans Universal Description, Discover and Integration is a registry service, which contains metadata information.
* It is a framework used to define XML based registries
* Registries -> Repos -> Documents -> Business data
* Business publish info about the services they offer and about themselves
* **Service Registry/Broker** : Gives support for publishing and Locating services
* **Service Provider** : Provides e-business services or web services
* **Service Requestor** : Finds required services via the service broker

**![](https://lh7-us.googleusercontent.com/tYSpq1wl2u2zNol8YMFR24mtYZ7NiBzL0JKJw-uFXDZe_pxOi7p7WKKmMcBxNShBuX9v6zf5sVf8RAq7yzAABbCFsf9KTIrBlxx714WVsMeMkAe8IO0uFI-Y7FbplQ8mm2JVmFLpOz5U9hbFLTb68mk)**

<hr>

Q. What is Open Stack ?
Ans. Open Stack is a cloud OS , that controls large pools of computing, storage and networking resources.
* It uses a dashboard to give admins control.
* It empowers users to provision resources through a web interface.

OpenStack capabilities are as follows : 
* SaaS : Browser or thin client access
* PaaS : On ton of IaaS ( Cloud foundry )
* IaaS : Provision compute, network and storage
* Network
* Storage for VM's
* Multi-tenancy :
	* Users can be associated with multiple projects
	* These multiple users may need to use a single software, hence the need for multi-tenancy



**![](https://lh7-us.googleusercontent.com/JUmLRUA1XeBWvIg2wc3xarB4lzMgJOV7Hwr8RUWOYnLo0snBSMhNmauYVWLYmwKf-ajkAnDz9gm1oRWadxvKd8rkW2rLIgXd8SFZ8EDpN8Cbhmi-EYp_U5WcO6h7vbCkq-OXhqxe_q_jLi2oW77vGas)**

## Distributed Computing
Use of distributed systems to solve computational problems.
Ex. Internet, ATM machines, Intranets.

### Computers in a Distributed computing system
* **Workstations** : Used by end users
* **Server systems** : Provide resources and services
*  **Personal Assistance Devices** : Handheld computers connected via wifi

### Properties of Distributed Computing ~FERLEP~
* Fault Tolerance
* Each node plays a partial role
* Resource sharing
* Load sharing
* Easy to expand
* Performance

### Advantages of Distributed Computing
* Nature of application
* Performance
	* Computing Intensive
	* Data Intensive
* Robustness 
	* No single point of failure


## Grid Computing
"The grid" links together computing resources and provides the mechanism needed toa ccess them

### Uses of grid computing
**![](https://lh7-us.googleusercontent.com/z6jaASMPcqjVXSg0R4J9LfiJS7pIq82BsTDFx3GlujOivL9XX6k2X-SCYmUazGooZ8p82JsdRQTcOi-qdQOIxchAC6E4O-vCsHdoN7kosv17pHyndCvGWaVGsZ9-Sgw82WWW8wwSly0D7RzULMZbTB8)**



### Grid components : 
* **Users** 
* **Groups**
* **Sites**
<hr>

## Cluster Computing 

Consists of a collection of inter connected stand-alone computers working together as  single integrated computing resource


### Components of Cluster Computing 
* **PCs, Workstations, SMPs**
* **Operating systems**
* **Middleware**
* **Parallel programming environments**
* **Applications**

### Key operational benefits of clustering ~SHOSH~
* **System Availability** : Offer inherent high sustem availbility due to redundancy of hardware.
* **Hardware Fault Tolerance** : Redundancy for most system components , including both hardware and software.
* **OS and App Reliability** : Run multiple copies of the OS and apps.
* **Scalability** : Adding servers to the cluster or adding more clusters to the network.
* **High Performace** : Running cluster enabled programs

<hr> 

## Utility Computing
It is a service provisioning model in which a service provider makes computing resources and infrastructure management available to the customer as needed and charges them for specific usage, rather than a flat rate.
> It's concept is a pay-per-use model.


### Main properties of utility computing 
1. Pay-for-user pricing business model
2. Data center virtualization and provisioning
3. Solves resource utilization problem
4. Outsourcing
5. Web services Delivery
6. Automation

## Risks of Utility Computing
* Data Backup
* Data Security
* Partner Competency
* Defining SLA
* Getting value from chargeback

<hr>

## Cloud Computing
*It is a model for enabling ubiquitous, convenient, on-demand network access to a shared pool of configurable resources.*


### Essential characteristics of Cloud computing : 
* On-demand self-service :
	* A consumer can unilaterally provision computing capabilities, such as server time and network storage, as needed automatically without requiring human interaction.
* Broad Network access : 
	* All the services provided are available over the network and accessed through standard mechanisms that promote use by heterogeneous thin or thick client platforms ( Mobile phones, laptops, tablets, etc )
* Resource Pooling
	* The providers computing resources are pooled to serve multiple consumers, with different physical and virtual resources dynamically assigned and reassigned according to consumer demand.

### Cloud Service Models
**![](https://lh7-us.googleusercontent.com/E3Adbh1MOLwuOWVoRXj63VBJhlvOJ2B6RSLtFUgpWjUUdSnqk_w_1ThltCfqtvZlsBa_SxL9MQxcEjMeRmvqLlGI9UOI_YbW1LVvAdAiZDz2YWzMcASlI4hfFSPFS-dss-FlHH3d468OpFtin5wpogc)**







