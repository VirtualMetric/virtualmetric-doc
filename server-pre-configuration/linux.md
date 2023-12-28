# Linux

Following modules could be used for Linux monitoring:

* &#x20;  Bare Metal

## **Requirements**

Following Linux applications are required on Linux servers for monitoring:

* &#x20;  Awk
* &#x20;  Curl
* &#x20;  Sar (Sysstat)

***

## **Supported Distributions**

VirtualMetric supports following distributions of Linux:

```markup
CentOS 5
CentOS 6
CentOS 7
CloudLinux 5
CloudLinux 6
CloudLinux 7
Debian 7
Debian 8
RedHat Enterprise Linux 5
RedHat Enterprise Linux 6
RedHat Enterprise Linux 7
Ubuntu 12.04
Ubuntu 14.04
```

***

## **Sizing**

Hardware requirements for VirtualMetric depends on total number of monitored object and intervals used. The following values are provided as reference for common usage of VirtualMetric (based on 20 seconds interval). Inventory collections are not included in this calculations.

### **Bare Metal**

*   _**Per Server**_

    a. 50 MB of memory (VirtualMetric Trigger)\
    b. 4 Kbps of bandwidth (VirtualMetric API)\
    c. 15 MB of disk space per month (VirtualMetric Database)

