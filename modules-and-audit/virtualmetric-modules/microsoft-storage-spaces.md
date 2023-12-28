# Microsoft Storage Spaces

Storage Spaces is the monitoring module for Microsoft Storage Spaces and Storage Spaces Direct (S2D). You can monitor performance counters and get inventory reports for your Storage Spaces environments.

You can reach Storage Spaces module monitoring and reports via left menu.

<div align="left">

<figure><img src="../../.gitbook/assets/image (54).png" alt=""><figcaption></figcaption></figure>

</div>

## _**Module Reports**_

VirtualMetric collects following inventory reports for Storage Spaces module.

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
```

## _**Module Counters**_

VirtualMetric collects following performance counters for Storage Spaces module.\


**Processor**

```markup
% C1 Time
% C2 Time
% C3 Time
% DPC Time
% Idle Time
% Interrupt Time
% Privileged Time
% Processor Time
% User Time
C1 Transitions/sec
C2 Transitions/sec
C3 Transitions/sec
DPC Rate
DPCs Queued/sec
Interrupts/sec
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

**Cluster CSV Volume Cache**

```markup
Cache Size - Configured
Cache Size - Current
Disk IO Read - Bytes/Sec
Cache IO Read - Bytes/sec
LRU Cache Size - Current
LRU Cache Size - Target
```

## _**User Permissions**_

If you want to use non-administrator user for VirtualMetric, you need to add the following changes for the user account in addition to Bare Metal permissions.

**Cluster Access Permissions**

To enable Windows Failover Cluster monitoring, you need to run the code below:

```markup
Grant-ClusterAccess -User Domain\vmetricuser -ReadOnly
```

## _**Requirements**_

Following Windows features are required to monitor Microsoft Storage Spaces:

```markup
Failover Cluster Module for Windows PowerShell
```

You can install required features with following PowerShell command:

```markup
Get-WindowsFeature RSAT-Clustering-PowerShell | Add-WindowsFeature
```
