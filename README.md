# Rogers Workshop

Welcome to the first Rogers Workshop, presented as part of the UW Chair in Network Automation!

This two-day workshop, held on November 19th and 20th, will explore essential aspects of 5G technology, including 5G core deployment, network slicing, slice monitoring, and dynamic resource scaling.

## Table of Contents

- [Rogers Workshop](#rogers-workshop)
  - [Table of Contents](#table-of-contents)
  - [Workshop Schedule](#workshop-schedule)
    - [Day 1: 19th November](#day-1-19th-november)
    - [Day 2: 20th November](#day-2-20th-november)
  - [Learning Outcomes](#learning-outcomes)
    - [Day 1: 19th November](#day-1-19th-november-1)
    - [Day 2: 20th November](#day-2-20th-november-1)
  - [Hardware](#hardware)
    - [VM Specifications](#vm-specifications)
    - [SSH Access to the VM](#ssh-access-to-the-vm)
    - [Local Setup (Optional)](#local-setup-optional)
  - [Workshop Agenda](#workshop-agenda)
    - [Day 1: 19th November](#day-1-19th-november-2)
    - [Day 2: 20th November](#day-2-20th-november-2)
  - [Background Reading](#background-reading)



## Workshop Schedule

### Day 1: 19th November

| **Session**                  | **Time**            | **Notes**                                                                                                                                                                                                                                                      |
| ---------------------------- | ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Introduction                 | 9:00 AM - 9:45 AM   | [Slides](https://uofwaterloo-my.sharepoint.com/:p:/g/personal/n6saha_uwaterloo_ca/EWk_7MFU9pFJrVZkGdB-UioBMucyLwG3qi9S5FWbJesQug?e=dSHQqL)                                                                                                                     |
| Deploy 5G core on Kubernetes | 10:00 AM - 12:00 PM | - [Session Overview](core-deployment.md) <br> - [Companion Document 1](https://github.com/niloysh/testbed-automator) <br> - [Companion Document 2](https://github.com/niloysh/open5gs-k8s)                                                                     |
| Lunch Break                  | 12:00 PM - 1:30 PM  | Location: EC5 ([Map](https://maps.app.goo.gl/xcvsAFFkqKpyULCHA))                                                                                                                                                                                               |
| Monitoring network slices    | 1:30 PM - 4:00 PM   | - [Session Overview](slice-monitoring.md) <br> - [Slides](https://uofwaterloo-my.sharepoint.com/:p:/g/personal/n6saha_uwaterloo_ca/EXLDGhP2xdJFsUn9KRY_iMQBHPGl2FM--HnNeoniELuCkw?e=LuI9Xq) <br> - [Companion Document](https://github.com/niloysh/5g-monarch) |

### Day 2: 20th November

| **Session**                      | **Time**              | **Notes**                                                        |
| -------------------------------- | --------------------- | ---------------------------------------------------------------- |
| Ingestion and parsing of 5G data | 9:00 AM - 12:00 PM AM |                                                                  |
| Lunch Break                      | 12:00 PM - 1:30 PM    | Location: EC5 ([Map](https://maps.app.goo.gl/xcvsAFFkqKpyULCHA)) |
| Slice resource allocation        | 1:30 PM - 4:00 PM     |                                                                  |


## Learning Outcomes

### Day 1: 19th November

1. Deploy and configure a 5G network on Kubernetes.
2. Create and manage network slices.
3. Simulate a 5G RAN and send traffic through network slices.
4. Monitor network slices and collecting telemetry data in a 5G environment.

### Day 2: 20th November
1. Explore data processing pipeline technologies.
2. Hands-on with Kibana and Spark.
3. Introduction to dynamic resource scaling.
4. Collect datasets from the 5G environment and apply machine learning techniques for dynamic resource scaling.


## Hardware

Each participant will receive a virtual machine (VM) hosted in **MC3027**, pre-configured for the workshop.

[Map to MC](https://maps.app.goo.gl/2jaXV5coMXUh37SJ8)

### VM Specifications

| **CPU** | **Memory** | **Storage** | **OS**           |
| ------- | ---------- | ----------- | ---------------- |
| 8 vCPUs | 16GB RAM   | 50GB        | Ubuntu 22.04 LTS |

### SSH Access to the VM

Each participant will access their virtual machine (VM) via SSH. Please follow the instructions below to connect:

1. **Retrieve VM IP and Credentials**  
   - Your VM’s IP address and login credentials will be provided at the start of the workshop. Ensure you have these details ready.

2. **Connecting via SSH**  
   - **Linux/macOS Users**:  
     Open a terminal and use the following command:
     ```bash
     ssh username@your_vm_ip
     ```

3. **SSH Key Setup (Optional)**  
   - For a more secure and convenient connection, you can set up SSH keys. Run the following commands to generate a key pair and add it to your VM:
     ```bash
     ssh-keygen -t rsa -b 2048
     ssh-copy-id username@your_vm_ip
     ```
   - Once configured, you can log in without a password.



### Local Setup (Optional)

For participants who want to replicate the environment on their own device:

| **Requirement** | **Specification**                |
| --------------- | -------------------------------- |
| CPU             | 8 vCPUs                          |
| Memory          | 16GB RAM                         |
| Storage         | 50GB free                        |
| OS              | Ubuntu 20.04 / 22.04 (preferred) |


## Workshop Agenda

### Day 1: 19th November

1. **[Deploy 5G Core with Network Slicing](core-deployment.md)**  
   Set up and deploy a 5G core network on Kubernetes, configure network slices, and simulate user equipment for traffic testing.

2. **[Monitoring Network Slices](slice-monitoring.md)**  
   Configure monitoring tools for network slice telemetry, set up dashboards, and analyze slice performance metrics in real-time.

### Day 2: 20th November

1. **Introduction to Data Processing Pipelines**  
   Overview of data pipeline technologies, focusing on handling large-scale 5G telemetry data.

2. **Hands-on with Kibana and Spark**  
   Explore data visualization with Kibana and data processing with Spark to analyze and manage slice data.

3. **Dynamic Resource Scaling**  
   Implement dynamic scaling for slice resources based on network demand and load.

4. **Building and Training a Slice Model**  
   Gather a 5G dataset and use machine learning to train a model for predictive slice management.

## Background Reading

For more background, see these supporting resources:
- **[Introduction to 5G Core](intro-to-5g-core.md)**
- **[Technologies Overview](technologies.md)**
- **[Network Slicing](network-slicing.md)**