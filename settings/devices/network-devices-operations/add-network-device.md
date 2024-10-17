# Add Network Device

Before adding a new network device on VirtualMetric, please check that you have enough license and read _<mark style="color:red;">Server Pre-Configuration</mark>_ section for supported versions, software and hardware requirements.

Click to **Network Device** on the left pane.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (416).png" alt=""><figcaption></figcaption></figure>

</div>

On Network Devices Management screen, click **Add (+)** button on the right top section.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (420).png" alt=""><figcaption></figcaption></figure>

</div>

<div align="left">

<figure><img src="../../../.gitbook/assets/image (421).png" alt="" width="295"><figcaption></figcaption></figure>

</div>

1\.      Select an appropriate **trigger** from the field **Trigger**.

2\.      Add **FQDN/IP Address**

3\.      Select a **Credential Type** from the drop down:&#x20;

**None** – Select this type and add Community String&#x20;

**SNMPv2** – Selecting this option provides you with another Field called Credential from where you can select an appropriate option. &#x20;

**SNMPv3** – Selecting this option provides you with another Field called Credential from where you can select an appropriate option.&#x20;

4\.      When **credential type** is **none**, select the check box **Enable SNMPv3**, select **Authentication Protocol and write Username.**

5\.      Select the checkbox **Advance Settings**. You get the fields as follows.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (422).png" alt="" width="291"><figcaption></figcaption></figure>

</div>

<table data-header-hidden><thead><tr><th width="244"></th><th></th></tr></thead><tbody><tr><td>Fields </td><td>Description </td></tr><tr><td>Network Device Name </td><td>A label or name that is assigned to a network device. </td></tr><tr><td>Trigger</td><td>You may want to assign the servers to a custom Trigger if target server is in an Isolated network or if you want to setup a scalable infrastructure. You will only see available Triggers in this field.</td></tr><tr><td>FQDN / IP Address </td><td><p> <br>FQDN represents the complete domain name of a machine or application on a network.  For example: <a href="http://www.example.com/">www.example.com.</a> </p><p> </p><p>The numerical label assigned to each device connected to a computer network is called an "IP address." An IP address is typically represented in the format XXX.XXX.XXX.XX, where each "XXX" is a number ranging from 0 to 255, and the "XX" is a similar two-digit number. IP addresses are used to uniquely identify and locate devices on a network. </p></td></tr><tr><td>Port Number </td><td> A specific endpoint for data exchange between two devices or applications within a network. </td></tr><tr><td>Inventory Interval </td><td><p>This option defines frequency of Inventory Collector. Inventory Collector is responsible for: </p><p>·       Collecting server inventory like pending updates, installed applications, local administrators etc. </p><p>·       Collecting module inventory like virtual machines, web sites, databases etc. </p><p>·       Hardware Health Monitoring </p><p>·       Windows Firewall Logs </p><p>·       Change Tracking </p><p> </p></td></tr><tr><td>Stats Interval </td><td><p>This option defines frequency of Monitoring Collector. Monitoring Collector is responsible for: </p><p>·       Collecting all performance counters results </p><p>·       Collecting Event Logs </p><p>·       Collecting TCP Connections </p><p> </p></td></tr><tr><td>Logging Type </td><td>Logging Levels determine the frequency at which statistic queries occur, the length of time statistical data is stored in the database and the type of statistical data that is collected.</td></tr><tr><td>Debug </td><td><p>To choose debug such as:</p><p>·       <strong>Off</strong></p><p>·       <strong>Inventory:</strong> Only collects debug logs for Inventory Collector</p><p>·     <strong>Monitoring:</strong> Only collects debug logs for Monitoring Collector</p><p>·       <strong>On:</strong> Collects debug logs for Inventory and Monitoring Collector</p></td></tr><tr><td>Status </td><td><p>To choose a server status such as: </p><p>·       <strong>Active:</strong> Enables monitoring for server</p><p>·       <strong>Maintenance:</strong> Enables maintenance mode for server and disables all notifications</p><p>·       <strong>Reconnect:</strong> Restarts all collectors for server</p><p>·       <strong>Disabled:</strong> Disables monitoring for server</p></td></tr><tr><td><p> Connection String</p><p> </p></td><td><p>This field only appears when <strong>configuration backup enabled</strong>.</p><p>You can write connection string to this field.</p><p><img src="../../../.gitbook/assets/image (423).png" alt="" data-size="original"></p></td></tr></tbody></table>

{% hint style="info" %}
When configuration backup is enabled, connection string can be written by following below example and explanations.&#x20;

**Example:** {"Model":"cisco-ios","Protocol":"ssh","UserName":"cisco","Password":"cisco","IPAddress":"192.168.1.111","EnablePassword":"cisco","EnableMode":true,"KeepBackupFiles":false,"BackupCount":2}



**Model:** Model Of the Network Device. Ex:cisco-ios,mikrotik,fortios,junos&#x20;

**Protocol:** Which protocol to use for backup. SSH-Telnet&#x20;

**Username:** Username&#x20;

**Password:** Password&#x20;

**IPAddress:** IP Info of the device&#x20;

**EnableMode:** If the Device have enable exec mode active&#x20;

**EnablePassword:** If the enablemode is active enable password&#x20;

**KeepBackupFiles:** If you want to keep the backup file under trigger backup folder

**BackupCount:** How many backup files to keep in backup folder
{% endhint %}

6\.      After entering all the required info, **click** the button **SUBMIT**. The Network Device will be added now.
