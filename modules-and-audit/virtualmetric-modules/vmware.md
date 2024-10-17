# VMware

VMware is the monitoring module for VMware products including vCenter and vSphere. You can monitor performance counters and get inventory reports for your VMware Hosts and virtual machines.

<div align="left">

<figure><img src="../../.gitbook/assets/image (48).png" alt=""><figcaption></figcaption></figure>

</div>

You can reach VMware module monitoring and reports via left menu.

## _**Module Reports**_

VirtualMetric collects following inventory reports for VMware module.

**Bare Metal Reports**

```markup
Change Tracking
Event Log
Security Log
Firewall Log
Best Practices
TCP Connections
Services
Programs
Firewall Rules
Administrators
```

**Cluster Reports**

```markup
Distributed Switch
```

**Server Reports**

```markup
Standard Switch
Storage Paths
```

**Virtual Machine Reports**

```markup
Config
Snapshot
Services
```

## _**Module Counters**_

VirtualMetric collects following performance counters for VMware module.

**CPU**

```markup
Latency
Usage (%)
Demand
Co-stop
Usage (Mhz)
Used
Swapwait
Ready
Total Capacity
Reserved Capacity
Core Utilization
Wait
Idle
Utilization
```

**Memory**

```markup
Consumed
Decompression Rate
Low Free Threshold
Shared
Overhead
Host Cache Used for Swapping
Swap Out Rate for Host Cache
Total Capacity
Active Write
Swap Out to Host Cache
Zero
Memory Usage
Active
Compressed
Heap
Balloon
Unreserved
Compression Rate
Swap In
State
Swap Out
Shared Common
Swap In from Host Cache
Used by VMKernel
Swap Used
Swap In Rate
Reserved Capacity
Heap Free
Granted
Swap Out Rate
Swap In Rate from Host Cache
Latency
```

**Network**

```markup
Multicast Receives
Packet Receive Errors
Data Receive Rate
Broadcast Transmits
Multicast Transmits
Data Transmit Rate
Broadcast Receives
Data Received Rate
Network Usage
Packets Received
Packets Transmitted
Transmit Packets Dropped
Data Transmitted Rate
Unknown Protocol Frames
Packet Transmit Errors
Receive Packets Dropped
```

**Disk**

```markup
Write Rate
Command Latency
Kernel Read Latency
Commands Aborted
Kernel Write Latency
Read Rate
Commands Issued
Queue Write Latency
Kernel Command Latency
Average Read Requests per Second
Queue Command Latency
Maximum Queue Depth
Write Latency
Physical Device Read Latency
Read Requests
Average Commands Issued per Second
Queue Read Latency
Read Latency
Write Requests
Average Write Requests per Second
Bus Resets
Physical Device Write Latency
Physical Device Command Latency
```

**Datastore**

```markup
Read Latency
Average Write Requests per Second
Storage DRS Datastore Normalized Read Latency
Storage DRS Datastore Write IO Rate
Storage IO Control Active Time Percentage
Storage DRS Datastore Outstanding Read Requests
Storage DRS Datastore Outstanding Write Requests
Storage IO Control Datastore Maximum Queue Depth
Write Latency
Storage DRS Datastore Write Workload Metric
Storage DRS Datastore Bytes Written
Storage IO Control Normalized Latency
Write Rate
Storage IO Control Aggregated IOPS
Storage DRS Datastore Bytes Read
Datastore Latency Observed by VMs
Storage DRS Datastore Read IO Rate
Read Rate
Storage DRS Datastore Normalized Write Latency
Average Read Requests per Second
Storage DRS Datastore Read Workload Metric
```

**Power**

```markup
Energy Usage
Cap
Usage
```

**Storage Path**

```markup
Average Read Requests per Second
Average Command Issued per Second
Write Rate
Read Rate
Average Write Requests per Second
Read Latency
Write Latency
```

**Storage Adapter**

```markup
Average Read Requests per Second
Average Command Issued per Second
Write Rate
Read Rate
Average Write Requests per Second
Read Latency
Write Latency
```

**VM Processor**

```markup
Usage
Demand to Entitlement Ratio
Wait
Latency
Idle
Entitlement
Used
Usage in Mhz
Swap Wait
Demand
Run
Overlap
Ready
Max Limited
System
Co-Stop
```

**VM Memory**

```markup
Memory Saved by Zipping
Decompression Rate
Swapped
Overhead Touched
Balloon
Active
Shared
Entitlement
Host Cache Used for Swapping
Active Write
Reserved Overhead
Zipped Memory
Swap Out
Compressed
Balloon Target
Latency
Swap in Rate
Swap in Rate from Host Cache
Overhead
Consumed
Zero
Swap in
Compression Rate
Swap Target
Swap Out Rate to Host Cache
Swap Out Rate
Granted
Memory Usage
```

