# Bare Metal

Bare Metal is the default server monitoring module of VirtualMetric. VirtualMetric uses standardized performance counters, so you can monitor Windows, VMware and Linux servers on same charts and reports.

You can reach Bare Metal module monitoring and reports via left menu.

## _**Module Reports**_

VirtualMetric collects following inventory reports for Bare Metal module.

**Hardware: General**

```markup
OS Name
OS Version
Manufacturer
Model
Serial Number
Management IP Address
Chassis Name
Chassis Slot
Chassis IP Address
Chassis Serial Number
Power Plan
UAC Status
Firewall Status
Last Reboot Date
Pending Update
```

**Hardware: Processor**

```markup
CPU Index
Name
Device Id
Description
Family
Cores
Logical Processors
Max Clock Speed
L2 Cache Size
L3 Cache Size
Manufacturer
Status
Health State
```

**Hardware: Memory**

```markup
Device Locator
Name
Description
Manufacturer
Model
Part Number
Serial Number
Capacity
Speed
Status
Health State
```

**Hardware: Volume**

```markup
Volume Id
Name
Volume Name
Volume Type
Number
Label
State
Block Size
Signature
Serial Number
Model
Firmware Revision
Volume Dirty
Storage Name
Storage Id
Status
```

**Hardware: Disk Drive**

```markup
Name
Description
Serial Number
Operational Status
```

**Hardware: Array Controller**

```markup
Name
Serial Number
Cache Size
Cache Serial Number
Operational Status
```

**Hardware: HBA**

```markup
Description
Manufacturer
Model
Serial Number
Driver Name
Driver Version
Firmware Version
Option Rom Version
Node WWN
Port WWN
Identifier
Operational Status
```

**Hardware: Network Adapter**

```markup
Name
Mac Address / Permanent Address
IPv4/IPv6 Address
Link Speed / Speed
Jumbo Frames
IP/TCP/UDP IPv4 Checksum Offload
TCP/UDP IPv6 Checksum Offload
RSS/VMQ Enabled
Media Connection State
Driver Provider/Version/Date
NDIS Version
Full Duplex
Device Wake Up Enable
MTU Size
VLAN Id
Status/Health State
```

**Hardware: FAN**

```markup
Name
Operational Status
Health State
```

**Hardware: Power Supply**

```markup
Name
Part Number
Operational Status
Health State
```

**Server Reports**

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

## _**Module Counters**_

VirtualMetric collects following performance counters for Bare Metal module.\


**Processor**

```markup
Processor Load
Processor Usage
Total Socket Count
Total Number of Cores
Total Number of Logical Processors
Current Clock Speed
Current Voltage
```

**Memory**

```markup
% Memory Usage
Memory Usage
Total Memory
Free Memory
Swap Usage
```

**Network**

```markup
Received Throughput
Sent Throughput
Total Throughput
Received Bandwidth
Sent Bandwidth
Total Bandwidth
Received Packets
Sent Packets
Total Packets
Received Packets Dropped
Sent Packets Dropped
Total Packets Dropped
Packets Outbound Discarded
Packets Received Discarded
Packets Outbound Errors
Packets Received Errors
Current Bandwidth
```

**Storage**

```markup
% Storage Usage
Storage Usage
Total Storage
Free Storage
Read IOPS
Write IOPS
Total IOPS
Read Throughput
Write Throughput
Total Throughput
Read Latency
Write Latency
Total Latency
```

**System**

```markup

CPU Temperature
Ambient Temperature
Server Pending Reboot
Server Ping Check
```

**Event Log**

```markup
Critical Event Count
Error Event Count
Warning Event Count
Information Event Count
```

**Authentication**

```markup
Successful Login Count
Failed Login Count
```

**Session**

```markup
RDP Connection Count
SSH Connection Count
WSMan Connection Count
TCP Connection Count
```

**Update**

```markup
Critical Update Count
Important Update Count
Other Update Count
```

## _**User Permissions**_

If you want to use non-privileged user for VirtualMetric, you need to do following changes for the user account.

## _**Windows User Permissions**_

**User Group Membership**

```markup
Event Log Readers
Remote Management Users
Performance Log Users
Performance Monitor Users
```

Go to user properties and add groups into Member Of section:

<div align="left">

<figure><img src="../../.gitbook/assets/image (32).png" alt="" width="314"><figcaption></figcaption></figure>

</div>

Remote Management Users group is required for remote agentless connection. Alternatively, you can restrict the user with readonly permissions. Open PowerShell console and type following command:

```markup
Set-PSSessionConfiguration -Name Microsoft.PowerShell -showSecurityDescriptorUI
```

Type **y** and press **Enter** to continue.

<div align="left">

<figure><img src="../../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

</div>

Add the user and select Read and Execute permissions. Click Submit to apply changes.

<div align="left">

