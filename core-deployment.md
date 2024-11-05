## **Deploy 5G Core with Network Slicing**  
**Time:** November 19th, 10:00 AM - 12:00 PM  

### **Background Reading**
For a brief overview of the 5G core, please see [intro-to-5g-core](intro-to-5g-core.md).

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