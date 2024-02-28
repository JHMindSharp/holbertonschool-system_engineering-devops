![WEBINFRA](https://image.noelshack.com/fichiers/2024/09/3/1709125457-621f0817-bc3f-4b2d-973b-bdd6dab5cfa1.jpg)
# Web Infrastructure Design

## Introduction
This project explores the fundamentals of web infrastructure design. We delve into the architecture of web servers, application servers, and databases, and how they interact to serve content to users. By understanding these components, we aim to design scalable, reliable, and secure web infrastructures.

## Concepts
In this project, we cover several key concepts:
- Network basics
- Servers
- Web servers
- DNS
- Load balancers
- Monitoring

## Resources
To grasp the foundational knowledge required for this project, the following resources are recommended:
- [Network basics concept page](#)
- [Server concept page](#)
- [Web server concept page](#)
- [DNS concept page](#)
- [Load balancer concept page](#)
- [Monitoring concept page](#)
- [What is a database](#)
- [What’s the difference between a web server and an app server?](#)
- [DNS record types](#)
- [Single point of failure](#)
- [How to avoid downtime when deploying new code](#)
- [High availability cluster (active-active/active-passive)](#)
- [What is HTTPS](#)
- [What is a firewall](#)

## Learning Objectives
By the end of this project, learners will be able to:
- Design a basic web stack infrastructure using a LAMP model.
- Explain the role and function of each component within the stack.
- Understand and explain system redundancy and common acronyms like LAMP, SPOF, and QPS.
- Identify single points of failure and strategies for mitigating downtime.
- Design a scalable and secure web infrastructure with load balancing, HTTPS, and firewalls.

## Tasks

### Task 0: Simple Web Stack
Design a one-server web infrastructure hosting a website accessible via `www.foobar.com`. The design includes:
- 1 server
- 1 web server (Nginx)
- 1 application server
- 1 database (MySQL)
- Domain name `foobar.com` with a `www` record pointing to server IP `8.8.8.8`

#### Considerations:
- Explain the role of each component.
- Discuss potential issues such as Single Point of Failure (SPOF) and scalability.

### Task 1: Distributed Web Infrastructure
Expand the design to a three-server infrastructure for `www.foobar.com`, adding:
- 2 additional servers
- 1 load balancer (HAproxy)

#### Considerations:
- Justify the addition of each new element.
- Discuss the chosen load balancing algorithm and its setup.
- Explain the database Primary-Replica setup.

### Task 2: Secured and Monitored Web Infrastructure
Enhance the three-server infrastructure for `www.foobar.com` to include security and monitoring features:
- 3 firewalls
- 1 SSL certificate for HTTPS
- 3 monitoring clients

#### Considerations:
- Justify each added element, focusing on firewalls, HTTPS, and monitoring.
- Discuss potential issues like SSL termination at the load balancer and single-write MySQL server setup.

### Task 3: Scale Up
Further scale the infrastructure by:
- Adding 1 more server
- Configuring the load balancer as a cluster

#### Considerations:
- Justify the addition of each new element.
- Discuss the separation of components across servers.

## Conclusion
This project lays the groundwork for understanding and designing robust web infrastructures. By dissecting each component's role and interplay, we aim to build scalable, secure, and efficient web services.

---

**Author: Sylvain Kalache**