**VM Network**

```markup
Data Receive Rate
Packets Transmitted
Packets Received
Data Received Rate
Network Usage
Data Transmit Rate
Data Transmitted Rate
Broadcast Receives
Multicast Receives
Transmit Packets Dropped
Broadcast Transmits
Receive Packets Dropped
Multicast Transmits
```

**VM Virtual Disk**

```markup
Write Request Size
Read Latency
Write Workload Metric
Write Latency
Average Write Requests per Second
Number of Small Seeks
Average Number of Outstanding Read Requests
Average Read Requests per Second
Read Workload Metric
Number of Large Seeks
Read Request Size
Number of Medium Seeks
Average Number of Outstanding Write Requests
Write Rate
Read Rate
```

## _**User Permissions - vSphere**_

If you want to use non-administrator user for VMware operations, you need to add and configure the following User and Role permissions according to your environment.

**Creating User**

Create your user from Local Users & Groups tab.

Click Add New User and type new user information.

<div align="left">

<figure><img src="../../.gitbook/assets/image (49).png" alt="" width="563"><figcaption></figcaption></figure>

</div>

**Creating Role**

You need to create a new role for your user.

Go to Home view.

<div align="left">

<figure><img src="../../.gitbook/assets/image (50).png" alt="" width="563"><figcaption></figcaption></figure>

</div>

Click on Roles icon.

<div align="left">

<figure><img src="../../.gitbook/assets/image (51).png" alt="" width="460"><figcaption></figcaption></figure>

</div>

Click Add button to open dialog.

<div align="left">

<figure><img src="../../.gitbook/assets/image (52).png" alt="" width="266"><figcaption></figcaption></figure>

</div>

Assign the following permission to your user role:

```markup
Global > Settings
Host > CIM > CIM Interaction
Host > Configuration > System Management
Virtual Machine > Interaction > Console Interaction
```

\
For VMware 6.5 and later versions, you should also add following permission:

```markup
Virtual Machine > Interaction > Inject USB HID scan codes
```

\
After you add permissions, you will see following User Role view.

After that, you should add the new user to the user role as a member.

<div align="left">

<figure><img src="../../.gitbook/assets/image (53).png" alt="" width="563"><figcaption></figcaption></figure>

</div>

Click Add button, select the user and click OK button to apply changes.

<div align="left">

<figure><img src="../../.gitbook/assets/image (54).png" alt="" width="563"><figcaption></figcaption></figure>

</div>

## _**User Permissions - vCenter**_

If you want to use non-administrator user for vCenter operations, you need to add and configure the following User and Role permissions according to your environment.\
\
**Creating User**

First, we will start with adding a new user.

Go to Administration tab.

<div align="left">

<figure><img src="../../.gitbook/assets/image (55).png" alt=""><figcaption></figcaption></figure>

</div>

From Users and Groups section, click + button to add a new user.

<div align="left">

<figure><img src="../../.gitbook/assets/image (56).png" alt="" width="439"><figcaption></figcaption></figure>

</div>

**Creating Role**

Now you should add a new user role to configure permissions.

From Roles section, click + button to add new a Role.

<div align="left">

<figure><img src="../../.gitbook/assets/image (57).png" alt="" width="383"><figcaption></figcaption></figure>

</div>

On the dialog, expand the All Privileges section to add permissions.

<div align="left">

<figure><img src="../../.gitbook/assets/image (58).png" alt="" width="314"><figcaption></figcaption></figure>

</div>

Select the following Permissions from the list:

```markup
Global > Settings
Host > CIM > CIM Interaction
Virtual Machine > Interaction > Console Interaction
Virtual Machine > Interaction > Inject USB HID scan codes
```

After Role and User creation, you need to assign the User to the Role.

<div align="left">

<figure><img src="../../.gitbook/assets/image (59).png" alt="" width="563"><figcaption></figcaption></figure>

</div>

By default, the new user will have access to all objects in vCenter. If you want to narrow the scope, you can follow the steps below.

Go to Navigator and select Hosts and Clusters.

<div align="left">

<figure><img src="../../.gitbook/assets/image (60).png" alt=""><figcaption></figcaption></figure>

</div>

Switch to Permissions tab and complete User-Role Assignment for the scope.

<div align="left">

<figure><img src="../../.gitbook/assets/image (61).png" alt="" width="462"><figcaption></figcaption></figure>

</div>

