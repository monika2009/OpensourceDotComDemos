<style type="text/css">
  body{
  font-size: 10pt;
  font-family: Arial, Helvetica, sans-serif;
  text-align: justify;
  text-justify: inter-word;
}
table, th, td {
  border: 1px solid black;
  text-align: left;
}
</style> 

![Screenshot from 2021-06-21 21-08-13](https://user-images.githubusercontent.com/67622286/120605829-261ed900-c46c-11eb-8e9c-899a4fb6351c.png)


# 𝗡𝗜𝗖 𝗖𝗹𝗼𝘂𝗱 𝗗𝗲𝘃𝗢𝗽𝘀 𝗣𝗹𝗮𝘁𝗳𝗼𝗿𝗺


<!--**NIC DevOps Platform** is a container management platform built for organizations that deploy containers  based applications in production environments. For understand the NIC DevOps Platform go through with below sections--->

| Name | Description |
| ----------- | :----------------------------------------- |
| [**Overview**](#overview) | Introduction of CaaS platform in NIC DevOps and its offerings |
| [**Introduction to CaaS**](#introduction-to-caas) | This section provides a brief introduction of the Caas platform and its components such as Container/ Docker & Kubernetes which are the underlying technologies to support devops |
| [**DevOps Architecture**](#devops-architecture) | This section helps users to understand how the two fundamental technologies, Docker and Kubernetes compliment each other in making the DevopS architecture |
| [**Devops Platform Components**](#devops-platform-components)| This section explains how each DevOps Platform’s  softwares runs on the NIC DevOps Platform Servers that are used to manage the entire deployment |
| [**Using the NIC DevOps Platform**](#using-the-nic-devops-platform)| Provides the procedures for using the NIC DevOps Platform which requires onboarding & Various operations and Workflows |
| [**1. NIC Onboarding Procedure**](#nic-onboarding-procedure) | NIC Onboarding steps for using the CaaS on NIC DevOps Platform |
| [**2. Operating NIC DevOps Platform**](#operating-nic-devops-platform) | This section explains how to deploy a sample application using NIC DevOps Platform |

<div style="page-break-after: always"></div>

## **Overview**

NIC DevOps Platform is a container management platform built for various Indian government’s organizations that deploy containers based applications in production environments. Containerisation helps developers create applications faster and orchestrate the entire development cycle in the agile manner and combines development and IT operations through a practice popularly known as DevOps. DevOps facilitate modern application development, testing and packaging. NIC’s DevOps platform is the underlying IT infrastructure that is made up of many other software technologies such as Docker/container, Kubernetes  which provides a service for containerized workloads and is known as CaaS i.e. container as a service. Following sections provide a detailed description of each technology and procedures to use the DevOps platforms.


**Why DevOps**

DevOps is like a culture when adopted has proven to increase the speed and quality of software delivery as well as better teamwork and efficiency across multiple teams. DevOps removes silos of communication and improves collaboration. Adoption of DevOps has improved the progress of software delivery through **CI/CD**, reliability and removes gaps and mistakes that can considerably delay the software release.

<img src="https://user-images.githubusercontent.com/67622286/126584545-23458724-f99a-44ee-aeb2-bce18112ac31.png" width=650 height=350>

> CaaS is a requirement for the successful adoption of DevOps

<div style="page-break-after: always"></div>

## **Introduction to CaaS**

Container as a Service (CaaS) is a cloud based service model that allows users to provision and manage containers. CaaS provides the necessary framework and orchestration that facilitates the containerised application development, security and scalability for cloud native applications.

<img src="https://user-images.githubusercontent.com/67622286/126586126-31f194f4-daf9-47b7-aef4-175d29cb5579.png" width=650 height=400>

**Benefits of CaaS**

- CaaS provides on-demand containers that provide the ability to package and run an application in a loosely isolated environment.
- Containerization helps customers or clients release software faster and promotes portability between hybrid and multi cloud environments, and reduces infrastructure, software licensing and operating costs.
- The container helps in distributing and testing your application.
- Containers are great for continuous integration and continuous delivery (CI/CD) workflows that provide agility to your development environment. 
- Being lightweight, Containers provide the ability to run more workloads on the same hardware without much additional overhead hence are more cost-effective.

NIC CaaS is a Container as a Service platform built for government organizations that deploy containers based applications in production. CaaS gives its users a secure, scalable containerised environment to deploy applications through NIC Cloud. The CaaS services model allows users to quickly deploy, start-stop applications instances through NIC Cloud DevOps Platform’s.

<div style="page-break-after: always"></div>

### **NIC CaaS Current Offering**

1. **Container as a  Services** - NIC CaaS is a highly securable, scalable container orchestration service that supports Docker containers that allows users to  easily run and scale containerised applications through NIC Cloud. 
2. **External Endpoints** - External Endpoints provide connectivity between users applications running on NIC CaaS & external servers/Systems like Database, SMTP, SMS Gateways servers for external access.
3. **Container Additional Items** - NIC CaaS provides a container Additional items in which users easily run and scale containerised applications through NIC Cloud. 

Before we dive into the NIC CaaS platform, it will be quite informative for you to know the core components and technologies that makes the NIC’s CaaS a cutting edge and modern DevOps Platform. While dealing with <a href="Container1.pdf">Container</a>, we will hear two popular technologies, <a href="Container1.pdf">Docker</a> and the <a href="Container1.md">Kubernetes</a>. 

<!--#### A brief introduction to container   
 
A container is a standard unit of software that packages up code and all its dependencies so the application can be ported from one computing environment to another where it can run quickly and reliably. Docker is the most popular container runtime. Docker packages(containerize) your application and all its dependencies together in the form of a docker container image that is portable and works seamlessly in any environment that supports docker containers.

Containers are supported in Linux, Windows, and other modern operating systems. A container can run  anything from small software or a micro service to large applications. 

#### What is Kubernetes

Kubernetes, popularly known as K8s, is an open-source system for automating deployment, scaling, and management of containerized applications. Kubernetes distributes containerized applications across a cluster of machines. Kubernetes adds distributed computing features on top of containers such as load balancing, autoscaling, self-healing, rollout and roll back features etc. 

#### Docker and kubernetes are related

**How Dockers helps**

- Docker provides the ability to package and run an application in a loosely isolated environment called a container.

- The isolation and security allow you to run many containers simultaneously on a given host.

- Docker provides tooling and a platform to manage the lifecycle of your containers.

- Containerised application facilitates fast, consistent delivery of your applications.

- Docker’s container-based platform allows for highly portable workloads.

- Docker helps in dynamically managing workloads, scaling up or tearing down applications and services as business needs dictate, in near real time.

- In the long run, docker provides a viable, cost-effective alternative to hypervisor-based virtual machines, so you can use more of your compute capacity to achieve your business goals.

**How Kubernetes helps**

K8s helps in managing containerized workloads and services, which facilitates both declarative configuration and automation. It provides features that facilitate agile, continuous development, integration and delivery. The K8skey features are:

- **Service discovery and load balancing**: Kubernetes can expose a container using the DNS name or using their own IP address. If traffic to a container is high, Kubernetes is able to load balance and distribute the network traffic so that the deployment is stable.
- **Storage orchestration**: Kubernetes allows you to automatically mount a storage system of your choice, such as local storages, public cloud providers, and more.
- **Automated rollouts and rollbacks**: You can describe the desired state for your deployed containers using Kubernetes, and it can change the actual state to the desired state at a controlled rate. For example, you can automate Kubernetes to create new containers for your deployment, remove existing containers and adapt all their resources to the new container.
- **Automatic bin packing**: You provide Kubernetes with a cluster of nodes that it can use to run containerized tasks. You tell Kubernetes how much CPU and memory (RAM) each container needs. Kubernetes can fit containers onto your nodes to make the best use of your resources.
- **Self-healing**: Kubernetes restarts containers that fail, replaces containers, kills containers that don't respond to your user-defined health check, and doesn't advertise them to clients until they are ready to serve.
- **Secret and configuration management**: Kubernetes lets you store and manage sensitive information, such as passwords, OAuth tokens, and SSH keys. You can deploy and update secrets and application configuration without rebuilding your container images, and without exposing secrets in your stack configuration.

A detailed information of docker and kubernetes platform is given under the architecture section below. So the underlying platform in NIC CaaS is based on docker & kubernetes.


<!--![Screenshot from 2021-06-21 21-08-13](https://user-images.githubusercontent.com/67622286/122789463-f88fb780-d2d4-11eb-9ed1-f6309d3639e3.png-->

<!--## Basics of CaaS Platform

This section helps us to know about the <a href="/home/monika/Container1.pdf">Core Components and Technologies</a> like container, Virtual machines, Docker & Kubernetes that makes the NIC’s CaaS a cutting edge and modern DevOps Platform. -->


## **DevOps Architecture**

Let’s understand how DevOps Platform interacts with the two fundamental technologies Docker & Kubernetes. 

<a href="/home/monika/Devops _Architecture_docker&kubernets.pdf">Docker Technology</a>

<a href="/home/monika/Devops _Architecture_docker&kubernets.pdf">Kubernetes Technology</a>


<!--A simple explanation can be that a container is a form of operating system virtualization that contains all necessary executables, binary code, libraries and configuration files. There are some basic similarities but containers are very different from virtual machines. Compared to virtualization approaches, containers take advantage of a form of operating system (OS) virtualization in which features of the OS. In the case of the Linux kernel, namely the namespaces and cgroups are leveraged to isolate processes and control the amount of CPU, memory, and disk that those processes have access to.

Each container shares the same host OS or system kernel which makes containers more lightweight, portable and with less overhead. A container is a logical partition where users can run applications isolated from the rest of the system. Each application running in the container gets its own private network and a virtual filesystem that is not shared with other containers or the host.

<img src="https://user-images.githubusercontent.com/67622286/122790347-dcd8e100-d2d5-11eb-961b-2657ef015188.jpg" width=500 height=350>

*A comparison between Containers and Virtual machines*

<a href="/home/monika/Docker.pdf">Docker</a>
Docker uses a client server architecture where a **docker client** talks to a **docker daemon** which builds, runs and distributes containers.  The Docker client and daemon communicate using a REST API, over UNIX sockets or a network interface. 
  
A Docker **image** is a read-only template with instructions for creating a Docker container.
  
The Docker daemon (dockerd) listens for Docker API requests and manages Docker objects such as images, containers, networks, and volumes.  A daemon can also communicate with other daemons to manage Docker services.
  
**Docker engine** is the core of Docker, the underlying client-server technology that creates and runs the container. Docker engine components are : 
- A system with a running daemon process dockerd.
- APIs which specify interfaces that programs can use to talk to and instruct the Docker daemon.
- A command line interface (CLI) client docker.

A logical representation of docker engine -

<img src="https://user-images.githubusercontent.com/67622286/125411011-1e434480-e3db-11eb-828d-1f216d4852d8.png" width=500 height=220>

>**Note:  runc is a small, lightweight CLI wrapper for libcontainer and a standalone container runtime tool**.

### **Container Images**
  
A container image is a ready-to-run software package, containing everything needed to run an application. The code and any runtime it requires, all its software dependencies, system libraries, and default values for any essential settings that are required to run the application.

  
A container is a runnable instance on image. A docker container **registry** is a catalog of storage locations where you can push and pull container images. Docker hub is Docker’s own official image registry which can be a starting point for those who are new to container registry.  A Docker or a container **registry** stores Docker images. **Self-Hosted Registries** are one which can be setup as an organisation's own private registry.**Third-party registry** services are fully managed offerings that also give you control over how you manage your images—but without the operational headache of running your own on-premises registry. 
  
### **Container workflow**
  
Developers build container images from Dockerfiles and distribute container images from Docker registries. 


<img src="https://user-images.githubusercontent.com/67622286/122794469-ec5a2900-d2d9-11eb-9037-38cfb4cefdc7.png" width=650 height=170>

<div style="page-break-after: always"></div>

### **Kubernetes Technology**

Kubernetes when deployed, it's basically a **cluster**. A Kubernetes cluster consists of a set of machines called **nodes**. A node can be a virtual or physical machine. A node is a worker machine. A **worker node** hosts the Pods that are the components of the application workload. The application workload runs on worker nodes. 
     
*Please refer to the below diagram which is a high level representation of a Kubernetes cluster*.
     
<img src="https://user-images.githubusercontent.com/67622286/125412850-eb9a4b80-e3dc-11eb-89eb-108d85a26077.png" width=600 height=350>

A **pod** represents a set of running containers in the kubernetes cluster. A Pod is a group of one or more containers, with shared storage and network resources, and a specification for how to run the containers

>Every cluster should have at least one worker node.

The **control plane** manages the worker nodes and the Pods in the cluster. A control plane is the container orchestration layer that exposes the API and interfaces to define, deploy and manage the life cycle of a container. 

Kubernetes follows master-slave architecture having 

- [Master Node](#master-node)
     
- [Worker Node](#worker-node)
 
### Master Node 
The master node manages the Kubernetes cluster, and it is the entry point for all the administrative tasks. You can talk/connect to the master node via the CLI, GUI, or API. For achieving fault tolerance, there can be more than one master node in the cluster.

Below are the main components of a master node-

- **kube-apiserver** - The API server is the front end for the Kubernetes control plane.The main implementation of a Kubernetes API server is kube-apiserver. All communications and operations between the control plane components and external clients are translated into RESTful API calls that are handled by the API server, which then validates the requests, then processes and executes them.

- **kube-controller-manager** - Non-terminating control loops that regulate the state of the Kubernetes cluster are managed by the Control Manager. Now, each one of these control loops knows about the desired state of the object it manages, and then they look at their current state through the API servers. The controller manager makes sure that your current state is the same as the desired state.

- **cloud-controller-manager** - The cloud-controller-manager is a Kubernetes control plane component that embeds cloud-specific control logic. The cloud controller manager lets you link your cluster into your cloud provider's API. The cloud-controller-manager is structured using a plugin mechanism that allows different cloud providers to integrate their platforms with Kubernetes.

- **kube-scheduler** - The kube-scheduler is the Kubernetes controller responsible for assigning pods to nodes in the cluster. It's scope is narrow but complex. The scheduler also considers the quality of service requirements, data locality, and many other such parameters. kube-scheduler selects a node for the pod in a 2-step operation known as *Filtering & Scoring*.

- **etcd** -  The etcd is a distributed key-value store that is used to store the cluster state. etcd is written in the *goLang*, and it is based on the [Raft consensus algorithm](https://en.wikipedia.org/wiki/Raft_(algorithm)). Besides storing the cluster state, etcd is also used to store the configuration details such as the subnets and the config maps.


### Worker Node
A worker node is a virtual or physical server that runs the applications and is controlled by the master node. The pods are scheduled on the worker nodes, which have the necessary tools to run and connect them. **The application workload runs on worker nodes**.


The worker node has three components-

- **kubelet** - Kubelet is basically an agent that runs on each worker node and communicates with the master node. The kubelet takes a set of PodSpecs ``` a version of Pod library``` that are provided through various mechanisms and ensures that the containers described in those PodSpecs are running and healthy. The kubelet connects to the container runtime using *gRPC framework*. The kubelet connects to the *container runtime interface (CRI)* to perform containers and image operations. 
- **kube-proxy** - Kube-proxy is a network proxy that runs on each node in cluster.kube-proxy maintains network rules on nodes. These network rules allow network communication to Pods from network sessions inside or outside of cluster.
- **Container runtime** - The container runtime is the software that is responsible for running containers. Kubernetes supports several container runtimes: *Docker, containerd, CRI-O*, and any implementation of the Kubernetes CRI.

## Kubernetes Workloads

Workloads is an application running on Kubernetes inside a pod or a set of pods. Workload resources manage a set of pods. An application can be stateless or stateful. The workload resources configure controllers that make sure the right number of the right kind of pod are running, to match the state specified by you.-->

## **DevOps Platform Components** 

 The majority of NIC DevOps Platform software runs on the NIC DevOps Platform Server. This Server includes all the software components used to manage the entire deployment.


### **NIC DevOps Platform API Server**
NIC DevOps Platform API server is built on top of an embedded Kubernetes API server and etcd database. It implements the following functionalities:

#### User Management
NIC DevOps Platform API server manages user identities.

#### Authorization
NIC DevOps Platform API server manages access control and security policies.

#### Projects
A project is a group of multiple namespaces and access control policies within a cluster.

#### Nodes
NIC DevOps Platform API server tracks identities of all the nodes in all clusters.

### **Cluster Controller and Agents**
The cluster controller and cluster agents implement the business logic required to manage Kubernetes clusters.

- The *cluster controller* implements the logic required for the global NIC DevOps Platform install. It performs the following actions:
   - Configuration of access control policies to clusters and projects.
   - Provisioning of clusters by calling:
      - The required Docker machine drivers.
      - Kubernetes engines like RKE and GKE.

- A separate *cluster agent* instance implements the logic required for the corresponding cluster. It performs the following activities:
   - Workload Management, such as pod creation and deployment within each cluster.
   - Application of the roles and bindings defined in each cluster’s global policies.
   - Communication between clusters and NIC DevOps Platform Server: events, stats, node info, and health.

<div style="page-break-after: always"></div>

### **Authentication Proxy**

The *authentication proxy* forwards all Kubernetes API calls. It integrates with authentication services like local authentication, Active Directory, and GitHub. On every Kubernetes API call, the authentication proxy authenticates the caller and sets the proper Kubernetes impersonation headers before forwarding the call to Kubernetes masters. NIC DevOps Platform communicates with Kubernetes clusters using a service account.


## **Using the NIC DevOps Platform**

- Onboard Procedure for using the NIC DevOps Platform

- User Department can apply for availing National Cloud Services on the cloud portal at [https://cloud.gov.in/](https://cloud.gov.in/)
     
>Note: NIC National Cloud Services are presently available for Government Organizations.
   
### **NIC Onboarding Procedure**

Below are the various stages through which users can get the access to the desired Container as a  service. 
   
A user gets a dashboard for the applied service- 
     
<img src = "https://user-images.githubusercontent.com/67622286/122192835-a18f7a00-ceb1-11eb-8618-b9aa419fb594.png" width:05px height=150>

This url [https://cloud.gov.in/onboarding_procedure.php](https://cloud.gov.in/onboarding_procedure.php) provides the details on the onboarding process via stages. 


#### 1.Registration

User would be required to provide basic details in 'Get NIC Cloud Services' window of this portal. The required to be entered are as follows:

- Department Name
- Contact Person's Name
- Designation
- Email and Mobile Number  

<img src="https://user-images.githubusercontent.com/67622286/125433544-ec125991-379e-4093-95c8-5c1de50c7ef6.png" width=600 height=350>
     
#### 2.Sign-Up
     
On receipt of mail for Sign Up Applicant is required to perform following steps:

- Applicant will receive mail along with [https://cloud.gov.in/signup/](https://cloud.gov.in/signup/) for Sign Up.

- Using above link applicant can Sign Up using his email credentials.

- User would be required to agree with the [terms and conditions](https://cloud.gov.in/termsandconditions.php) to use the NIC Cloud Services.
On successful Sign Up, Applicant will be presented with Sign Up screen for keying in the details of officials responsible for Owning and Administration of Cloud Account. On submission of these details Sign Up form will be generated.

- A duly signed and stamped copy of this [form](https://cloud.gov.in/assets/on-boarding-image/sample_pdf.pdf) is required to be submitted to NIC Cloud Coordinator for further processing.

- NIC Cloud Coordinator (SIO/HOG/HOD) will then sign & upload the form on to the Cloud Portal through the upload link. (Kindly note, SIO in case of States/UTs or HOG/HOD Coordinator in case of Ministry/Department - 
please refer https://cloud.gov.in/contact.php for NIC Cloud Coordinators details).

<div style="page-break-after: always"></div>

#### 3.Service Request 
Once the Applicant's signup form is received, a service request ID is created for the user and is mailed to Cloud Account owner along with the [Url link]. (https://cloud.gov.in/service_request/) for the same. **(Kindly note, Here onwards term 'user' would apply for the officer who is the Owner of Cloud Account.)**

After the sign in, the user will be presented with the Cloud Service Catalogue of the following Cloud Offerings:

**3.1. Service Cloud Catalogue**
     
<img src="https://user-images.githubusercontent.com/67622286/122382704-cce49880-cf87-11eb-9126-9e73ddee4d0e.png" height=500>

From this catalogue, click to choose Container from the Container Services offerings You will be directed to following url [https://cloud.gov.in/procedure_container.php](https://cloud.gov.in/procedure_container.php)

     
Then follow the below steps to finally get access to your container dashboard
     
**3.2. Container Dashboard**

<img src="https://user-images.githubusercontent.com/67622286/122386237-4e89f580-cf8b-11eb-834a-0171600a4a5b.png" width=650 height=300>   
     
**3.3. Choose container as a service**

<img src="https://user-images.githubusercontent.com/67622286/122386941-fe5f6300-cf8b-11eb-97e4-51efba2dd2e5.png" width=650 height=300>  

<div style="page-break-after: always"></div>
    
**3.4. Order View for Container Service(s)**
     
<img src="https://user-images.githubusercontent.com/67622286/122709250-850d8c00-d27b-11eb-9250-5be81ceea47c.png" width=650 height=300> 

     
**3.5. Order Confirmation**
     
<img src = "https://user-images.githubusercontent.com/67622286/122795857-5fb06a80-d2db-11eb-95c3-21faf1735f24.png" width=650 height=300>

**3.6. Order Submittted**

<img src = "https://user-images.githubusercontent.com/67622286/122795868-6212c480-d2db-11eb-9ee9-bad54d2176b4.png" width=900 height=200>

<div style="page-break-after: always"></div>

**3.7. My Orders**
     
<img src = "https://user-images.githubusercontent.com/67622286/122795875-650db500-d2db-11eb-98f7-dcb85af1c482.png" width=900 height=200>
 

**3.8. Order List**

<img src = "https://user-images.githubusercontent.com/67622286/122795884-67700f00-d2db-11eb-98a7-3d2e28d3a532.png" width=650 height=300>
     
**3.9. Order Details**
     
<img src = "https://user-images.githubusercontent.com/67622286/122795900-69d26900-d2db-11eb-88ef-4ce2aa254011.png" width=650 height=300>

<div style="page-break-after: always"></div>

## **Operating NIC DevOps Platform**

Users will be provided with an Organization Admin account to access Services on Cloud after the Service request is given for the first time. Cloud dashboard link is available on Public Cloud portal https://cloud.gov.in Cloud dashboard can be accessed only through Secure network (VPN). Users can manage allocated resources to run the cloud Infrastructure Services through their respective dashboards.
  
Under the Platform of NIC DevOps it provides 3 Dashboards  which can be accessed by the below URL-

1. [https://git.cloud.gov.in](https://git.cloud.gov.in)
2. [https://chub.cloud.gov.in](https://chub.cloud.gov.in)
3. [https://devops.cloud.gov.in](https://devops.cloud.gov.in)


**https://git.cloud.gov.in** - It is a dedicated hub for source code management where developers keep personal repositories.The Dashboard of git.cloud.gov.in seems like-

 <img src ="https://user-images.githubusercontent.com/67622286/125444188-502ccfec-1da6-46ec-9f35-9f87c34e422a.png" width=600 height=350>
     
**https://Chub.cloud.gov.in** - It is a Cloud native repository that stores & secure images with policy and role based access control.The Dashboard of chub.cloud.gov.in seems like-

<img src ="https://user-images.githubusercontent.com/67622286/125445852-b73170b7-be05-4456-b9dc-5249c246f526.png" width=600 height=350> 
     
**https://devops.cloud.gov.in** - It is a container management platform which provides tools to successfully deploy the application in a production environment.The Dashboard of https://devops.cloud.gov.in seems like-

<img src ="https://user-images.githubusercontent.com/67622286/125446986-3a189da9-6eed-4040-acc3-24be6f5e874d.png" width=600 height=350>
     
Steps to work on the requested services which convert it into a dedicated Assigned projects to user in CaaS DevOps cloud platform-

Here we are discussing how to deploy applications into the production environment by using the CaaS NIC devops cloud platform. Few steps need to be followed to understand the procedure.

1. First Users will create the docker file & Docker file contains few layers & contents in order to build the docker image.

- **FROM BASE IMAGE**- Ask docker to fetch a base image & which docker will use in order to execute the rest of the commands. 
- **WORKDIR /app** - Docker will create a work directory (workdir /app)
- **COPY PACKAGE** - Docker will copy all the contents of the package file. 
- **RUN PACKAGE MANAGER INSTALL** - Docker uses package manager to install all the packages into the file.
- **COPY** - Copy rest of the content inside current working directory.
- **EXPOSE PORT** - This is the port which the Application is running.
- **CMD (“package manager”,“start”)**  - This is the command that is used to start the application.

2. After building and tagging the Docker image it is added into the repository with the latest tag.
     
3. Having created this image now we will push into our Registry in chub.cloud.gov.in portal by docker push command.

When we login into the chub portal by giving credentials we will explore further container hub platforms and see various features in chub suits.
     
### **chub Cloud Platform**
     
Here login into the chub portal user can see the dashboard of projects where multiple projects are created of an application.

<img src ="https://user-images.githubusercontent.com/67622286/125584697-028e8a93-24e7-4a56-9dd0-ab2685feef2c.png" width=600 height=350>
     
There are two types of projects in NIC DevOps Container Registry:
- **Public**: All users have the read privilege to a public project, it's convenient for you to share some repositories with others in this way.
- **Private**: A private project can only be accessed by users with proper privileges.

If the project that the image belongs to is private, you should sign in first:
```
$ docker login chub.cloud.gov.in
```
**You can now pull the image**:
```     
$ docker pull chub.cloud.gov.in/library/ubuntu:14.04
```
**Pushing images** - Before pushing an image, you must create a corresponding project on NIC DevOps Container Registry web UI.

First, log in from Docker client:

```     
$ docker login chub.cloud.gov.in
```
**Tag the image**:
```
$ docker tag ubuntu:16.04 chub.cloud.gov.in/demo/ubuntu:16.04
```
**Push the image:**
```
$ docker push chub.cloud.gov.in/demo/ubuntu:16.04:latest

```
> **Note - The above command only for reference purpose.**

**Result** - After pushing the image you can see the pushed repository under the Projects dashboard.

**Labels**
     
NIC DevOps Container Registry provides two kinds of labels to isolate kinds of images.
     
- **Global Level Label:** Managed by system administrators and used to manage the images of the whole system. They can be added to images under any projects.
- **Project Level Label:** Managed by project administrators under a project and can only be added to the images of the project.
     
When images are pushed on the project repository we have to assign labels accordingly like whether the image is used for *development*, *production* & *testing* purposes. we can refer below screenshot how to add label under the project - 

- click the ADD LABELS button & add labels

<div style="page-break-after: always"></div>

Refer screenshot below -

<img src ="https://user-images.githubusercontent.com/67622286/125591554-c7a66d8e-e93f-47cf-a07d-a5e5833028bb.png" width=700 height=350>   
     
**Result** - We  have successfully added the labels into the project repository.

     
**Logs**

In the log section we can find the activities like how many images have been pulled,how much time it's pushed,how many images are deleted etc.
Refer screenshot

<img src ="https://user-images.githubusercontent.com/67622286/125608050-8a07f89f-c187-489e-aa7d-e5cf0ad36e91.png" width=700 height=350>

<div style="page-break-after: always"></div>


**Configure Webhooks** 
     
When you have configured the webhook, you can see the status of the different notifications and the timestamp of the last time each notification was triggered.In webhooks we just provide the endpoints URL for triggered webhooks.Webhooks allow you to also integrate NIC DevOps Container Registry with other tools to streamline continuous integration and development processes.
Steps to configure webhooks-

1) Select a project and go to the Webhooks tab.
2) Enter the URL for your webhook endpoint listener.

<img src ="https://user-images.githubusercontent.com/67622286/125612284-db09387c-c5ad-439a-bc60-af6271885408.png" width=700 height=350>
 
    
3) If your webhook listener implements authentication, enter the authentication header.
4) To implement HTTPS POST instead of HTTP POST, select the Verify Remote Certificate check box.
5) Click Test Endpoint to make sure that NIC DevOps Container Registry can connect to the listener.
6) Click Continue to create the webhook.

**Result** - When you have created the webhook, you see the status of the different notifications and the timestamp of the last time each notification was triggered.
     
<img src ="https://user-images.githubusercontent.com/67622286/125613276-85cb5c44-dbfa-4a9e-9828-9c23d5179e04.png" width=700 height=350>
    
**Vulnerability scanning**

This section provides the scanning of the particular image or all images in NIC DevOps Container Registry having into the projects for deployed the images successfully into the environment. 

We have a dedicated scanner called *Clair* to check the vulnerabilities in the project Repository.Simply we just follow below steps-

1) Enter into the  project, select the repository. 
2) To trigger the vulnerability into the image we just select the image and click the **SCAN** button for the scan process.

    
<img src ="https://user-images.githubusercontent.com/67622286/125736137-2bae2e74-9f9c-4029-954f-0ed8dc8f5185.png" width=700 height=350> 
     
Click on the tag name link, the detail page will be opened. Besides the information about the tag, all the vulnerabilities found in the last analysis process will be listed with the related information.  
     
<img src ="https://user-images.githubusercontent.com/67622286/125736580-c1d2288a-b1a1-4b33-8b92-935d3a994ab4.png" width=700 height=350>      
     
     
**Note**- When you run vulnerability scans, images that are subject to Common Vulnerabilities and Exposures (CVE) are identified. According to the severity of the CVE and your security settings, the images might not be permitted to run so system administrators can create whitelists of CVEs to ignore during vulnerability scanning.
     
**Configuration** 

It is the one of the important sections in which we can set the Deployment Security where we can set the vulnerability severity of the image to be **below low** & **below high**  then only after that we can deploy the images successfully into the environment.
After that all the dependencies are fulfilled to run the image in the environment then we should move into the DevOps cloud portal to deploy the application.
    
<img src ="https://user-images.githubusercontent.com/67622286/125739996-f3f80ae2-7a64-4b8c-bd8a-fc3ea74f4781.png" width=700 height=350> 

<div style="page-break-after: always"></div>

# **DevOps Cloud** 

Login to NIC devops cloud through https://devops.cloud.gov.in and after successful login, the user will see the below dashboard providing information on the cluster.

<img src ="https://user-images.githubusercontent.com/67622286/125744310-e4a0047d-7978-4418-82fc-f69918e71b45.png" width=700 height=350>     

In the Cluster we can go further into the assigned project for Add Registry in order to deploy the application.

<img src ="https://user-images.githubusercontent.com/67622286/125743049-b1603470-f7b3-441f-9e5b-723cf469bcd3.png" width=700 height=350> 

Under the assigned project we just need to Add the Registry in order to deploy the application. So, Here are a few steps to deploy the application successfully into the environment.

1) Simply **click** into the Resource Tab, select the **Secrets** option and then we will find the **Registry Credentials Tab**.

2) Next we need to **Add** the Registry.
     
<img src ="https://user-images.githubusercontent.com/67622286/125746471-d27f2995-0412-4254-a070-f175a091c18c.png"  width=700 height=350> 
     
Into the Add Registry tab below are the field we just need to fill- 
     
**Add Registry name** - Here we define the name of the Registry.
     
**Define Scope** - Select a Scope for the registry. You can either make the registry available for the entire project or a single namespace.
     
**Add a Namespace** - Here we enter the name space.
     
**Define Address** - In this we Select the website that hosts your private/Public Registry.
     
**Enter User Name** - Enter credentials that authenticate with the registry.
     
**Enter Password**- Enter credentials that authenticate with the registry.
     
**SAVE**

**Result** - Your secret is added to the project or namespace, depending on the scope you chose.
- You can view the secret in the NIC DevOps Platform UI from the Resources > Registries view.
- Any workload that you create in the NIC DevOps Platform UI will have the credentials to access the registry if the workload is within the registry's scope.

<img src ="https://user-images.githubusercontent.com/67622286/125748805-de41af1d-a47b-4e02-a9fb-d31d2298f500.png" width=700 height=350>  

 After the above procedure the Registry save & below dashboard shows-
   
 <img src ="https://user-images.githubusercontent.com/67622286/125745992-0bb48de5-f183-4fa6-b13b-0b0552dbc09e.png" width=700 height=350>
     
Now this is the time to deploy the **Workload** `Workloads let you define the rules for application scheduling, scaling, and upgrade`

1) Click Resources > **Workloads**.
2) Enter a **Name** for the workload. 
3) Select a **workload type**.
4) From the Docker Image field, enter the name of the **Docker image** that you want to deploy to the project.
5) Either select an existing **namespace**, or click Add to a new namespace and enter a new namespace.
6) Click **Add Port** to enter a port mapping (which is declared in the docker file), which enables access to the application inside and outside of the cluster .
7) Click **Launch**.
      
<img src ="https://user-images.githubusercontent.com/67622286/125751430-23e1f560-4abd-4b13-90e0-5bfe2b660550.png" width=700 height=350>   
     
**Result**: The workload is deployed to the chosen namespace. You can view the workload's status from the project's Workloads view.     
     
After Deployed the workloads we can see below -
   
<img src ="https://user-images.githubusercontent.com/67622286/125752426-d334135b-c197-468f-a35d-27b727580a5c.png" width=700 height=350>     

**Result** - Now the Workload is succesfully running.
     
<img src ="https://user-images.githubusercontent.com/67622286/125753091-bb909964-0639-426c-89f8-db7b3dfd6df4.png" width=700 height=350>

### **Load balancers** 

If you want your applications to be externally accessible, you must add a load balancer to your cluster. Here we create an L7 load balancer through which we will be able to access the application.In order to create a Load Balancer we will be perform following steps -
     
1) Click the **Load Balancing** tab. Then click **Add Ingress**.
2) Enter a **Name** for the ingress.
3) Select an existing **Namespace** from the drop-down list in which the workload is.
4) Create ingress forwarding Rules.In which we can see three rule -
     - Automatically generate a xip.io hostname (This option is best used for testing, not production environments.)
     - Specify a **hostname** to use (If you use this option, ingress routes requests for a hostname to the service or workload that you specify.)
     - Use as the default backend (Use this option to set an ingress rule for handling requests that don't match any other ingress rules. For example, use this option to route requests that can't be found to a *404* page)
     
Here, we specify a hostname to use , in which ingress routes requests for a hostname to the service or workload that we are specifying.

5) Enter the **Hostname**
6) After adding the Request Hostname we move further into another next option which is **Add Target**.
7) Add a Target Backend. By default, a workload is added to the ingress, but you can add more targets by clicking either Service or Workload.
8) Select a **workload** or **service** from the Target drop-down list for each target you've added.
9) As we have deployed the Cluster IP therefore In order to access the Workload we should access it by Service backend because we have dedicated service running for this workload.
10) Then we Select the **Service Target**-->>Add **Service Name** then it automatically fetches the port. 
     
