# Little Anchorage Financial Bank: DevOps Project

In fulfilment of the group DevOps project assignment due Monday week 11 at QA consulting.

## Index
[Brief](#brief)
   
[Architecture](#architecture)
     
[Technologies Used](#tech)

[Deployment](#depl)
   * [Prerequisites](#prereq)
   * [CI Pipeline](#CI)
   * [Docker Swarm](swarm)

 
[Authors](#auth)

[Acknowledgements](#ack)

<a name="brief"></a>
## The Brief

To create an OOP-based application with utilisation of supporting tools, methodologies and technologies that encapsulate all core modules covered during training. The application must manipulate two tables with full CRUD functionality.

<a name="architecture"></a>
## Architecture
#### Before

#### After

<a name="tech"></a>
### Technologies Used

* H2 Database Engine - Database
* Java - Logic
* Wildfly - Deployment
* Jenkins - CI Server
* Maven - Dependency Management
* Jacoco, EclEmma, Surefire - Test Reporting
* SonarQube - Static Testing
* [Git](https://github.com/ayshamarty/SoloProject.git) - VCS
* [Trello](https://trello.com/qasoloproject) - Project Tracking
* GCP - Live Environment

<a name="depl"></a>
## Deployment

<a name="prereq"></a>
### Prerequisites
* A virtual machine with Jenkins, Docker and Docker-Compose installed
* At least one other virtual machine with Docker installed
* Access to a Dockerhub registry

#### Installing Jenkins, Docker and Docker Compose
1. Clone down this repository and run the following commands and follow the instructions:
<p align="center">
**sh ~/LAFB/installation/jenkins.sh**

**sh ~/LAFB/installation/docker.sh**
*remember to copy this script and run it on at least one other machine. These machines will be used for your worker nodes*

</p>
2. As the Jenkins user, login to a dockerhub account that has access to the registry:
<p align="center">
**sudo su Jenkins**
**docker login**
*enter your username and password*
</p)


<a name="CI"></a>
### CI pipeline

<a name="swarm"></a>
### Docker Swarm

<a name="auth"></a>
## Authors

Aysha Marty and Krystal Ryan

<a name="ack"></a>
## Acknowledgements

* QA consulting and our fantastic instructors
* The rest of our wonderful cohort on the programme
