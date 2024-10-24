---
hidden: true
---

# High Availability Components

You can install two or more VirtualMetric roles that work together to form a high availability monitoring system. The objective is to reach true 100% uptime for the monitoring tool. By clustering, the uptime will no longer be degraded by failing connections because of an Internet outage at a VirtualMetric server's location, failing hardware, or because of downtime due to a software update for the operating system or VirtualMetric itself.

***

## **Install a VirtualMetric API**

All VirtualMetric components use VirtualMetric API to communicate with VirtualMetric DB. You can easily install two or more VirtualMetric API roles to form a high availability VirtualMetric API.

<div align="left">

<figure><img src="../.gitbook/assets/image (151).png" alt=""><figcaption></figcaption></figure>

</div>

Load balancing is a way to distribute workload across multiple web servers. The purpose is to attain optimal resource utilization, maximize request throughput, minimize response time, and avoid server overload.

Load balancers use various algorithms to accomplish this task. One of the simplest algorithms is round robin, which sends each new request to a different web server in an attempt to load all servers equally. Other algorithms send specific types of requests to specific servers in an attempt to reduce response time.

Create an entry for your VirtualMetric API roles on the load balancer. After that you can reach to load balancer entry instead of VirtualMetric API roles IP addresses.

{% hint style="info" %}
For information about setting up an entry on Load Balancer, please contact with your Load Balancer support.
{% endhint %}

Installing VirtualMetric is easy and works like other Windows-based applications. To install VirtualMetric, run the installation setup program that you have downloaded.

1\.      Confirm the question of the Windows User Account Control with **Yes** to allow the program to install. The VirtualMetric installation dialog will guide you through the installation process.

<div align="left">

<figure><img src="../.gitbook/assets/UACPrompt.png" alt=""><figcaption></figcaption></figure>

</div>

2\.      You will see Welcome Screen. Please click **Next** to continue.

<div align="left">

<figure><img src="../.gitbook/assets/APISetupWelcome.png" alt="" width="386"><figcaption></figcaption></figure>

</div>

3\.      **Accept** the license agreement and click **Next**.

<div align="left">

<figure><img src="../.gitbook/assets/APISetupLicense.png" alt="" width="386"><figcaption></figcaption></figure>

</div>

4\.      In this step, you will configure VirtualMetric API settings. After filling the **required fields**, click N**ext**.

<div align="left">

<figure><img src="../.gitbook/assets/APISetupAPI.png" alt="" width="386"><figcaption></figcaption></figure>

</div>

* You can use either **IP address or FQDN** for VirtualMetric API connectivity. All servers will use this address for inventory and performance stats collection. So if you use FQDN, FQDN address should be resolved by all servers.
* By default, VirtualMetric API listens TCP **8080**. You can change following port configuration on this step to use different port. After you specify port address, VirtualMetric will setup its REST API with this port configuration.
* Setup will add firewall rule into Windows Firewall as part of the installation.