<img src ="https://user-images.githubusercontent.com/67622286/125762212-40651f6c-8d16-49b3-9697-9525a3a25712.png" width=700 height=350>
   
**Result**: Your ingress has successfully added into the project. 
     
The ingress begins enforcing your ingress rules.
     
11) If any of your ingress rules handle requests for encrypted ports, add a **certificate** to encrypt/decrypt communications.
     
**Note**: You must have an SSL certificate that the ingress can use to encrypt/decrypt communications.`
     
12) Click **Add Certificate**.
13) Select a Certificate from the drop-down list.
14) Enter the Host using encrypted communication.
15) To add additional hosts that use the certificate, click Add Hosts.
     
**Now we have achieved the deployment of a simple application file from the local system onto the DevOps Platform.**


<div style="page-break-after: always"></div>

# **CI/CD**


Using NIC DevOps Platform, you can integrate with a Git repository to set up a continuous integration (CI) pipeline.

NIC DevOps Platform contains a variety of tools that aren't included in Kubernetes to assist in your DevOps operations. NIC DevOps Platform can integrate with external services to help your clusters run more efficiently.The one of the tool is **Pipeline**

A pipeline consists of stages and steps. It is based on a specific repository. It defines the process to build, test, and deploy your code. NIC DevOps Platform uses the pipeline as a code model. Pipeline configuration is represented as a pipeline file in the source code repository, using the file name *rancher-pipeline.yml or .rancher-pipeline.yaml.*

To set up a pipeline, you'll first need to authorize NIC DevOps Platform using your Git settings. Directions are provided in the NIC DevOps Platform UI. After authorizing NIC DevOps Platform in GitHub, provide NIC DevOps Platform with a client ID and secret to authenticate.
     
After configuring NIC DevOps Platform and GitHub, you can deploy containers running Jenkins to automate a pipeline execution:
     
- Build your application from code to image.
- Validate your builds.
- Deploy your build images to your cluster.
- Run unit tests.
- Run regression tests.
     
### Here is the below workflow of CI/CD pipeline with Kubernetes-
     
<img src ="https://user-images.githubusercontent.com/67622286/125779875-26924826-8ee7-4fcc-8e2f-a3533f5e2f18.png" width=700 height=350> 

Now, we will discuss how to deploy a simple application file via CI/CD into DevOps platform.
     
- First login into the Git cloud Portal -
    
<img src ="https://user-images.githubusercontent.com/67622286/125780466-681002cb-1289-4e5f-9708-aaab744d4894.png" width=700 height=350> 

- After login into it we can see the assigned Projects dashboard.Into the project dashboard an assigned project consists of a group,subgroup and project name so here we can mention the same accordingly.
- Next we will push the local created folder onto the git repository master branch.
    
<img src ="https://user-images.githubusercontent.com/67622286/125781535-7290b61f-fc1f-426c-8793-dc46855de657.png" width=700 height=350>  
    
- After successfully pushed into the Git lab we need to add this Git repository into the devops cloud platform in order to interact with it. First we need to add the Kubernetes cluster into the Git repository.Click to the **Operation** Tab & choose **Kubernetes** and then click on **Add Kubernetes cluster**.   
     
<img src ="https://user-images.githubusercontent.com/67622286/125782087-63aed479-ac55-4f9e-a3b6-4c64e1063b5e.png" width=700 height=350> 

- Add the required details in order to add the cluster-
    - **Kubernetes Cluster Name** - Mention K8s cluster name
    - **Add URL** - Cluster Address
    - **CA Certificate** - Add Certificate
    - **Service Token Name** - By this option we can access the cluster

<img src ="https://user-images.githubusercontent.com/67622286/125782857-ba38d882-59d6-4c8c-b5a1-cf48cdab29f9.png" width=700 height=350>

>Note - The above details like URL & service token we fetch through the kubeconfig file (It is a file that is used to configured access to clusters) which is under the devops assigned cluster project.
     
<img src ="https://user-images.githubusercontent.com/67622286/125783293-d33ad879-c459-4ff1-8efb-1641b97253d0.png" width=700 height=350>

- After adding the required details (URL & Service token) by kubeconfig file click tab -->> Add kubernetes cluster.
- Click **Save Changes**.
     
<img src ="https://user-images.githubusercontent.com/67622286/125783852-4ff5c3c5-99fd-416c-b300-b8ee59660e4f.png" width=700 height=350>

**Result** - You have to add the Kubernetes cluster successfully.
     
Now we can see the Kubernetes cluster is on active state-
    
<img src="https://user-images.githubusercontent.com/67622286/125784164-3c743aee-8089-4b1a-b21f-e4e9f4d6c661.png" width=700 height=350>
     
- When configuring a pipeline, certain steps allow you to use environment variables to configure the step's script. In order to do that -
     
     - Go into the git lab setting click **CI/CD** option.
     - Now go into the Variable section and add the **desired variables** we need to set like *password*,*image* & *project name* etc.  
     - Click Resources > Pipelines.
     - From the pipeline for which you want to edit build triggers, select Ellipsis (...) > Edit Config.
     - Within one of the stages, find the step that you want to add an environment variable for, click the Edit icon.
     - Click Show advanced options.
     - Click Add **Variable**, and then enter a key and value in the fields that appear. Add more variables if needed.
     - Add your environment variable(s) into either the script or file.
     - Click **Save**.     
     
     
<img src="https://user-images.githubusercontent.com/67622286/125784555-f6465d11-6db2-486f-a014-cf27f908447b.png" width=700 height=350>
     
**Result** - Now Variable have successfully added.

<img src="https://user-images.githubusercontent.com/67622286/125788787-5c819e12-2b74-46c8-b676-b7bebee79dcb.png" width=700 height=350>
     
After this we need to trigger the pipeline-

Runners execute the jobs for build and deploy stages.
     
### **Build and Deploy Images**

The Build and Deploy Image step builds and publishes a Docker image. This process requires a Dockerfile in your source code's repository to complete successfully.

- Docker build is the first step in which script builds our docker image which is fetched from the libraries repository.
- Then into the script execution the docker login into our chub Repository & Push newly built image into the chub repository.

**Result**- So the job succeeded in building the image.
     
<img src="https://user-images.githubusercontent.com/67622286/125789913-1e1ac537-cd63-445f-bbb1-773b2917884b.png" width=700 height=350>
   
Then going into the **deploying stage** -After executing the whole end stage it's deployed now and seen the build job on to the passed stages.

At the stage of the completed the deployment we have to see the following into the scripts - 
     
- Configured Deployment
- Configured Service
- Configured Ingress  LB
     
<img src="https://user-images.githubusercontent.com/67622286/125790688-999129c0-efe5-44d5-addc-6819fbf0e8a2.png" width=700 height=350>
  
     
Now if we login into the devops cloud portal and then hit the assigned projects we are able to see the deployed one workload, Load Balancing & Services into it.

If we login into the devops cloud portal we have to be able to see the deployed workloads under the assigned project.
     
<img src="https://user-images.githubusercontent.com/67622286/125791025-fee35ab8-6aa0-48ea-8019-7d0a778e9cc5.png" width=700 height=350>


To ensure that we can check the log to see that the configuration has been completed or not and  workload ready for start up.

<img src="https://user-images.githubusercontent.com/67622286/125791355-b259e792-34cb-4086-9619-99143403992a.png" width=700 height=350>

Then we go into the git cloud CI/CD section and we are able to see the Pipeline has been passed successfully with the two stages  - Build & Deploy.

<img src ="https://user-images.githubusercontent.com/67622286/125791803-02df119e-57ef-4f99-b5fe-2976f5d129e8.png" width=700 height=350>
     
    
In order to check the running application we need to click on the endpoint into the workloads and then see the below result-
     
<img src="https://user-images.githubusercontent.com/67622286/125792092-f6754754-bce4-47ea-ae5b-fe08d3d830ee.png" width=700 height=350>

     
## Now we are able to deploy the application and follow the CI/CD pipeline in order to deploy.
    
     
     
     
