# Maintenance

In this section, you will find some maintenance options for VirtualMetric. If you need further support, please contact with VirtualMetric support.

***

## **Repair Files**

If you are using latest version of VirtualMetric and you need to repair VirtualMetric Standalone Server, then you can use following package to repair your installation.

**VirtualMetric Standalone Server - Full Update - NoSQL (Latest Version)**

[ VirtualMetric-Update-Full-NoSQL.exe](http://www.virtualmetric.com/files/VirtualMetric-Update-Full-NoSQL.exe)

To repair VirtualMetric files, you can use Update packages of corresponding versions.

{% hint style="info" %}
Please read [Running Update Application](update-from-previous-versions.md#running-update-application) to learn how to repair your installation.
{% endhint %}

***

## **Repair Database**

If your VirtualMetric installation is not able to access VirtualMetric Database due to a failed update process or other reasons, please be aware of that working on VirtualMetric Database is not supported.

Please try reinstalling update package that you are trying to apply. If the problem still persists, please contact with VirtualMetric support. We recommend that you always have a proper backup of your VirtualMetric Database before update.

{% hint style="info" %}
Please read [Backup Database](maintenance.md#backup-database) to learn how to backup your VirtualMetric Database.
{% endhint %}

***

## **Backup Database**

To backup your VirtualMetric Database, first you should connect to your current Microsoft SQL Server instance via [ SQL Server Management Studio](https://en.wikipedia.org/wiki/SQL\_Server\_Management\_Studio).

1\.      Right click on **VIRTUALMETRICDB** and select **Tasks -> Back Up...** from menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (147).png" alt=""><figcaption></figcaption></figure>

</div>

2\.      Please make sure that backup type is **Full** and backup location for disk is exist. Then click **OK** to start backup.

<div align="left">

<figure><img src="../.gitbook/assets/image (148).png" alt="" width="362"><figcaption></figcaption></figure>

</div>

<div align="left">

<figure><img src="../.gitbook/assets/image (149).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

3\.      When backup is completed successfully, please click **OK** to close notification dialog.

<div align="left">

<figure><img src="../.gitbook/assets/image (150).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

4\.      Please verify that Backup file is exist under your backup path. You can **save** this **.bak** file for **Restore** purposes.

<div align="left">

<figure><img src="../.gitbook/assets/image (151).png" alt=""><figcaption></figcaption></figure>

</div>

## Restore Database

To restore your VirtualMetric Database, first you should connect to your current Microsoft SQL Server instance via [ SQL Server Management Studio](https://en.wikipedia.org/wiki/SQL\_Server\_Management\_Studio).

<div align="left">

<figure><img src="../.gitbook/assets/image (152).png" alt=""><figcaption></figcaption></figure>

</div>

1\.      **Right click** on **VIRTUALMETRICDB** and select **Tasks -> Take Offline** from menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (153).png" alt="" width="360"><figcaption></figcaption></figure>

</div>

2\.      Please make sure that you choose Drop All Active Connections and then click **OK** to make database offline.

<div align="left">

<figure><img src="../.gitbook/assets/image (154).png" alt="" width="346"><figcaption></figcaption></figure>

</div>

3\.      You will see that database is in **Offline** mode. Now you can start restoring VirtualMetric Database from previous backup.

<div align="left">

<figure><img src="../.gitbook/assets/image (155).png" alt=""><figcaption></figcaption></figure>

</div>

4\.      Right click on **VIRTUALMETRICDB** and select **Tasks -> Restore -> Database...** from menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (156).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

5\.      Please verify that Backup file is exist under your backup path. Click **OK** to restore database.

<div align="left">

<figure><img src="../.gitbook/assets/image (157).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

6\.      Click **OK** to close restore dialog.

<div align="left">

<figure><img src="../.gitbook/assets/image (158).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

7\.      After this operation, your VirtualMetric Database will be restored and online for operations.

<div align="left">

<figure><img src="../.gitbook/assets/image (159).png" alt=""><figcaption></figcaption></figure>

</div>

***

## Migrate Database

To migrate your VirtualMetric Database to another server, first you should have proper backup of VirtualMetric Database.

{% hint style="info" %}
Please read [Backup Database](maintenance.md#backup-database) to learn how to backup your VirtualMetric Database.
{% endhint %}

1\.      To start migration, first you should connect to your current Microsoft SQL Server instance via [ SQL Server Management Studio](https://en.wikipedia.org/wiki/SQL\_Server\_Management\_Studio).

<div align="left">

<figure><img src="../.gitbook/assets/image (160).png" alt=""><figcaption></figcaption></figure>

</div>

2\.      **Right click** on Databases and select **Restore Database..**. from menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (161).png" alt=""><figcaption></figcaption></figure>

</div>

3\.      On **Restore Database** window, select **Device** as source, click to **...** button on the right side for backup location window. Then click **Add** to locate Backup file.

<div align="left">

<figure><img src="../.gitbook/assets/image (162).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

4\.      Locate the backup file with **.bak** extension, then click **OK** to close dialog.

<div align="left">

<figure><img src="../.gitbook/assets/image (163).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

5\.      Click **OK** to close Select backup devices window.

<div align="left">

<figure><img src="../.gitbook/assets/image (164).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

6\.      Click **OK** to start restoring VirtualMetric Database.

<div align="left">

<figure><img src="../.gitbook/assets/image (165).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

7\.      Click **OK** to close restoration dialog.

<div align="left">

<figure><img src="../.gitbook/assets/image (166).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

8\.      After this operation, your VirtualMetric Database will be **restored** and online for operations.

<div align="left">

<figure><img src="../.gitbook/assets/image (127).png" alt=""><figcaption></figcaption></figure>

</div>

9\.      When you **change** VirtualMetric Database settings, you **should also modify** following files:

```markup
C:\Program Files\VirtualMetric\API\Web.config
C:\Program Files\VirtualMetric\HealthCheck\VirtualMetricHealthCheck.exe.config
C:\Program Files\VirtualMetric\SQLJobs\VirtualMetricSQLJobs.exe.config
```

On these files, search for following entry:

```markup
initial catalog=VIRTUALMETRICDB;
```

When you find this line, you will see SQL Database settings like:

```javascript
data source={IPAddress}; // IP Address of VirtualMetric Database Instance
user id=sa; // SQL Username
password={SA Password}; // SQL User Password
```

\
10\.      After changing config files, you should only **restart** VirtualMetric SQL Jobs scheduled task. Please open **Task Scheduler** on VirtualMetric Standalone Server.

<div align="left">

<figure><img src="../.gitbook/assets/image (128).png" alt="" width="196"><figcaption></figcaption></figure>

</div>

11\.      Right click on **VirtualMetric SQL Jobs** and click **End** from menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (129).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

12\.      Click **Yes** to confirm dialog.

<div align="left">

<figure><img src="../.gitbook/assets/image (130).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

13\.      Wait for a few seconds. Then right click on VirtualMetric SQL Jobs and click **Run** from menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (131).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

14\.      Now, you can continue using VirtualMetric after these operations.

***

## Change Database User

You may need to change SQL user or SQL user password for several reasons. To change SQL user password, first you should connect to your current Microsoft SQL Server instance via [ SQL Server Management Studio](https://en.wikipedia.org/wiki/SQL\_Server\_Management\_Studio).

<div align="left">

<figure><img src="../.gitbook/assets/image (809).png" alt=""><figcaption></figcaption></figure>

</div>

1\.      Navigate to **current SQL user** via **Security -> Logins** on left menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (810).png" alt=""><figcaption></figcaption></figure>

</div>

2\.      **Right click** to SQL User and then **click Properties** on menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (811).png" alt=""><figcaption></figcaption></figure>

</div>

3\.      Type new **password** and click **OK** to apply changes.

<div align="left">

<figure><img src="../.gitbook/assets/image (812).png" alt="" width="345"><figcaption></figcaption></figure>

</div>

4\.      When you change VirtualMetric Database settings, you should also modify following files:

```markup
C:\Program Files\VirtualMetric\API\Web.config
C:\Program Files\VirtualMetric\HealthCheck\VirtualMetricHealthCheck.exe.config
C:\Program Files\VirtualMetric\SQLJobs\VirtualMetricSQLJobs.exe.config
```

On these files, search for following entry:

```csharp
initial catalog=VIRTUALMETRICDB;
```

When you find this line, you will see SQL Database settings like:

```csharp
data source={IPAddress}; // IP Address of VirtualMetric Database Instance
user id=sa; // SQL Username
password={SA Password}; // SQL User Password
```

5\.      After changing config files, you should only **restart** VirtualMetric SQL Jobs scheduled task. Please open **Task Scheduler** on VirtualMetric Standalone Server.

<div align="left">

<figure><img src="../.gitbook/assets/image (813).png" alt="" width="196"><figcaption></figcaption></figure>

</div>

6\.      **Right click** on VirtualMetric SQL Jobs and click **End** from menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (814).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

7\.      Click **Yes** to confirm dialog.

<div align="left">

<figure><img src="../.gitbook/assets/image (815).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

8\.      Wait for a few seconds. Then **right click** on VirtualMetric SQL Jobs and click **Run** from menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (816).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

9\.      Now, you can continue using VirtualMetric after these operations.

***

## Change Trigger Configuration

If you need to change following options of the VirtualMetric Trigger:

* &#x20;  VirtualMetric API Address
* &#x20;  Trigger Identifier
* &#x20;  API Username
* &#x20;  API Token

1\.      You should **modify** the **VirtualMetric Trigger config file**:

```markup
C:\Program Files\VirtualMetric\Trigger\VirtualMetricTrigger.exe.config
```

On the config file, you will see following lines:

```csharp
<appSettings>
    <add key="primaryApiUrl" value="https://api.virtualmetric.com:8080/API/" />
    <add key="failoverApiUrl" value="" />
    <add key="triggerId" value="3080487f-f3f6-43e2-bd27-7f1886a12816" />
    <add key="apiUser" value="vmapi" />
    <add key="apiPassword" value="727c9b3a51eb3407c7cc21c45d84bb28" />
</appSettings>
```

2\.      After changing these Trigger options, you should **restart** VirtualMetric **Trigger** scheduled task. Please open **Task Scheduler** on VirtualMetric Standalone Server.

<div align="left">

<figure><img src="../.gitbook/assets/image (817).png" alt="" width="196"><figcaption></figcaption></figure>

</div>

3\.      Right click on **VirtualMetric SQL Jobs** and click **End** from menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (814).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

4\.      Click **Yes** to confirm dialog.

<div align="left">

<figure><img src="../.gitbook/assets/image (815).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

5\.      Wait for a few seconds. Then **right click** on VirtualMetric SQL Jobs and click **Run** from menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (816).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

6\.      VirtualMetric Trigger will connect to VirtualMetric API and start monitoring in a few seconds.

{% hint style="info" %}
Please read [Install a VirtualMetric Trigger](high-availability-components.md#install-a-virtualmetric-trigger) to learn more about Trigger Options.
{% endhint %}

***

## Reset Admin Password

If you **forget** the admin **username/password** of VirtualMetric Dashboard, you have following options:

* Password recovery request on VirtualMetric Dashboard
* Changing directly from VirtualMetric Database

{% hint style="info" %}
Please read [Password Recovery Request](../virtual-metric-dashboard/login.md#password-recovery-request) to learn how to reset your password via VirtualMetric Dashboard.
{% endhint %}

1\.      To change admin password from VirtualMetric Database, first you should connect to your current Microsoft SQL Server instance via [ SQL Server Management Studio](https://en.wikipedia.org/wiki/SQL\_Server\_Management\_Studio).

<div align="left">

<figure><img src="../.gitbook/assets/image (818).png" alt=""><figcaption></figcaption></figure>

</div>

2\.      Navigate to **dbo.SystemUser** table via **VIRTUALMETRICDB -> Tables** on left menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (819).png" alt="" width="220"><figcaption></figcaption></figure>

</div>

3\.      **Right click** on **dbo.SystemUser** and **click Edit Top 200 Rows** on menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (820).png" alt="" width="220"><figcaption></figcaption></figure>

</div>

4\.      **Find the user** that you want to **change password** and navigate to **Password field**.

<figure><img src="../.gitbook/assets/image (821).png" alt=""><figcaption></figcaption></figure>

5\.      VirtualMetric uses MD5 hashes instead of real passwords. You can convert your password with online conversion websites or you can simply use PowerShell to convert your password to MD5 hash.

{% code overflow="wrap" lineNumbers="true" fullWidth="false" %}
```powershell
$userPassword = "Password1!"
$MD5 = New-Object -TypeName System.Security.Cryptography.MD5CryptoServiceProvider
$UTF8 = New-Object -TypeName System.Text.UTF8Encoding
[System.BitConverter]::ToString($MD5.ComputeHash($UTF8.GetBytes($userPassword))).Replace("-","")
```
{% endcode %}

6\.      You can **replace** new MD5 hash with old one on VirtualMetric Database.

{% hint style="warning" %}
You must restart application pool of VirtualMetric API via IIS Manager to apply password reset.
{% endhint %}

7\.      Please open **IIS Manager** on VirtualMetric Standalone Server.

<div align="left">

<figure><img src="../.gitbook/assets/image (822).png" alt="" width="196"><figcaption></figcaption></figure>

</div>

8\.      Click to **Application Pools** on left menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (823).png" alt=""><figcaption></figcaption></figure>

</div>

9\.      Right click on **VirtualMetric API** and then **click** **Recycle**... to restart the application pool.

<div align="left">

<figure><img src="../.gitbook/assets/image (824).png" alt="" width="269"><figcaption></figcaption></figure>

</div>

10\.      After application pool restart, you can login via VirtualMetric Dashboard.

***

## Setup SSL Certificate

To make VirtualMetric Dashboard and VirtualMetric API connections secure, you can use SSL certificate. You can use IIS Manager to apply SSL certificates for both websites.

1\.      Please open **IIS Manager** on VirtualMetric Standalone Server.

<div align="left">

<figure><img src="../.gitbook/assets/image (825).png" alt="" width="196"><figcaption></figcaption></figure>

</div>

2\.      Click to **Server Certificates** to create certificate request.

<div align="left">

<figure><img src="../.gitbook/assets/image (826).png" alt=""><figcaption></figcaption></figure>

</div>

3\.      **Click** **Create Certificate Request** on right menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (827).png" alt=""><figcaption></figcaption></figure>

</div>

4\.      **Fill** your **Certificate Request** and click **Next** to continue.

<div align="left">

<figure><img src="../.gitbook/assets/image (828).png" alt="" width="345"><figcaption></figcaption></figure>

</div>

5\.     **Set crypto settings** and click **Next** to continue.

<div align="left">

<figure><img src="../.gitbook/assets/image (829).png" alt="" width="345"><figcaption></figcaption></figure>

</div>

6\.      **Set** a **path** for request and **click Finish** to complete cert request.

<div align="left">

<figure><img src="../.gitbook/assets/image (830).png" alt="" width="345"><figcaption></figcaption></figure>

</div>

7\.      Use your cert request to purchase a commercial SSL. After you get your .cer file, **click Complete Certificate Request...** to continue.

<div align="left">

<figure><img src="../.gitbook/assets/image (831).png" alt=""><figcaption></figcaption></figure>

</div>

8\.      Specify .cer file, fill inputs and **click OK** to complete certificate process.

<div align="left">

<figure><img src="../.gitbook/assets/image (832).png" alt="" width="345"><figcaption></figcaption></figure>

</div>

9\.     **Click** to **VirtualMetric API** on left menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (833).png" alt=""><figcaption></figcaption></figure>

</div>

10\.      **Click** to **Bindings**... on right menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (834).png" alt=""><figcaption></figcaption></figure>

</div>

11\.      **Click** to **Add...** on right menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (835).png" alt=""><figcaption></figcaption></figure>

</div>

12\.      Fill **Bindings** inputs and click **OK** to complete.

<div align="left">

<figure><img src="../.gitbook/assets/image (836).png" alt="" width="495"><figcaption></figcaption></figure>

</div>

13\.      Click to **Close** to close dialog.

<div align="left">

<figure><img src="../.gitbook/assets/image (837).png" alt="" width="495"><figcaption></figcaption></figure>

</div>

14\.      When you change **VirtualMetric API SSL** settings, you should also **modify** following files:

```markup
C:\Program Files\VirtualMetric\HealthCheck\VirtualMetricHealthCheck.exe.config
C:\Program Files\VirtualMetric\Observer\VirtualMetricObserver.exe.config
C:\Program Files\VirtualMetric\Trigger\VirtualMetricTrigger.exe.config
C:\Program Files\VirtualMetric\ControlPanel\Web.config
```

On these files, you should change VirtualMetric API address lines with new address:

```csharp
<appSettings>
    <add key="primaryApiUrl" value="https://api.virtualmetric.com/API/" />
    <add key="failoverApiUrl" value="" />
    <add key="triggerId" value="3080487f-f3f6-43e2-bd27-7f1886a12816" />
    <add key="apiUser" value="vmapi" />
    <add key="apiPassword" value="727c9b3a51eb3407c7cc21c45d84bb28" />
</appSettings>
```

\
15\.      After changing config files, you should only **restart VirtualMetric Trigger** scheduled task.\
Please open **Task Scheduler** on VirtualMetric Standalone Server.

<div align="left">

<figure><img src="../.gitbook/assets/image (838).png" alt="" width="196"><figcaption></figcaption></figure>

</div>

16\.      **Right click** on **VirtualMetric Trigger** and click **End** from menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (839).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

17\.      Click **Yes** to confirm dialog.

<div align="left">

<figure><img src="../.gitbook/assets/image (840).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

18\.      Wait for a few seconds. Then **right click on VirtualMetric Trigger** and click **Run** from menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (841).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

19\.      VirtualMetric Trigger will connect to VirtualMetric API and start monitoring in a few seconds.

***

## **Change API Configuration**

If you want to change VirtualMetric API configuration, you should modify following file:

```markup
C:\Program Files\VirtualMetric\API\Web.config
```

On the .config file, you can change connection strings to use a different VirtualMetric Database instance.

{% hint style="info" %}
Please read [Install a VirtualMetric API](high-availability-components.md#install-a-virtualmetric-api) to learn more about API Options.
{% endhint %}

***

## **Dashboard NAT Configuration**

If you use private network for VirtualMetric Standalone Server and if you want to publish your VirtualMetric Dashboard to external networks via Firewall or Load Balancer, then you may have some issues.

<div align="left">

<figure><img src="../.gitbook/assets/image (842).png" alt=""><figcaption></figcaption></figure>

</div>

Because as you can see from diagram above, both VirtualMetric Dashboard and Client Devices try to connect VirtualMetric API.\
VirtualMetric Dashboard configuration file includes following lines:

```csharp
<appSettings>
    <add key="webpages:Version" value="3.0.0.0" />
    <add key="webpages:Enabled" value="false" />
    <add key="ClientValidationEnabled" value="true" />
    <add key="UnobtrusiveJavaScriptEnabled" value="true" />
    <add key="apiUrl" value="https://external.virtualmetric.com:8080/API/" />
    <add key="debugMode" value="false" />
</appSettings>
```

When you set external address for VirtualMetric API, Client Devices must be able to query VirtualMetric API. Otherwise you will see following error on VirtualMetric Dashboard login and that will prevent you to login:

<div align="left">

<figure><img src="../.gitbook/assets/image (843).png" alt=""><figcaption></figcaption></figure>

</div>

If Client Devices are able to reach to VirtualMetric API, then you must also be sure that VirtualMetric Dashboard can also reach to external address. Otherwise you will see following error when you try to connect:

<div align="left">

<figure><img src="../.gitbook/assets/image (844).png" alt=""><figcaption></figcaption></figure>

</div>

If external address is not resolved by VirtualMetric Server's DNS, then you should modify local Hosts file to make it reachable.

***

## **Change Dashboard Timeout**

Default session timeout for VirtualMetric Dashboard is 20 minutes. This is the default value of IIS application pool. If you want to increase session timeout, you can use IIS Manager to modify timeout.

1\.      Please **open IIS Manager** on VirtualMetric Standalone Server.

<div align="left">

<figure><img src="../.gitbook/assets/image (845).png" alt="" width="196"><figcaption></figcaption></figure>

</div>

2\.      **Click** to **Application Pools** on the left menu. You will see Application Pools for **VirtualMetric Dashboard** and **VirtualMetric API**.

<div align="left">

<figure><img src="../.gitbook/assets/image (846).png" alt=""><figcaption></figcaption></figure>

</div>

3\.      **Right click** on **VirtualMetric ControlPanel** and select Advanced Settings to open timeout settings.

<div align="left">

<figure><img src="../.gitbook/assets/image (847).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

4\.      Set **0** for **Idle Time-out (minutes)** to disable timeout or select another timeout value. You can also set timeout value for VirtualMetric API with same steps.

<div align="left">

<figure><img src="../.gitbook/assets/image (848).png" alt=""><figcaption></figcaption></figure>

</div>

***

## **Configure Redis Distributed Cache**

If you want to use VirtualMetric API in HA mode, you should also configure VirtualMetric APIs to use Redis Distributed Cache. You need to set your Redis connection string into VirtualMetric API web.config.\
\
1\.      Add your **Redis connection string** into **VirtualMetric API** configuration file as following:

{% code overflow="wrap" lineNumbers="true" %}
```csharp
  <connectionStrings>
    <add name="VirtualMetricRedis" connectionString="{IPAddress},password={password},abortConnect=false" />
  </connectionStrings>
```
{% endcode %}

2\.      After that, you should **activate** Redis Caching via **VirtualMetric Advanced System Settings**.\
For security reasons Redis Default Listening interface is bind to "127.0.0.1".\
\
To enable Redis on Server IP address, you need to edit the following line in your Redis Configuration files:

```csharp
bind {IPAddress}
```

{% hint style="info" %}
Redis is not optimized for maximum security but for maximum performance and simplicity. For this reason you should not expose the Redis instance directly to the internet and restrict access to Redis port from untrusted network with ACLs.
{% endhint %}

3\.      We also recommend you to **enable Redis password** in your configuration files:

```csharp
requirepass {password}
```

4\.      If you want to use Redis Master/Slave option you need to enable the following lines on your Redis Servers Configuration files:

```csharp
Redis Master Server:
requirepass {password}

Redis Slave Server:
slaveof {MasterServerIPAddress} 6379
masterauth {password}
```

5\.      After changes, you should activate Redis from System Advanced Configuration. Find the "**Cache Provider"** option in the **System Advanced Settings**.

<div align="left">

<figure><img src="../.gitbook/assets/image (108).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

6\.      Change **"Cache Provider"** option as **Redis** and click **Submit** button.

<div align="left">

<figure><img src="../.gitbook/assets/image (109).png" alt="" width="309"><figcaption></figcaption></figure>

</div>

{% hint style="warning" %}
You must restart application pool of VirtualMetric API via IIS Manager to apply cache provider changes.
{% endhint %}

7\.      Please **open** **IIS Manager** on VirtualMetric Standalone Server.

<div align="left">

<figure><img src="../.gitbook/assets/image (110).png" alt="" width="196"><figcaption></figcaption></figure>

</div>

8\.      **Click** to **Application Pools** on left menu.

<div align="left">

<figure><img src="../.gitbook/assets/image (111).png" alt=""><figcaption></figcaption></figure>

</div>

9\.      **Right click** on **VirtualMetric API** and then **click Recycle**... to restart the application pool.

<div align="left">

<figure><img src="../.gitbook/assets/image (112).png" alt="" width="269"><figcaption></figcaption></figure>

</div>

10\.      After application pool restart, Redis will be activated on VirtualMetric.

***

## **Database Design Best Practices**

We recommend you to configure following Microsoft SQL Server optimizations to get the best performance.

1\.      **Click Properties** of the server in the SQL Server Management Studio.

<div align="left">

<figure><img src="../.gitbook/assets/image (113).png" alt="" width="372"><figcaption></figcaption></figure>

</div>

2\.      Click on **Advanced tab** and set following options:

* &#x20;  Miscellaneous > Optimize for Ad hoc Workloads: True
* &#x20;  Parallelism > Cost Threshold for Parallelism: 50
* &#x20;  Parallelism > Max degrees of Parallelism: 12

<div align="left">

<figure><img src="../.gitbook/assets/image (114).png" alt="" width="352"><figcaption></figcaption></figure>

</div>

3\.      Click on **Memory tab** and set following options.

* &#x20;  Minimum server in memory (in MB): 0
* &#x20;  Maximum server in memory (in MB): 4096 (Calculate this based on your server memory)

<div align="left">

<figure><img src="../.gitbook/assets/image (115).png" alt="" width="352"><figcaption></figcaption></figure>

</div>

4\.      Click on **Processor tab** and set following options.

* &#x20;  Maximum worker threads: 0

<div align="left">

<figure><img src="../.gitbook/assets/image (116).png" alt="" width="352"><figcaption></figcaption></figure>

</div>

5\.      After the changes, please restart SQL Service to apply changes.
