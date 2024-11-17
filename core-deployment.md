---
title: Core Deployment
permalink: /core-deployment
layout: default
---

# **Deploy 5G Core with Network Slicing**  

Welcome to the session on 5G core deployment and network slicing. In this session, participants will set up a complete 5G network environment on Kuberenetes using automated scripts, with a special focus on deploying Open5GS and UERANSIM for core network and RAN simulation, respectively. By the end, you will have a functional 5G setup with configured network slices, providing hands-on experience with key 5G technologies.

The figure below shows our network slicing setup with 2 network slices.

![slicing-setup](images/slicing-november-2024.png)

# **Background Reading**
- For a brief overview of the 5G core, see [intro-to-5g-core](intro-to-5g-core.md).
- For background on network slicing, see [network-slicing](network-slicing.md).
- For an overview of relevant technologies, see [technologies](technologies.md).

## **1. Setting Up the Environment**  


In this first part of the session, you will set up the environment required to deploy a 5G core network. Automated scripts will streamline the configuration process.

- **Access the Nodes**: Log in to the designated nodes using the following credentials:
    - Username: `user`
    - Password: `user`
- **Run the Automator Script**:
    1. **Kubernetes Setup**: Configure a Kubernetes cluster for efficient 5G core management.
    2. **Network Tools**: Set up Open vSwitch (OVS) and Multus for enhanced connectivity and multi-interface support for network slicing.
    3. **Configure OVS-CNI**: Integrate OVS Container Network Interface (CNI) for streamlined communication within Kubernetes, supporting our network slicing framework.

By the end of this setup, participants will have a fully functional environment for 5G core deployment.

**Slides for this section:** [Environment Setup Slides](https://niloysh.github.io/testbed-automator/slides.pdf).




## **2. Deploying a 5G Core Network with Open5GS and UERANSIM**

This section focuses on deploying and testing a 5G core network with network slicing:

1. **Deploy a 5G Core Network**: Set up two network slices.
2. **Simulate a RAN and UEs**: Deploy UERANSIM for RAN and user equipment simulation.
3. **Subscriber Testing**: Add two subscribers (one per slice) and conduct a ping test.

**Slides for this section:** [5G Core Deployment Slides](https://niloysh.github.io/open5gs-k8s/slides.pdf).