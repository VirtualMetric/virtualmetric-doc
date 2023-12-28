# Windows

Following modules could be used for Windows monitoring:

* &#x20;  Bare Metal
* &#x20;  Microsoft Hyper-V
* &#x20;  Storage Spaces
* &#x20;  Microsoft IIS Server
* &#x20;  Microsoft SQL Server

## **Requirements**

Following Windows components are required on Windows Servers for monitoring:

* &#x20;  Microsoft PowerShell v2 or later
* &#x20;  .NET Framework 2.0 or later

### **Remote Management Requirements for Windows Servers**

Remote Management is enabled by default for Windows Server 2012 R2 and later versions. If you want to monitor earlier versions of Windows, you should enable Remote Management to allow agentless monitoring.\
\
To enable Remote Management, please start a PowerShell with Administrator rights and execute following commands.\
\
1\. Enable PSRemoting. You should enter Y for all questions.\
\
`Enable-PSRemoting`\
\
2\. Configure WinRM Max Envelope Size. _(Optional)_\
\
`Set-Item WSMan:\localhost\MaxEnvelopeSizekb 1024`\
\
3\. Configure WinRM Max Memory Per Shell. _(Optional)_\
\
`Set-Item WSMan:\localhost\Shell\MaxMemoryPerShellMB 2048`

### **Remote Management Requirements for Windows Desktop Clients**

If you want to monitor Desktop versions of Windows, you should enable Remote Management to allow agentless monitoring.\
\
To enable Remote Management, please start a PowerShell with Administrator rights and execute following commands.\
\
1\. Enable PSRemoting. You should enter Y for all questions.\
\
`Enable-PSRemoting -SkipNetworkProfileCheck -Force`\
\
2\. Configure Windows Firewall Rule. _(Optional)_\
\
`Set-NetFirewallRule –Name "WINRM-HTTP-In-TCP-PUBLIC" –RemoteAddress Any`

***

## **Supported Versions**

VirtualMetric supports following versions of Windows:

```markup
Windows Server 2003 R2
Windows Server 2008
Windows Server 2008 R2
Windows Server 2012
Windows Server 2012 R2
Windows Server Core 2008 R2
Windows Server Core 2012
Windows Server Core 2012 R2
Windows Server 2016
Windows Server Core 2016
Windows Server 2019
Windows Server Core 2019
Windows Nano Server
Windows 7
Windows 8
Windows 10
```

***

## **Sizing**

Hardware requirements for VirtualMetric depends on total number of monitored object (Hyper-V VM, Microsoft IIS WebSite, Microsoft SQL Server Database etc.) and intervals used. The following values are provided as reference for common usage of VirtualMetric (based on 20 seconds interval). Inventory collections are not included in this calculations.

### **Bare Metal**

*   _**Per Server**_

    a. 50 MB of memory (VirtualMetric Trigger)\
    b. 4 Kbps of bandwidth (VirtualMetric API)\
    c. 15 MB of disk space per month (VirtualMetric Database)

### **Microsoft Hyper-V**

*   _**Per Host**_

    a. 50 MB of memory (VirtualMetric Trigger)\
    b. 4 Kbps of bandwidth (VirtualMetric API)\
    c. 15 MB of disk space per month (VirtualMetric Database)
*   _**Per Virtual Machine**_

    a. 5 KB of memory (VirtualMetric Database)\
    b. 4 Kbps of bandwidth (VirtualMetric API)\
    c. 20 MB of disk space per month (VirtualMetric Database)

### **Microsoft IIS Server**

*   _**Per Server**_

    a. 50 MB of memory (VirtualMetric Trigger)\
    b. 8 Kbps of bandwidth (VirtualMetric API)\
    c. 20 MB of disk space per month (VirtualMetric Database)
*   _**Per Web Site**_

    a. 5 KB of memory (VirtualMetric Database)\
    b. 16 Kbps of bandwidth (VirtualMetric API)\
    c. 30 MB of disk space per month (VirtualMetric Database)

### **Microsoft SQL Server**

*   _**Per Server**_

    a. 50 MB of memory (VirtualMetric Trigger)\
    b. 32 Kbps of bandwidth (VirtualMetric API)\
    c. 50 MB of disk space per month (VirtualMetric Database)
*   _**Per Database**_

    a. 10 KB of memory (VirtualMetric Database)\
    b. 24 Kbps of bandwidth (VirtualMetric API)\
    c. 40 MB of disk space per month (VirtualMetric Database)

***

## **Proxy Configuration**

If you use proxy configuration on Windows Server, you may need to add exception for VirtualMetric.

1\.      Go to Notification Center and click All Settings.

<div align="left">

<figure><img src="../.gitbook/assets/image (123).png" alt="" width="345"><figcaption></figcaption></figure>

</div>

2\.      To edit proxy exception list, click to Proxy and type your VirtualMetric API address. After changes, click Save button to apply changes.

<div align="left">

<figure><img src="../.gitbook/assets/image (124).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

***

## **Double Hop Configuration**

You may have following error when you try to monitor a Hyper-V Cluster or Standalone Server which uses Storage Spaces Scale Out File Server as storage.

```powershell
Cannot find path '\\S2DSMB\Gold\Test.vhdx' because it does not exist.
    + CategoryInfo          : ObjectNotFound: (\\S2DSMB\Gold\Test.vhdx:String)
    [Get-Item], ItemNotFoundException
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.Commands.GetIt
   emCommand
    + PSComputerName        : vmetric-s2d-hv.virtualmetric.com
```

Due to Double-Hop issue, VirtualMetric is not able reach to Storage Spaces File Share.

1\.      To fix this issue, you should give delegation on S2DSMB File-Share account with PowerShell.

{% code overflow="wrap" lineNumbers="true" %}
```powershell
$SOFSSMB = Get-ADComputer "S2DSMB" # This is your Scale Out File Server
$SOFSHV = Get-ADComputer "vmetric-s2d-hv" # This is your Hyper-V Host
Set-ADComputer -Identity $SOFSSMB -PrincipalsAllowedToDelegateToAccount @($SOFSHV) # Set delegation for Hyper-V host on SMB file share account
```
{% endcode %}

{% hint style="info" %}
You don't need to do this operation on all SOFS Cluster Members, but only for SOFS File Share.
{% endhint %}

2\.      After this operation, you may need to clear Kerberos cache to apply changes immediately.

```powershell
klist purge -li 0x3e7
```

3\.      You should clear Kerberos cache on all Hyper-V Hosts and SOFS Cluster members. Otherwise you may have to wait 15 minutes.

<div align="left">

<figure><img src="../.gitbook/assets/image (125).png" alt=""><figcaption></figcaption></figure>

</div>

4\.      You may still have Access Denied messages after clearing Kerberos Cache. If your user account has no privilege on SOFS Cluster nodes, you should give permission on nodes.

<div align="left">

<figure><img src="../.gitbook/assets/image (126).png" alt=""><figcaption></figcaption></figure>

</div>

5\.      Make sure that your user account has Local Administrator privilege on SOFS Nodes.
