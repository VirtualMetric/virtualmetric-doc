# VMWare

Following modules could be used for VMware vSphere monitoring:

* &#x20;  Bare Metal
* &#x20;  VMware

## **Supported Versions**

VirtualMetric supports following versions of VMware vSphere:

```markup
VMware vSphere Hypervisor (ESXi) 4.0
VMware vSphere Hypervisor (ESXi) 4.0 U1
VMware vSphere Hypervisor (ESXi) 4.0 U2
VMware vSphere Hypervisor (ESXi) 4.0 U3
VMware vSphere Hypervisor (ESXi) 4.0 U4
VMware vSphere Hypervisor (ESXi) 4.1
VMware vSphere Hypervisor (ESXi) 5.0
VMware vSphere Hypervisor (ESXi) 5.5
VMware vSphere Hypervisor (ESXi) 5.5 U1
VMware vSphere Hypervisor (ESXi) 5.5 U2
VMware vSphere Hypervisor (ESXi) 5.5 U3
VMware vSphere Hypervisor (ESXi) 6.0.0 U1
VMware vSphere Hypervisor (ESXi) 6.0.0 U2
VMware vSphere Hypervisor (ESXi) 6.5.0
VMware vSphere Hypervisor (ESXi) 7.0
VMware vSphere Hypervisor (ESXi) 7.0 U1
```

***

## **Sizing**

Hardware requirements for VirtualMetric depends on total number of monitored object (VMware VM etc.) and intervals used. The following values are provided as reference for common usage of VirtualMetric (based on 20 seconds interval). Inventory collections are not included in this calculations.

### **Bare Metal**

*   _**Per Host**_

    a. 150 MB of memory (VirtualMetric Trigger)\
    b. 4 Kbps of bandwidth (VirtualMetric API)\
    c. 15 MB of disk space per month (VirtualMetric Database)

### **VMware**

*   _**Per Host**_

    a. 150 MB of memory (VirtualMetric Trigger)\
    b. 4 Kbps of bandwidth (VirtualMetric API)\
    c. 15 MB of disk space per month (VirtualMetric Database)
*   _**Per Virtual Machine**_

    a. 5 KB of memory (VirtualMetric Database)\
    b. 4 Kbps of bandwidth (VirtualMetric API)\
    c. 20 MB of disk space per month (VirtualMetric Database)
