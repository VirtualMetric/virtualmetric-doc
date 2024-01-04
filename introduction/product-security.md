# Product Security

VirtualMetric uses Microsoft IIS Server as the Web Server, so you are able to make VirtualMetric Dashboard and VirtualMetric API always up to date and secure via Microsoft Update. VirtualMetric also uses Microsoft SQL Server as the Database Server and stores user, inventory and monitoring data in it. So you can use Microsoft Authentication and Encryption methods to make Microsoft SQL Server secure as well.\
\
We put a lot of effort to make VirtualMetric suitable for enterprises to pass their network and security policies. First of all, VirtualMetric does not require an agent to connect servers. This is a great advantage for enterprises because VirtualMetric does not touch any system files, does not require any registry changes, or does not load any DLLs or Drivers on monitored servers, so it will help you on security scans since there is no system changes on your servers by VirtualMetric. VirtualMetric remotely connects Windows, VMware and Linux servers to collect monitoring and inventory data. So we focused to make this remote connection as secure as possible. We can explain these efforts in a few sections.

***

## **Authentication**

VirtualMetric allows you to use two different authentication methods to connect servers: **Basic** and **Active Directory**.

* If you setup VirtualMetric on a Active Directory member server, you can start VirtualMetric Collector with a privileged account on Active Directory. By doing this, you won't need to type any username/password on VirtualMetric to connect servers which are members in the same Active Directory.
* If you want to use Basic Authentication to connect servers, VirtualMetric uses The Advanced Encryption Standard or AES with a 128-bit key to encrypt your passwords. It is one of the most secure encryption methods used in most modern encryption algorithms and technologies. 128-bit encryption is considered to be logically unbreakable.

<table data-full-width="false"><thead><tr><th></th><th align="center">Password in Database?</th><th align="center">Password Security</th></tr></thead><tbody><tr><td>Active Directory Authentication</td><td align="center">No</td><td align="center">No</td></tr><tr><td>Basic Authentication</td><td align="center">Yes</td><td align="center">AES 128-bit</td></tr></tbody></table>

{% hint style="info" %}
We suggest you to prefer Active Directory Authentication if it's possible to use on your environment.
{% endhint %}

When you create a user to connect VirtualMetric API or Dashboard, we also encrypt your user passwords with MD5 hashing. So instead of storing clear text passwords, VirtualMetric Databases only contains MD5 hashes of your passwords. When a user tries to logon VirtualMetric, we only send MD5 hash via network traffic.

***

## Encryption

The communication between VirtualMetric and monitored server is encrypted at the protocol layer. When VirtualMetric connects to your servers, we use SSL protocol to protect your sensitive data from unwanted eyes on your network.\
\


<table><thead><tr><th width="134">Platform</th><th width="200" align="center">Secure Authentication</th><th width="222" align="center">Encrypted Data Transfer</th><th align="center">SSL Supported?</th></tr></thead><tbody><tr><td>Windows</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td></tr><tr><td>VMware</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td></tr><tr><td>Linux</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td></tr></tbody></table>

***

## **Connection Protocols**

If you use Active Directory authentication for Windows Servers, VirtualMetric uses PowerShell Remoting to connect servers. PowerShell Remoting is a solution to some of the security and consistency issues that IT professionals currently work around. It’s built on Microsoft’s implementation of the Web Services for Management (WSMan) protocol, and it uses the Windows Remote Management (WinRM) service to manage communication and authentication. This framework was designed to be a secure and reliable method for managing computers that’s built on well-known standards like Simple Object Access Protocol (SOAP) and Hypertext Transfer Protocol (HTTP). The communication between VirtualMetric and monitored server is encrypted at the protocol layer, except when basic access authentication is used, which is intended for use with Hypertext Transfer Protocol Secure (HTTPS) sessions. Since we use WinRM, you can always configure WinRM security, change encryption type and you can set SSL certificate to make communication even more secure.\
\
For VMware Servers, VirtualMetric uses VMware vSphere Web Services to connect Hosts. By default, VirtualMetric uses SSL protocol to connect VMware Hosts. But you can always change communication protocol for VMware Hosts as well.\
\
For Linux Servers, VirtualMetric uses SSH to connect servers. You can use basic authentication or key-based authentication to connect your Linux servers. VirtualMetric supports RSA and DSA private keys. You can also use pass phrase for your keys.\


<table><thead><tr><th width="159">Platform</th><th>Connection Protocol</th><th align="center">Firewall Friendly?</th><th>Supported Protocols</th></tr></thead><tbody><tr><td>Windows</td><td>WS-Man</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>HTTP / HTTPS</td></tr><tr><td>VMware</td><td>SOAP</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>HTTP / HTTPS</td></tr><tr><td>Linux</td><td>SSH / SCP</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>SSH / SCP</td></tr></tbody></table>

***

## Required Firewall Ports

We designed VirtualMetric to become a Firewall friendly monitoring solution. Many monitoring solution on the market requires RPC/DCOM/SNMP protocols to monitor servers. Because of their protocols, they usually requires complex firewall configurations due to their dynamic ports requirements. VirtualMetric only uses HTTP/HTTPS protocols to connect Windows and VMWare Servers. For Linux servers, VirtualMetric uses secure shell (SSH) protocol for connection. So you can easily configure access via Firewall.

**Client Access to VirtualMetric Dashboard**

<div align="left">

<figure><img src="../.gitbook/assets/image (186).png" alt="" width="343"><figcaption></figcaption></figure>

</div>

<table><thead><tr><th width="127">Source</th><th>Destination</th><th>Protocol</th><th>Ports</th><th>Action</th></tr></thead><tbody><tr><td>Client</td><td>VirtualMetric Dashboard</td><td>TCP</td><td>80/443</td><td>ALLOW</td></tr><tr><td>Client</td><td>VirtualMetric API</td><td>TCP</td><td>8080</td><td>ALLOW</td></tr></tbody></table>

**Server Monitoring**

<div align="left">

<figure><img src="../.gitbook/assets/image (185).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

<table><thead><tr><th>Source</th><th>Destination</th><th width="119">Protocol</th><th>Ports</th><th>Action</th></tr></thead><tbody><tr><td>VirtualMetric Trigger</td><td>VirtualMetric API</td><td>TCP</td><td>8080</td><td>ALLOW</td></tr><tr><td>VirtualMetric Trigger</td><td>Windows Server</td><td>TCP</td><td>5985/5986</td><td>ALLOW</td></tr><tr><td>VirtualMetric Trigger</td><td>VMware Server</td><td>TCP</td><td>80/443</td><td>ALLOW</td></tr><tr><td>VirtualMetric Trigger</td><td>Linux Server</td><td>TCP</td><td>22</td><td>ALLOW</td></tr><tr><td>VirtualMetric Trigger</td><td>Network Device</td><td>UDP</td><td>161</td><td>ALLOW</td></tr><tr><td>Windows / VMware / Linux Server</td><td>VirtualMetric API</td><td>TCP</td><td>8080</td><td>ALLOW</td></tr><tr><td>sFlow Endpoint</td><td>VirtualMetric Trigger</td><td>UDP</td><td>6343</td><td>ALLOW</td></tr><tr><td>NetFlow Endpoint</td><td>VirtualMetric Trigger</td><td>UDP</td><td>2055</td><td>ALLOW</td></tr><tr><td>IPFIX Endpoint</td><td>VirtualMetric Trigger</td><td>UDP</td><td>4739</td><td>ALLOW</td></tr></tbody></table>

