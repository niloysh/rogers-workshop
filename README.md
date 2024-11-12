# Rogers Executive Workshop

Welcome to the first Rogers Executive Workshop, presented as part of the UW Chair in Network Automation!

This two-day workshop, held on November 19 and 20, will explore essential aspects of 5G technology, including 5G core deployment, network slicing, slice monitoring, and dynamic resource scaling.

## Table of Contents

- [Rogers Executive Workshop](#rogers-executive-workshop)
  - [Table of Contents](#table-of-contents)
  - [Workshop Schedule](#workshop-schedule)
    - [November 19](#november-19)
    - [November 20](#november-20)
  - [Learning Outcomes](#learning-outcomes)
    - [November 19](#november-19-1)
    - [November 20](#november-20-1)
  - [Hardware](#hardware)
    - [VM Specifications](#vm-specifications)
    - [Accessing Your Workshop VM](#accessing-your-workshop-vm)
      - [1. Retrieve Your Login Credentials](#1-retrieve-your-login-credentials)
      - [2. Launching the Workshop VM](#2-launching-the-workshop-vm)
      - [3.	Ubuntu Desktop Environment](#3ubuntu-desktop-environment)
    - [Local Setup (Optional)](#local-setup-optional)
  - [Workshop Agenda](#workshop-agenda)
    - [November 19](#november-19-2)
    - [November 20](#november-20-2)
  - [Background Reading](#background-reading)



## Workshop Schedule

### November 19

| **Time**            | **Session**                           | **Notes**                                                                                                                                                                                                                                                       |
| ------------------- | ------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 9:00 AM - 9:45 AM   | Workshop Introduction                 | [Slides](https://uofwaterloo-my.sharepoint.com/:p:/g/personal/n6saha_uwaterloo_ca/EWk_7MFU9pFJrVZkGdB-UioBMucyLwG3qi9S5FWbJesQug?e=dSHQqL)                                                                                                                      |
| 10:00 AM - 11:00 AM | Deploy 5G core on Kubernetes          | - [Session Overview](core-deployment.md) <br> - [Companion Document 1](https://github.com/niloysh/testbed-automator) <br> - [Companion Document 2](https://github.com/niloysh/open5gs-k8s)                                                                      |
| 11:00 AM - 11:15 AM | Coffee Break                          |                                                                                                                                                                                                                                                                 |
| 11:15 AM - 12:00 PM | Deploy 5G core on Kubernetes (cont'd) | [Exercises](https://github.com/niloysh/open5gs-k8s/blob/main/labs/lab1/lab1.md)                                                                                                                                                                                 |
| 12:00 PM - 1:30 PM  | Lunch Break                           | Location: EC5 ([Map](https://maps.app.goo.gl/xcvsAFFkqKpyULCHA))                                                                                                                                                                                                |
| 1:30 PM - 2:00 PM   | Demo Session                          | - Location: DC2554 ([Map](https://maps.app.goo.gl/TL3auogCjkvPy2J37))          <br> - [Slides](https://uofwaterloo-my.sharepoint.com/:p:/g/personal/n6saha_uwaterloo_ca/EXLDGhP2xdJFsUn9KRY_iMQBHPGl2FM--HnNeoniELuCkw?e=LuI9Xq)                                |
| 2:00 PM - 3:00 PM   | Monitoring network slices             | - [Slides](https://uofwaterloo-my.sharepoint.com/:p:/g/personal/n6saha_uwaterloo_ca/EeysQgkYTAtIiXRsfu3hI0sB63caGOhvK1MWLSvfzVsIHw?e=Yn94Lf) <br> - [Session Overview](slice-monitoring.md)  <br> - [Companion Document](https://github.com/niloysh/5g-monarch) |
| 3:00 PM - 3:15 PM   | Coffee Break                          |                                                                                                                                                                                                                                                                 |
| 3:15 PM - 4:00 PM   | Monitoring network slices (cont'd)    | [Exercises](https://github.com/niloysh/5g-monarch/blob/main/labs/lab1.md)                                                                                                                                                                                       |

### November 20

| **Time**            | **Session**                               | **Notes**                                                                                                                                                                                         |
| ------------------- | ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 9:00 AM - 10:30 AM  | Ingestion and parsing of 5G data          | [Slides](https://uofwaterloo-my.sharepoint.com/:p:/g/personal/n6saha_uwaterloo_ca/Ec-IgYDYxoNPqzz_B6I_BSMBg88t2JdNEBmCWpq_9OIckw?e=NYDzTO) |
| 10:30 AM - 10:45 AM | Coffee Break                              |                                                                                                                                                                                                   |
| 10:45 AM - 12:00 PM | Ingestion and parsing of 5G data (cont'd) |                                                                                                                                                                                                   |
| 12:00 PM - 1:30 PM  | Lunch Break                               | Location: EC5 ([Map](https://maps.app.goo.gl/xcvsAFFkqKpyULCHA))                                                                                                                                  |
| 1:30 PM - 2:45 PM   | Dynamic resource scaling                  | [Slides](https://uofwaterloo-my.sharepoint.com/:p:/g/personal/n6saha_uwaterloo_ca/EbCHISVoIG9DpRWlvCTeEakBL3S3s3A9IAMavYtXEGT9Qg?e=6Uv12C) <br> [Companion Document](dynamic-resource-scaling.md) |
| 2:45 PM - 3:00 PM   | Coffee Break                              |                                                                                                                                                                                                   |
| 3:00 PM - 4:00 PM   | Dynamic resource scaling (cont'd)         |                                                                                                                                                                                                   |  |  |


## Learning Outcomes

### November 19

1.	Understand the deployment and configuration of a 5G core network on Kubernetes.
2.	Gain hands-on experience in creating, configuring, and managing 5G network slices.
3.	Learn to configure and deploy a monitoring architecture for network slices.
4.	Acquire practical skills in analyzing 5G network KPIs.

### November 20
1.	Explore data processing pipeline technologies for 5G telemetry.
2.	Experiment with building and maintaining data pipelines using NiFi and Kafka.
3.	Learn how to train 5G VNF models and compose them to form end-to-end slice models.
4.	Experiment with ML-based slice model for dynamic resource scaling


## Hardware

Each participant will receive a virtual machine (VM) hosted in **MC2061**, pre-configured for the workshop.

[Map to MC](https://maps.app.goo.gl/2jaXV5coMXUh37SJ8)

### VM Specifications

| **CPU** | **Memory** | **Storage** | **OS**           |
| ------- | ---------- | ----------- | ---------------- |
| 8 vCPUs | 16GB RAM   | 50GB        | Ubuntu 22.04 LTS |

### Accessing Your Workshop VM

Participants will be seated at workstations in room **MC2061**, where each machine will have an individual login. 

> [!NOTE]
> Please choose a machine at the start and remain at the same workstation for all sessions.

#### 1. Retrieve Your Login Credentials
You will receive a card with login credentials for your workstation at the start of the workshop. Please keep these details secure.
#### 2. Launching the Workshop VM
Once logged in, use the provided script on your desktop to start the workshop VM. This VM is pre-configured with all necessary tools and resources for the sessions.
#### 3.	Ubuntu Desktop Environment
The workshop VM features Ubuntu 22.04 LTS with a Desktop GUI, where all tasks and exercises will take place.

If you have any issues logging in or launching the VM, workshop assistants will be available to help.


### Local Setup (Optional)

For participants who want to replicate the environment on their own device:

| **Requirement** | **Specification**                |
| --------------- | -------------------------------- |
| CPU             | 8 vCPUs                          |
| Memory          | 16GB RAM                         |
| Storage         | 50GB free                        |
| OS              | Ubuntu 20.04 / 22.04 (preferred) |


## Workshop Agenda

### November 19

1. **[Deploy 5G Core with Network Slicing](core-deployment.md)**  
   Set up and deploy a 5G core network on Kubernetes, configure network slices, and simulate user equipment for traffic testing.

2. **[Monitoring Network Slices](slice-monitoring.md)**  
   Configure monitoring tools for network slice telemetry, set up dashboards, and analyze slice performance metrics in real-time.

### November 20

1. **Introduction to Data Processing Pipelines**  
   Overview of data pipeline technologies, focusing on handling large-scale 5G telemetry data.

2. **Hands-on with Kibana and Spark**  
   Explore data visualization with Kibana and data processing with Spark to analyze and manage slice data.

3. **[Slice modeling using vNetRunner](dynamic-resource-scaling.md)**  
   Use the vNetRunner framework to train VNF models and compose them to form end-to-end slice models.

4. **[Dynamic Resource Scaling using MicroOpt](dynamic-resource-scaling.md)**  
   Use the MicroOpt framework to perform dynamic resource scaling for network slices.

## Background Reading

For more background, see these supporting resources:
- **[Introduction to 5G Core](intro-to-5g-core.md)**
- **[Technologies Overview](technologies.md)**
- **[Network Slicing](network-slicing.md)**
- **[Introduction to Dynamic Resource Scaling](intro-to-drs.md)**
