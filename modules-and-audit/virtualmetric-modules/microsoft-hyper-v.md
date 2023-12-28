# Microsoft Hyper-V

Microsoft Hyper-V is the monitoring module for Microsoft Hyper-V Server. You can monitor performance counters and get inventory reports for your Hyper-V Servers and virtual machines.

<div align="left">

<figure><img src="../../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>

</div>

You can reach Microsoft Hyper-V module monitoring and reports via left menu.

## _**Module Reports**_

VirtualMetric collects following inventory reports for Microsoft Hyper-V module.\


**Bare Metal Reports**

```markup
Change Tracking
Event Log
Security Log
Firewall Log
Best Practices
Pending Updates
TCP Connections         
Security Threats
File Change Tracking
User Sessions
Processes
Services
Hotfix
Programs
Windows Features         
Windows Defender
Firewall Rules
Network Teaming
Startup Commands
Local DNS Records
Administrators
```

**Cluster Reports**

```markup
Cluster Network
Cluster Aware Update
Replica Broker
```

**Server Reports**

```markup
Config
Virtual Switch
vHBA Switch
VM Migration Network
```

**Virtual Machine Reports**

```markup
Config
Snapshot
Services
Replica Config
Replica Health
```

## _**Module Counters**_

VirtualMetric collects following performance counters for Microsoft Hyper-V module.\


**Hyper-V Hypervisor Logical Processor**

```markup
% Guest Run Time
% Hypervisor Run Time
% Idle Time
% Total Run Time
Context Switches/Sec
Total Interrupts/Sec
```

**Memory**

```markup
Available MBytes
Pages/Sec
Page Faults/Sec
% Committed Bytes In Use
Free System Page Table Entries
Pool Nonpaged Bytes
Pool Paged Bytes
```

**Paging File**

```markup
% Usage
```

**Network Interface**

```markup
Bytes Received/Sec
Bytes Sent/Sec
Packets Received/Sec
Packets Sent/Sec
Output Queue Length
```

**Hyper-V Virtual Switch**

```markup
Bytes Received/Sec
Bytes Sent/Sec
Packets Received/Sec
Packets Sent/Sec
```

**LogicalDisk**

```markup
Disk Reads/Sec
Disk Writes/Sec
Disk Read Bytes/Sec
Disk Write Bytes/Sec
% Idle Time
Split IO/Sec
Current Disk Queue Length
Avg. Disk Read Queue Length
Avg. Disk Write Queue Length
Avg. Disk Sec/Read
Avg. Disk Sec/Write
```

**PhysicalDisk**

```markup
Disk Reads/Sec
Disk Writes/Sec
Disk Read Bytes/Sec
Disk Write Bytes/Sec
% Idle Time
Split IO/Sec
Current Disk Queue Length
Avg. Disk Read Queue Length
Avg. Disk Write Queue Length
Avg. Disk Sec/Read
Avg. Disk Sec/Write
```

**Cluster CSV File System**

```markup
IO Reads/Sec
IO Writes/Sec
IO Read Bytes/Sec
IO Write Bytes/Sec
Redirected Reads/Sec
Redirected Writes/Sec
Redirected Read Bytes/sec
Redirected Write Bytes/sec
Read Queue Length
Write Queue Length
Read Latency
Write Latency
Redirected Read Queue Length
Redirected Write Queue Length
Redirected Read Latency
Redirected Write Latency
Disk IO Reads/Sec
Cache Read/Sec
```

**Hyper-V Hypervisor Virtual Processor**

```markup
% Guest Run Time
% Hypervisor Run Time
% Total Run Time
```

**Hyper-V Dynamic Memory VM**

```markup
Average Pressure
Current Pressure
Guest Visible Physical Memory
Maximum Pressure
Minimum Pressure
Physical Memory
Smart Paging Working Set Size
```

**Hyper-V Virtual Network Adapter**

```markup
Bytes Received/Sec
Bytes Sent/Sec
Packets Received/Sec
Packets Sent/Sec
```

**Hyper-V Virtual Storage Device**

```markup
Queue Length
Read Count
Write Count
Read Bytes/Sec
Write Bytes/Sec
Read Operations/Sec
Write Operations/Sec
```

**Cluster CSV Volume Cache**

```markup
Cache Size - Configured
Cache Size - Current
Disk IO Read - Bytes/Sec
Cache IO Read - Bytes/sec
LRU Cache Size - Current
LRU Cache Size - Target
```

## _**Feature Limitations**_

Following features are not supported for Hyper-V v2 on Windows Server 2008 R2 due to Hyper-V limitations:

* **Dynamic Memory Monitoring:** Dynamic Memory Performance Counters are not available on Windows Server 2008 R2: Hyper-V.
* **Queue Length for Virtual Disk:** Queue Length Performance Counter is not available on Windows Server 2008 R2: Hyper-V.
* **vHBA Reports:** Virtual HBA is not supported on Windows Server 2008 R2: Hyper-V
* **Hyper-V Replica:** Hyper-V Replica is not supported on Windows Server 2008 R2: Hyper-V.
* **Live Storage Migration Settings:** Live Storage Migration is not supported on Windows Server 2008 R2: Hyper-V.
* **Virtual Disk Sharing:** Virtual Disk Sharing is not supported on Windows Server 2008 R2: Hyper-V.
* **Virtual Disk IO Limits:** Virtual Disk IO limitation is not supported on Windows Server 2008 R2: Hyper-V.
* **Limited Host Network Adapter Features:** RSS, VMQ, TCP Offload features are not supported on Windows Server 2008 R2.
* **Smart Paging File:** Smart Paging File feature is not supported on Windows Server 2008 R2: Hyper-V.
* **Virtual Machine Guest Services:** Virtual Machine Guest Service Interface Service is not supported on Windows Server 2008 R2: Hyper-V.
* **Virtual Memory Limitations:** Memory Buffer feature is not supported on Windows Server 2008 R2: Hyper-V.
* **VM Config Limitations:** VM Operational Status is not supported on Windows Server 2008 R2: Hyper-V.
* **Cluster Shared Volumes Counters:** Read/Write Queue Length and Read/Write Latency counters are not supported on Windows Server 2008 R2: Hyper-V.

## _**User Permissions**_

If you want to use non-administrator user for VirtualMetric, you need to add the following changes for the user account in addition to Bare Metal permissions.

**User Group Membership**

```markup
Hyper-V Administrators
```

Go to user properties and add groups into Member Of section:

<div align="left">

<figure><img src="../../.gitbook/assets/image (31).png" alt="" width="314"><figcaption></figcaption></figure>

</div>

**Cluster Access Permissions**

To enable Windows Failover Cluster monitoring, you need to run the code below:

```markup
Grant-ClusterAccess -User Domain\vmetricuser -ReadOnly
```

## _**Requirements**_

Following Windows features are required to monitor Microsoft Hyper-V:

```markup
Failover Cluster Module for Windows PowerShell
Hyper-V Module for Windows PowerShell
```

\
You can install required features with following PowerShell command:

```markup
Get-WindowsFeature RSAT-Clustering-PowerShell,Hyper-V-PowerShell | Add-WindowsFeature
```