<figure><img src="../../.gitbook/assets/image (34).png" alt="" width="563"><figcaption></figcaption></figure>

</div>

PowerShell will ask you to restart WinRM service. Type y and press Enter to confirm.

<div align="left">

<figure><img src="../../.gitbook/assets/image (35).png" alt="" width="563"><figcaption></figcaption></figure>

</div>

After this operation, you can remove Remote Management Users from the user membership.

**Security Logs Permissions**

To collect security logs you need to give acces to following Registry key for VirtualMetric user.

```markup
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\services\eventlog\Security
```

<div align="left">

<figure><img src="../../.gitbook/assets/image (36).png" alt="" width="272"><figcaption></figcaption></figure>

</div>

**WMI Security Permissions**

```markup
CIMV2
Hardware
LsiMr13 (Dell Hardware Only)
StandardCimv2
```

Go to Computer Manager to set WMI security permissions.

Right click on WMI Control and click Properties to open dialog.

<div align="left">

<figure><img src="../../.gitbook/assets/image (37).png" alt="" width="563"><figcaption></figcaption></figure>

</div>

Go to Security tab, select CIMV2 and click Security button.

<div align="left">

<figure><img src="../../.gitbook/assets/image (38).png" alt="" width="563"><figcaption></figcaption></figure>

</div>

Add your user account and select Allow permission for Enable Account and Remote Enable properties and select Advanced.

<div align="left">

<figure><img src="../../.gitbook/assets/image (39).png" alt="" width="563"><figcaption></figcaption></figure>

</div>

Select user and click Edit.

<div align="left">

<figure><img src="../../.gitbook/assets/image (40).png" alt="" width="563"><figcaption></figcaption></figure>

</div>

Select This namespace and subnamespaces and click OK button.

<div align="left">

<figure><img src="../../.gitbook/assets/image (41).png" alt="" width="563"><figcaption></figcaption></figure>

</div>

{% hint style="info" %}
Please repeat the steps for the other WMI namespaces on the list.
{% endhint %}

**Windows Firewall Configuration**

```markup
netsh firewall set service RemoteAdmin enable (Deprecated)
netsh advfirewall firewall set rule group="Remote Administration" new enable=yes
```

Enable Remote Administration on Windows Firewall:

<figure><img src="../../.gitbook/assets/image (42).png" alt=""><figcaption></figcaption></figure>

**Service Control Manager Configuration**

You need to open CMD window to configure security descriptor for Service Control Manager. Type following command on CMD:

```markup
sc sdshow scmanager
```

You will see default security descriptor of the Service Control Manager.

<div align="left">

<figure><img src="../../.gitbook/assets/image (43).png" alt="" width="510"><figcaption></figcaption></figure>

</div>

Find the security descriptor for VirtualMetric user:

```markup
wmic useraccount where name='virtualmetric' get sid
S-1-5-21-3132494459-2649941077-65550600-1000
```

And create the following key:

```markup
(A;;CCLCRPRC;;;S-1-5-21-3132494459-2649941077-65550600-1000)
```

<div align="left">

<figure><img src="../../.gitbook/assets/image (44).png" alt=""><figcaption></figcaption></figure>

</div>

Update the Security Description via following command with VirtualMetric user key added:

{% code overflow="wrap" lineNumbers="true" %}
```markup
sc sdset SCMANAGER D:(A;;CC;;;AU)(A;;CCLCRPRC;;;IU)(A;;CCLCRPRC;;;SU)(A;;CCLCRPWPRC;;;SY)(A;;KA;;;BA)(A;;CCLCRPRC;;;S-1-5-21-3132494459-2649941077-65550600-1000)S:(AU;FA;KA;;;WD)(AU;OIIOFA;GA;;;WD)
```
{% endcode %}

<div align="left">

<figure><img src="../../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

</div>

You need to restart WinRM service to activate security description changes.

## _**Linux User Permissions**_

**Creating User**

```markup
useradd -m virtualmetric
```

{% hint style="info" %}
Please make sure to use "-m" parameter to create users home directory. If your user does not have access to "/tmp" folder you need to specify tmp path while adding the host to VirtualMetric. Example: "/home/virtualmetric/tmp"
{% endhint %}

After creating the user you can set user password like below;

```markup
passwd virtualmetric
```

For some of data collection you can add the following executable file paths to sudoers file.

```markup
dmidecode ( Memory Inventory Information )
journalctl ( Event Log Collection )
ss ( TCP Connection Collection )
```

{% hint style="info" %}
To find the file path you can use "which" command and add the outpath directory to sudoers.
{% endhint %}

To add the file permission to sudo you can use visudo (visudo will check for any type errors in case there is any instead of directly editing the "/etc/sudoers" file. )

```markup
virtualmetric ALL = NOPASSWD: /usr/sbin/dmidecode,/usr/bin/journalctl,/usr/sbin/ss
```

