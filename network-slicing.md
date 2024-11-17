---
title: Network Slicing Overview
permalink: /network-slicing
layout: default
---

# Network Slicing Overview

In this workshop, we focus on network slicing within the 5G Core. Future workshops will cover slicing for the Radio Access Network (RAN) and transport segments.

### Transport Layer Slicing
Methods like VLAN tagging and MPLS provide differentiated paths for various traffic types, and programmable switches can enable data paths for distinct slices.

### RAN Slicing
RAN slicing can use slice-specific schedulers to optimize Physical Resource Block (PRB) allocation.

## Core Network Slicing

In the 5G Core, network slicing is achieved by deploying distinct instances of key network functions (NFs) for each slice. These instances are allocated resources based on their specific service level agreements (SLAs). Using Kubernetes, we create isolated environments for each slice, allowing for flexible scaling and management of resources like CPU, memory, and storage.

On **Day 2**, we will explore algorithms that dynamically allocate resources based on real-time traffic and data patterns, optimizing resource distribution across slices to meet service requirements efficiently.

### Slice Configuration
In this workshop setup, each slice has a dedicated **Session Management Function (SMF)** and **User Plane Function (UPF)**, while other core functions, like the **Access and Mobility Management Function (AMF)**, are shared. This setup enhances control over resources to meet varying demands for applications such as **enhanced mobile broadband (eMBB)** and **ultra-reliable low-latency communication (URLLC)**.

> [!TIP]
> For a brief background on the 5G core, see the [intro-to-5g-core](intro-to-5g-core.md) document.

## Workshop Slicing Setup

![slicing-setup](images/slicing-november-2024.png)
*Figure: Two network slices with individual SMF and UPF for dedicated resources.*

Each slice supports one or more **PDU sessions**, representing a logical user data connection. This structure enables tailored resource management for specific use cases.


## Slicing Use Cases
In a [previous demos](https://uwaterloo.ca/news/researching-cutting-edge-5g-network-slicing-technology) conducted at the University of Waterloo, we showcased how two PDU sessions support two clients (UEs) on a cloud gaming slice. Using a resource scaling algorithm, we dynamically optimized bandwidth and latency, meeting the specific needs of each client efficiently.
