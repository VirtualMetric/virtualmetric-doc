# Add New Workstation

Before adding a new Workstation on VirtualMetric, please check that you have enough license and read _<mark style="color:red;">**Server Pre-Configuration**</mark>_ section for supported versions, software and hardware requirements.

Click to Workstation on the left pane.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (499).png" alt="" width="128"><figcaption></figcaption></figure>

</div>

On Workstation Management screen, click **Add (+)** button on the right top section.

<figure><img src="../../../.gitbook/assets/image (500).png" alt=""><figcaption></figcaption></figure>

Select **Workstation Type** and enter **FQDN / IP Address** of Workstation, then click **Submit** button.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (501).png" alt="" width="290"><figcaption></figcaption></figure>

</div>

## Add a Windows Workstation

1\.      To add a **new** Workstation, go to **Devices > Workstation** and then click the + button located in the upper right corner.&#x20;

<div align="left">

<figure><img src="../../../.gitbook/assets/image (502).png" alt="" width="290"><figcaption></figcaption></figure>

</div>

2\.      Select the Workstation Type as **Windows**.&#x20;

3\.      Select a **Trigger** as per your need.&#x20;

4\.      Enter the **FQDN/IP Address**. Note: The FQDN is a complete and unambiguous domain name that specifies the exact location of the workstation within the Domain Name System (DNS) hierarchy. It typically includes the hostname of the workstation and the domain name it belongs to. For example, "workstation.example.com&#x20;

5\.      Select the checkbox Active Directory Authentication if you wish to use delegation of VirtualMetric service user credentials if target server is in the same Active Directory. &#x20;

6\.      If you unselect the checkbox, you will get 2 more additional fields: Username and Password. &#x20;

7\.      Add the Username and Password for your Windows Workstation.&#x20;

8\.      Select the checkbox Advance Settings. You get the fields as follows.

#### &#x20;Advance Settings: Refer to the following table to understand the fields in the above screen.&#x20;

<table><thead><tr><th width="219">Fields </th><th>Description</th></tr></thead><tbody><tr><td>Hostname </td><td>A label or name that is assigned to a workstation. </td></tr><tr><td>Server Type </td><td>Workstation types such as Windows, Linux </td></tr><tr><td>Trigger</td><td>You may want to assign the servers to a custom Trigger if target server is in an Isolated network or if you want to setup a scalable infrastructure. You will only see available Triggers in this field.</td></tr><tr><td>FQDN / IP Address </td><td><p> <br>FQDN represents the complete domain name of a machine or application on a network.  For example: <a href="http://www.example.com/">www.example.com.</a> </p><p> </p><p>The numerical label assigned to each device connected to a computer network is called an "IP address." An IP address is typically represented in the format XXX.XXX.XXX.XX, where each "XXX" is a number ranging from 0 to 255, and the "XX" is a similar two-digit number. IP addresses are used to uniquely identify and locate devices on a network. </p></td></tr><tr><td>Port Number </td><td> A specific endpoint for data exchange between two devices or applications within a network. </td></tr><tr><td>Inventory Interval </td><td><p>This option defines frequency of Inventory Collector. Inventory Collector is responsible for: </p><p>·       Collecting server inventory like pending updates, installed applications, local administrators etc. </p><p>·       Collecting module inventory like virtual machines, web sites, databases etc. </p><p>·       Hardware Health Monitoring </p><p>·       Windows Firewall Logs </p><p>·       Change Tracking </p><p> </p></td></tr><tr><td>Stats Interval </td><td><p>This option defines frequency of Monitoring Collector. Monitoring Collector is responsible for: </p><p>·       Collecting all performance counters results </p><p>·       Collecting Event Logs </p><p>·       Collecting TCP Connections </p><p> </p></td></tr><tr><td>Logging Type </td><td>Logging Levels determine the frequency at which statistic queries occur, the length of time statistical data is stored in the database and the type of statistical data that is collected.</td></tr><tr><td>Debug </td><td><p>To choose debug such as:</p><p>·       <strong>Off</strong></p><p>·      <strong>Inventory:</strong> Only collects debug logs for Inventory Collector</p><p>·       <strong>Monitoring:</strong> Only collects debug logs for Monitoring Collector</p><p>·       <strong>On:</strong> Collects debug logs for Inventory and Monitoring Collector</p></td></tr><tr><td>Status </td><td><p>To choose a server status such as: </p><p>·       <strong>Active:</strong> Enables monitoring for server</p><p>·       <strong>Maintenance:</strong> Enables maintenance mode for server and disables all notifications</p><p>·       <strong>Reconnect:</strong> Restarts all collectors for server</p><p>·       <strong>Disabled:</strong> Disables monitoring for server</p></td></tr><tr><td>Temporary Path </td><td>This option appears only for Linux and VMWare servers.  </td></tr></tbody></table>

## Add a Linux Workstation

1\.      To add a Linux workstation, go to **Workstation Operations > Add Workstation** > then click the **+** button on the right corner, you get the Add New Workstation screen, where you need to select the Workstation Type as **Linux**.&#x20;

2\.      Select **Linux** from the **Workstation Type** field.&#x20;

<div align="left">

<figure><img src="../../../.gitbook/assets/image (505).png" alt="" width="291"><figcaption></figcaption></figure>

</div>

3\.      Select the appropriate trigger from the field Trigger. &#x20;

4\.      Add **FQDN / IP Address**.&#x20;

5\.      Select the checkbox **key-Based Authentication** to enable SSH key-based authentication.&#x20;

6\.      Enter your **SSH private key**.&#x20;

<div align="left">

<figure><img src="../../../.gitbook/assets/image (506).png" alt="" width="281"><figcaption></figcaption></figure>

</div>

7\.      If your private key requires a passphrase, select the checkbox Enable Passphrase. This would bring up a field to enter the passphrase.

8\.      Enter the passphrase and click **Submit** to apply changes and add your Linux server.&#x20;

9\.      If you want to add more advanced setting to your Linux server, select the checkbox Advanced Settings. You get the additional fields: Refer to the section [Advance Settings](add-new-workstation.md#advance-settings-refer-to-the-following-table-to-understand-the-fields-in-the-above-screen.)&#x20;

10\.    After entering all the required info, click the button **SUBMIT**. The Windows server will be added now.
