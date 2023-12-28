# Add New Manager

Before adding a new Manager on VirtualMetric, please check that you have enough license and read _<mark style="color:red;">Server Pre-Configuration</mark>_ section for supported versions, software and hardware requirements.

Click to Managers on the left panel.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (377).png" alt=""><figcaption></figcaption></figure>

</div>

VirtualMetric Management Screen

<div align="left">

<figure><img src="../../../.gitbook/assets/image (378).png" alt=""><figcaption></figcaption></figure>

</div>

Select the **type** of the **Manager** then, click **Add (+)** button on the right top section.

<figure><img src="../../../.gitbook/assets/image (381).png" alt=""><figcaption></figcaption></figure>

<div align="left">

<figure><img src="../../../.gitbook/assets/image (380).png" alt="" width="297"><figcaption></figcaption></figure>

</div>

1\.      Enter name of **Manager**.

2\.      Select an appropriate **trigger** from the field Trigger.

3\.      Add **IP Address** of Manager.

4\.      Select a **Credential Type** from the drop down:&#x20;

&#x20;

**None** – Select this type and add Username and Password&#x20;

**Basic** – Selecting this option provides you with another Field called Credential from where you can select an appropriate option. &#x20;

**Cyberark** – Selecting this option provides you with another Field called Credential from where you can select an appropriate option.&#x20;

&#x20;

5\.      Select the checkbox Advance Settings. You get the fields as follows.

<table data-header-hidden><thead><tr><th width="254"></th><th></th></tr></thead><tbody><tr><td>Fields </td><td>Description </td></tr><tr><td>Manager Name </td><td>A label or name that is assigned to a manager. </td></tr><tr><td>Trigger</td><td>You may want to assign the servers to a custom Trigger if target server is in an Isolated network or if you want to setup a scalable infrastructure. You will only see available Triggers in this field.</td></tr><tr><td>FQDN / IP Address </td><td><p> <br>FQDN represents the complete domain name of a machine or application on a network.  For example: <a href="http://www.example.com/">www.example.com.</a> </p><p> </p><p>The numerical label assigned to each device connected to a computer network is called an "IP address." An IP address is typically represented in the format XXX.XXX.XXX.XX, where each "XXX" is a number ranging from 0 to 255, and the "XX" is a similar two-digit number. IP addresses are used to uniquely identify and locate devices on a network. </p></td></tr><tr><td>Port Number </td><td> A specific endpoint for data exchange between two devices or applications within a network. </td></tr><tr><td>Inventory Interval </td><td><p>This option defines frequency of Inventory Collector. Inventory Collector is responsible for: </p><p>·       Collecting server inventory like pending updates, installed applications, local administrators etc. </p><p>·       Collecting module inventory like virtual machines, web sites, databases etc. </p><p>·       Hardware Health Monitoring </p><p>·       Windows Firewall Logs </p><p>·       Change Tracking </p><p> </p></td></tr><tr><td>Stats Interval </td><td><p>This option defines frequency of Monitoring Collector. Monitoring Collector is responsible for: </p><p>·       Collecting all performance counters results </p><p>·       Collecting Event Logs </p><p>·       Collecting TCP Connections </p><p> </p></td></tr><tr><td>Logging Type </td><td>Logging Levels determine the frequency at which statistic queries occur, the length of time statistical data is stored in the database and the type of statistical data that is collected.</td></tr><tr><td>Debug </td><td><p>To choose debug such as:</p><p>·       <strong>Off</strong></p><p>·       <strong>Inventory:</strong> Only collects debug logs for Inventory Collector</p><p>·       <strong>Monitoring:</strong> Only collects debug logs for Monitoring Collector</p><p>·       <strong>On:</strong> Collects debug logs for Inventory and Monitoring Collector</p></td></tr><tr><td>Status </td><td><p>To choose a server status such as: </p><p>·       <strong>Active:</strong> Enables monitoring for server</p><p>·       <strong>Maintenance:</strong> Enables maintenance mode for server and disables all notifications</p><p>·      <strong>Reconnect:</strong> Restarts all collectors for server</p><p>·       <strong>Disabled:</strong> Disables monitoring for server</p></td></tr><tr><td>HP 3ParInfo</td><td><p>This is a hardware Integration component. You can set them as per the need.  Click the toggle button to get the field to add info. Type HP3ParInfo.exe path on server to activate HP 3Par Integration. </p><p>Example: <img src="../../../.gitbook/assets/image (382).png" alt=""></p></td></tr><tr><td>SuperMicro SuperDoctor 5</td><td><p>This is a hardware Integration component. You can set them as per the need.  Click the toggle button to get the field to add info. Type sdc.bat path on server to activate SuperMicro Integration. </p><p>Example:  <img src="../../../.gitbook/assets/image (383).png" alt=""></p></td></tr></tbody></table>
