# Active Directory User Permissions

You need to create a user and add user to the following groups:

```markup
Event Log Readers
Remote Management Users
Performance Log Users
Performance Monitor Users
```

{% hint style="info" %}
For IIS monitoring User must have Administrative Privileges.
{% endhint %}

After you add the VirtualMetric user to the groups. You need to add this user to the following WMI Namespaces:

**WMI Security Permissions**

```markup
CIMV2
Hardware
LsiMr13 (Dell Hardware Only)
StandardCimv2
```

\
You can use the following script to add the user on computers you wish to add to VirtualMetric:\


| Script Name                     |                                                                                                                |
| ------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| VirtualMetric Permission Script | [Download](https://s3.eu-central-1.amazonaws.com/download.virtualmetric.com/VirtualMetricPermissionScript.zip) |

\
You need to update the DOMAIN\USER with the user you configured before. These permission will give access to get hardware data from the server :

```markup
    Set-WmiNamespaceSecurity root/cimv2 add DOMAIN\USER Enable,RemoteAccess
    Set-WmiNamespaceSecurity root/hardware add DOMAIN\USER Enable,RemoteAccess
    Set-WmiNamespaceSecurity root/standardcimv2 add DOMAIN\USER Enable,RemoteAccess
```

\
These permissions will allow to read Windows Service Status. You need to change USER to the username you created before:

{% code overflow="wrap" lineNumbers="true" %}
```markup
$sid = invoke-command -scriptblock {cmd.exe /c 'wmic useraccount where name="USER" get sid'} | where {$_ -ne "" -and $_ -notlike "SID*"}
```
{% endcode %}

To Read Security logs you need to give Read access to following key:

```markup
    HKLM:\SYSTEM\CurrentControlSet\services\eventlog\Security
```

Inside the script update the User from the following line:

```markup
$idRef = [System.Security.Principal.NTAccount]("DOMAIN\USER")
```

**MSSQL Service Configuration**

If you want to use non-administrator user for VirtualMetric, you need to add the following changes for the user account in addition to Bare Metal permissions.\
\
You need to open CMD window to configure Security Descriptions for MSSQLSERVER Service. Type following command on CMD:

```markup
sc sdshow mssqlserver
```

<div align="left">

<figure><img src="../../.gitbook/assets/image (55).png" alt="" width="502"><figcaption></figcaption></figure>

</div>

You will see default security descriptor of the MSSQLSERVER Service.\
\
Add the following security descriptor to MSSQLSERVER security descriptions:

```markup
(A;;CCLCRPRCLO;;;AU)
```

Update the Security Description via following command:

{% code overflow="wrap" lineNumbers="true" %}
```markup
sc sdset MSSQLSERVER D:(A;;CCLCRPRCLO;;;AU)(A;;CCLCRPRC;;;IU)(A;;CCLCRPRC;;;SU)(A;;CCLCRPWPRC;;;SY)(A;;KA;;;BA)(A;;CC;;;AC)S:(AU;FA;KA;;;WD)(AU;OIIOFA;GA;;;WD)
```
{% endcode %}

<div align="left">

<figure><img src="../../.gitbook/assets/image (56).png" alt="" width="502"><figcaption></figcaption></figure>

</div>

**SSMS User Configurations**

Using SSMS add user to Server Logins:

<div align="left">

<figure><img src="../../.gitbook/assets/image (57).png" alt=""><figcaption></figcaption></figure>

</div>

Choose user and click OK button:

<div align="left">

<figure><img src="../../.gitbook/assets/image (58).png" alt="" width="520"><figcaption></figcaption></figure>

</div>

From Securables tab select Search and choose The Server selection.

<div align="left">

<figure><img src="../../.gitbook/assets/image (59).png" alt="" width="521"><figcaption></figcaption></figure>

</div>

And enable the following permissions:

**Login Securable Options**

```
Connect Any Database
View any database
View any definition
View server state
```

<div align="left">

<figure><img src="../../.gitbook/assets/image (917).png" alt="" width="518"><figcaption></figcaption></figure>

</div>
