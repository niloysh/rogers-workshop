## **Monitoring Network Slices**  

Welcome to the second session of the Rogers Executive Workshop.
In this session, we will look at monitoring network slices with **5G-Monarch**.

![monarch-conceptual-architecture](images/monarch-conceptual-architecture.png)

The figure above shows the conceptual architecture of Monarch. Monarch is designed for cloud-native 5G deployments and focuses on network slice monitoring and per-slice KPI computation.

### **1. Setting Up Monitoring Tools**

In this session, we will use [5g-Monarch](https://github.com/niloysh/5g-monarch) to monitor 5G network slices and collect real-time telemetry data.

**Install Monarch Components**
- Install various Monarch components such as Prometheus for collecting and storing metrics data and Grafana for visualizing and analyzing slice performance metrics.
- Configure Monarch for slice-level data collection, e.g., slice throughput.

By the end of this setup, participants will have real-time monitoring for deployed slices.


### **2. Hands-on Monitoring and Telemetry Collection**

We will monitor slices using the configured tools, observe performance metrics, and gain insights into slice health:

1. **Set Up Dashboards in Grafana**: Create custom dashboards for visualizing slice-specific metrics.
2. **Real-Time Monitoring Exercises**:
    - Track number of subscribers and CPU usage for NFs.

For exercises, see the [Labs](https://github.com/niloysh/5g-monarch/blob/main/labs/lab1.md).
