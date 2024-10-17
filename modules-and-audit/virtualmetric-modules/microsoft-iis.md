# Microsoft IIS

Microsoft IIS is the monitoring module for Microsoft IIS Server. You can monitor performance counters and get inventory reports for your IIS Servers and web sites.

<div align="left">

<figure><img src="../../.gitbook/assets/image (62).png" alt=""><figcaption></figcaption></figure>

</div>

You can reach Microsoft IIS module monitoring and reports via left menu.

## _**Module Reports**_

VirtualMetric collects following inventory reports for Microsoft IIS module.

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

**Server Reports**

```markup
Application Pools
Application Pools Limits
Application Pools Recycling
```

**Web Site Reports**

```markup
Config
Binding
ASP
Compression
Redirection
Security
Logging
```

## _**Module Counters**_

VirtualMetric collects following performance counters for Microsoft IIS module.\


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

**Process**

```markup
% Privileged Time
% Processor Time
% User Time
IO Read Operations/sec
IO Write Operations/sec
IO Data Operations/sec
IO Read Bytes/sec
IO Write Bytes/sec
IO Data Bytes/sec
Working Set - Private
Private Bytes
Handle Count
```

**Web Service**

```markup
Bytes Received/sec
Bytes Sent/sec
Current Connections
Files Received/sec
Files Sent/sec
Get Requests/sec
Post Requests/sec
```

**ASP.NET**

```markup
Application Restarts
Applications Running
Worker Process Restarts
Request Wait Time
Requests Rejected
Requests Disconnected
Requests Queued
State Server Sessions Active
```

**ASP.NET Applications**

```markup
Requests/Sec
Sessions Total
Cache Total Hits
Cache Total Misses
Cache Total Turnover Rate
Errors During Preprocessing
Errors During Compilation
Errors During Execution
Errors Unhandled During Execution
Errors Total
Requests Failed
Requests Not Found
Requests Not Authorized
Requests Timed Out
```

**.NET CLR Exceptions**

```markup
# of Exceps Thrown
# of Exceps Thrown/Sec
# of Filters/Sec
# of Finallys/Sec
Throw to Catch Depth/Sec
```

## _**Feature Limitations**_

Following features are not supported for IIS module on Windows Server 2003 R2 due to IIS v6 limitations:

* Site Redirections: Web Site redirection feature is not supported on IIS 6.
* Application Pool Limitations: Log Event On Process Model is not supported on IIS 6.
* SSL Certificates: SSL support is not available for Web Site Bindings due to Windows Server 2003 R2 limitations.
* Web Site Trust Levels: .NET Trust Levels are not supported on IIS 6.

## _**Requirements**_

Following Windows features are required to monitor Microsoft IIS:

```markup
IIS Management Console
```

\
You can install required features with following PowerShell command:

```markup
Get-WindowsFeature Web-Mgmt-Console | Add-WindowsFeature
```