{% hint style="warning" %}
VirtualMetric API address should be reachable by all servers. Please visit [Firewall Configuration](../introduction/product-security.md#required-firewall-ports) section to make sure.
{% endhint %}

{% hint style="info" %}
If you want to secure VirtualMetric API connections with an SSL certificate, please visit [Setup SSL Certificate](maintenance.md#setup-ssl-certificate) section.
{% endhint %}

5\.      In this step, you will configure VirtualMetric Database settings. After filling the required fields, click **Next**.

* &#x20;  You should enter your Microsoft SQL Server Instance information and User information in this step.
* &#x20;  Our setup supports Windows and SQL Authentication methods.

<div align="left">

<figure><img src="../.gitbook/assets/APISetupDatabase.png" alt="" width="386"><figcaption></figcaption></figure>

</div>

6\.      Review setup location and click **Next**.

<div align="left">

<figure><img src="../.gitbook/assets/APISetupLocation.png" alt="" width="386"><figcaption></figcaption></figure>

</div>

7\.      Click **Install** to start VirtualMetric installation.

<div align="left">

<figure><img src="../.gitbook/assets/APISetupInstall.png" alt="" width="386"><figcaption></figcaption></figure>

</div>

8\.      Click **Finish** to close Setup Wizard.

<div align="left">

<figure><img src="../.gitbook/assets/APISetupFinish.png" alt="" width="386"><figcaption></figcaption></figure>

</div>

***

## **Install a VirtualMetric Dashboard**

VirtualMetric Dashboard is the HTML based web interface to access VirtualMetric. You can easily install two or more VirtualMetric Dashboard roles to form a high availability VirtualMetric Dashboard.

<div align="left">

<figure><img src="../.gitbook/assets/image (152).png" alt=""><figcaption></figcaption></figure>

</div>

Load balancing is a way to distribute workload across multiple web servers. The purpose is to attain optimal resource utilization, maximize request throughput, minimize response time, and avoid server overload.

Load balancers use various algorithms to accomplish this task. One of the simplest algorithms is round robin, which sends each new request to a different web server in an attempt to load all servers equally. Other algorithms send specific types of requests to specific servers in an attempt to reduce response time.

Create an entry for your VirtualMetric Dashboard roles on the load balancer. After that you can reach to load balancer entry instead of VirtualMetric Dashboard roles IP addresses.

{% hint style="info" %}
For information about setting up an entry on Load Balancer, please contact with your Load Balancer support.
{% endhint %}

Installing VirtualMetric Dashboard is easy and works like other Windows-based applications. To install VirtualMetric Dashboard, run the installation setup program that you have downloaded.

1\.      Confirm the question of the Windows User Account Control with **Yes** to allow the program to install. The VirtualMetric Dashboard installation dialog will guide you through the installation process.

<div align="left">

<figure><img src="../.gitbook/assets/DashboardSetupUAC.png" alt=""><figcaption></figcaption></figure>

</div>

2\.      You will see Welcome Screen. Please click **Next** to continue.

<div align="left">

<figure><img src="../.gitbook/assets/DashboardSetupWelcome.png" alt="" width="386"><figcaption></figcaption></figure>

</div>

3\.      **Accept** the license agreement and click **Next**.

<div align="left">

<figure><img src="../.gitbook/assets/DashboardSetupLicense.png" alt="" width="386"><figcaption></figcaption></figure>

</div>

4\.      Enter VirtualMetric API address and click **Next** to continue.

<div align="left">

<figure><img src="../.gitbook/assets/DashboardSetupAPI.png" alt="" width="386"><figcaption></figcaption></figure>

</div>

{% hint style="info" %}
If you want to secure VirtualMetric Dashboard and VirtualMetric API connections with an SSL certificate, please visit [Setup SSL Certificate](maintenance.md#setup-ssl-certificate) section.
{% endhint %}

5\.      **Review** setup location and click **Next**.

<div align="left">

<figure><img src="../.gitbook/assets/DashboardSetupLocation.png" alt="" width="386"><figcaption></figcaption></figure>

</div>

6\.      Click **Install** to start VirtualMetric installation.

<div align="left">

<figure><img src="../.gitbook/assets/DashboardSetupInstall.png" alt="" width="386"><figcaption></figcaption></figure>

</div>

7\.      Click **Finish** to close Setup Wizard.

<div align="left">

<figure><img src="../.gitbook/assets/DashboardSetupFinish.png" alt="" width="386"><figcaption></figcaption></figure>

</div>

***

## **Install a VirtualMetric Database**

VirtualMetric Database uses Microsoft SQL Server for the database role. You can use SQL Server AlwaysOn to form a high availability VirtualMetric Database. AlwaysOn is a new integrated, flexible, cost-efficient high availability and disaster recovery solution for SQL Server. It can provide data and hardware redundancy within and across data centers, and improves application failover time to increase the availability of your mission-critical applications. AlwaysOn provides flexibility in configuration and enables reuse of existing hardware investments.

<div align="left">

<figure><img src="../.gitbook/assets/image (153).png" alt=""><figcaption></figcaption></figure>

</div>

If you want to install a SQL Server AlwaysOn cluster, please contact with Microsoft support. If you already have a SQL Server AlwaysOn cluster, you can migrate VirtualMetric Database on it.

{% hint style="info" %}
To migrate your current VirtualMetric Database to a SQL Server AlwaysOn instance, please visit [Migrate Database](maintenance.md#migrate-database) section.
{% endhint %}

***

## **Install a VirtualMetric Trigger**

VirtualMetric Trigger (aka VirtualMetric Collector) is the main component to connect servers, clusters and managers for monitoring and data collection. You can easily install two or more VirtualMetric Trigger roles to distribute servers, clusters and managers on different VirtualMetric Triggers. Also if you want to monitor servers in the isolated networks like NAT, NVGRE, Virtual Network etc, then installing a new VirtualMetric Trigger in this networks will help you for monitoring.

<div align="left">

<figure><img src="../.gitbook/assets/image (154).png" alt=""><figcaption></figcaption></figure>

</div>

Before installing VirtualMetric Trigger, you should create a new Trigger entry on VirtualMetric Settings Page.

1\.      Go to **Settings** and then **Click** to Devices, then you will see **Triggers** option.

<div align="left">

<figure><img src="../.gitbook/assets/image (155).png" alt=""><figcaption></figcaption></figure>

</div>

2\.      On Triggers screen, click **Add (+)** button on the right top section.

<figure><img src="../.gitbook/assets/image (156).png" alt=""><figcaption></figcaption></figure>

3\.      Enter a **Trigger name** and **description**, select **visibility** then click **Submit** button.

<div align="left">

<figure><img src="../.gitbook/assets/image (157).png" alt="" width="295"><figcaption></figcaption></figure>

</div>

4\.      Write down the **Trigger Identifier**. You will **need that when you install VirtualMetric Trigger**.

<figure><img src="../.gitbook/assets/image (158).png" alt=""><figcaption></figcaption></figure>

5\.      Click to **API** **Users** on the left pane.

<div align="left">

<figure><img src="../.gitbook/assets/image (160).png" alt=""><figcaption></figcaption></figure>

</div>

6\.      Write down your **API Username** and **API Token**. You will **need that when you install VirtualMetric Trigger**.

<figure><img src="../.gitbook/assets/image (161).png" alt=""><figcaption></figcaption></figure>

7\.      Installing VirtualMetric Trigger is easy and works like other Windows-based applications. To install VirtualMetric Trigger, run the installation setup program that you have downloaded.

8\.      Confirm the question of the Windows User Account Control with **Yes** to allow the program to install. The VirtualMetric Trigger installation dialog will guide you through the installation process.

<div align="left">

<figure><img src="../.gitbook/assets/TriggerSetupUAC (1).png" alt=""><figcaption></figcaption></figure>

</div>

9\.      You will see Welcome Screen. Please click **Next** to continue.

<div align="left">

<figure><img src="../.gitbook/assets/TriggerSetupWelcome.png" alt="" width="386"><figcaption></figcaption></figure>

</div>

10\.      Accept the license agreement and click **Next**.

<div align="left">

<figure><img src="../.gitbook/assets/TriggerSetupLicense.png" alt="" width="386"><figcaption></figcaption></figure>

</div>

11\.      In this step, you will configure VirtualMetric Trigger settings. Please click **Next** to continue

* &#x20;  VirtualMetric API Address
* &#x20;  Trigger Identifier
* &#x20;  API Username
* &#x20;  API Token

<div align="left">

<figure><img src="../.gitbook/assets/TriggerSetupTrigger.png" alt="" width="386"><figcaption></figcaption></figure>

</div>

{% hint style="info" %}
If you want to secure VirtualMetric Dashboard and VirtualMetric API connections with an SSL certificate, please visit [Setup SSL Certificate](maintenance.md#setup-ssl-certificate) section.
{% endhint %}

12\.      In this step, you can enable Active Directory authentication for VirtualMetric Trigger. Please click **Next** to continue.

* &#x20;  VirtualMetric uses scheduled task jobs for VirtualMetric Trigger. This user should also have administrator privileges on the local server. If you provide a domain user with necessary privileges on target servers, VirtualMetric will use this user to monitor servers. Please see [User Permissions](../modules-and-audit/virtualmetric-modules/bare-metal.md#windows-user-permissions) section for required privileges.
* &#x20;  If you want to use a domain user, please type its username as Domain\Username. User credentials will be used during setup to create VirtualMetric Trigger job and will not be stored anywhere.

<div align="left">

<figure><img src="../.gitbook/assets/TriggerUsernamePassword.png" alt="" width="385"><figcaption></figcaption></figure>

</div>

13\.      **Review** setup location and click **Next**.

<div align="left">

<figure><img src="../.gitbook/assets/TriggerSetupLocation.png" alt="" width="386"><figcaption></figcaption></figure>

</div>

14\.      Click **Install** to start VirtualMetric installation.

<div align="left">

<figure><img src="../.gitbook/assets/TriggerSetupInstall.png" alt="" width="386"><figcaption></figcaption></figure>

</div>

15\.      Click **Finish** to close Setup Wizard.

<div align="left">

<figure><img src="../.gitbook/assets/TriggerSetupFinish.png" alt="" width="386"><figcaption></figcaption></figure>

</div>
