## **Deploy 5G Core with Network Slicing**  

Welcome to the session on 5G core deployment and network slicing. Participants will set up a complete 5G network environment on Kuberenetes using automated scripts, with a special focus on deploying Open5GS and UERANSIM for core network and RAN simulation, respectively. By the end, you will have a functional 5G setup with configured network slices, providing hands-on experience with key 5G technologies.

The figure below shows our network slicing setup with 2 network slices.

![slicing-setup](images/slicing-november-2024.png)

### **Background Reading**
- For a brief overview of the 5G core, see [intro-to-5g-core](intro-to-5g-core.md).
- For background on network slicing, see [network-slicing](network-slicing.md).

### **1. Setting Up the Environment**  
**Location:** MC2061 (pre-configured with VirtualBox and VMs)

In this hands-on session, we will set up the environment to deploy a 5G core network, using pre-loaded virtual machines (VMs) and automated scripts to simplify configuration:

- **Access the Nodes**: Connect to the designated nodes for deployment.
- **Run the [testbed-automator](https://github.com/niloysh/testbed-automator) Script**:
    1. **Kubernetes Setup**: Configure a Kubernetes cluster for efficient 5G core management.
    2. **Network Tools**: Set up Open vSwitch (OVS) and Multus for enhanced connectivity and multi-interface support for network slicing.
    3. **Configure OVS-CNI**: Integrate OVS Container Network Interface (CNI) for streamlined communication within Kubernetes, supporting our network slicing framework.

By the end of this setup, participants will have a fully functional environment for 5G core deployment. For exercises, see the [labs](https://github.com/niloysh/testbed-automator/blob/main/labs/lab1/lab1.md).

> [!NOTE] 
> For an overview of relevant technologies, see [technologies](technologies.md).

### **2. Deploying a 5G Core Network with Open5GS and UERANSIM**

Using [open5gs-k8s](https://github.com/niloysh/open5gs-k8s), we will:

1. **Deploy a 5G Core Network**: Set up two network slices.
2. **Simulate a RAN and UEs**: Deploy UERANSIM for RAN and user equipment simulation.
3. **Subscriber Testing**: Add two subscribers (one per slice) and conduct a ping test.

After deployment, exercises are available in the [labs](https://github.com/niloysh/open5gs-k8s/blob/main/labs/lab1/lab1.md).
