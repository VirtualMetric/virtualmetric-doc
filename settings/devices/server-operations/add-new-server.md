# Add New Server

![](<../../../.gitbook/assets/image (543).png>)

Select Server Type and enter FQDN/IP Address of the server, then click Submit button.

<figure><img src="../../../.gitbook/assets/image (544).png" alt=""><figcaption></figcaption></figure>

## Server Type

You can choose target Servers Type at this field. If you choose a wrong Server Type for target servers, VirtualMetric will not be able to make connection to the server. VirtualMetric supports Windows, VMware, and Linux server types.

### **Add a Windows Server**

1.  Go to Server **Operations > Add Server** > then click the + button located in the upper right corner.

    <figure><img src="../../../.gitbook/assets/image (545).png" alt=""><figcaption></figcaption></figure>
2.  Select **Windows** from the **Server Type** field.

    <div align="left">

    <figure><img src="../../../.gitbook/assets/image (546).png" alt="" width="563"><figcaption></figcaption></figure>

    </div>
3.  Select an appropriate trigger from the field **Trigger**. &#x20;

    **Note:** Trigger option is only available in Advanced Mode. You may want to assign the servers to a custom Trigger if target server is in an Isolated network or if you want to setup a scalable infrastructure. You will only see available Triggers in this field.
4. Add **FQDN/IP Address**
5. Select the checkbox **Active Directory Authentication** to use delegation of VirtualMetric service user credentials if target server is in same Active Directory.
6. Select the checkbox [**Advanced Settings**](add-new-server.md#advance-settings-refer-to-the-following-table-to-understand-the-fields-in-the-above-screen.). You get the additional fields as follows:

<div align="left">

<figure><img src="../../../.gitbook/assets/image (547).png" alt="" width="294"><figcaption></figcaption></figure>

</div>

#### Advance Settings: Refer to the following table to understand the fields in the above screen.  <a href="#advance-settings" id="advance-settings"></a>

<table><thead><tr><th width="258">Fields</th><th>Descriptrion</th></tr></thead><tbody><tr><td>Hostname </td><td>A  label or name that is assigned to a device on a computer network. </td></tr><tr><td>Server Type </td><td>Server types such as Windows, Linux, VMWare, etc. </td></tr><tr><td>FQDN / IP Address </td><td><p> <br>FQDN represents the complete domain name of a machine or application on a network. For example: <a href="http://www.example.com/">www.example.com.</a> </p><p> </p><p>The numerical label assigned to each device connected to a computer network is called an "IP address." An IP address is typically represented in the format XXX.XXX.XXX.XX, where each "XXX" is a number ranging from 0 to 255, and the "XX" is a similar two-digit number. IP addresses are used to uniquely identify and locate devices on a network. </p></td></tr><tr><td>Port Number </td><td> A specific endpoint for data exchange between two devices or applications within a network. </td></tr><tr><td>Inventory Interval </td><td><p>This option defines frequency of Inventory Collector. Inventory Collector is responsible for: </p><p>·        Collecting server inventory like pending updates, installed applications, local administrators etc. </p><p>·        Collecting module inventory like virtual machines, web sites, databases etc. </p><p>·        Hardware Health Monitoring </p><p>·        Windows Firewall Logs </p><p>·        Change Tracking </p><p> </p></td></tr><tr><td>Stats Interval </td><td><p>This option defines frequency of Monitoring Collector. Monitoring Collector is responsible for: </p><p>·        Collecting all performance counters results </p><p>·        Collecting Event Logs </p><p>·        Collecting TCP Connections </p><p> </p></td></tr><tr><td>Logging Type </td><td>In Logging option, you can choose Statistic Collection Level. </td></tr><tr><td>Debug </td><td><p> </p><p>If you want to report an issue, you can enable extensive debugging with Debug Option.</p><ul><li>Inventory: Only collects debug logs for Inventory Collector</li><li>Monitoring: Only collects debug logs for Monitoring Collector</li><li>On: Collects debug logs for Inventory and Monitoring Collector</li></ul></td></tr><tr><td>Status </td><td><p>To choose a server status such as: </p><p>·        Active </p><p>·        Maintenance </p><p>·        Reconnect </p><p>·        Disabled </p></td></tr><tr><td><p> </p><p>HP 3ParInfo </p><p> </p></td><td><p>This is a hardware Integration component. You can set them as per the need.  Click the toggle button to get the field to add info. Type HP3ParInfo.exe path on server to activate HP 3Par Integration. </p><p>Example: </p><p><img src="../../../.gitbook/assets/image (548).png" alt=""> </p></td></tr><tr><td><p> </p><p>SuperMicro SuperDoctor 5 </p><p> </p></td><td><p>This is a hardware Integration component. You can set them as per the need.  Click the toggle button to get the field to add info. Type sdc.bat path on server to activate SuperMicro Integration. </p><p>Example:  </p><p><img src="../../../.gitbook/assets/image (549).png" alt=""> </p></td></tr><tr><td>Temporary Path </td><td>This option appears only for Linux and VMWare servers.  </td></tr></tbody></table>

7. After entering all the required info, click the button **SUMBIT**. The Windows server will be added now.

### Add a Linux Server

1. To add a Linux server, go to **Server Operations > Add Server** > then click the + button on the right corner, you get the **Add New Server** screen, where you need to select the **Server Type** as Linux.
2.  Select **Linux** from the Server Type field.

    <div align="left">

    <figure><img src="../../../.gitbook/assets/image (550).png" alt="" width="375"><figcaption></figcaption></figure>

    </div>
3. Select the appropriate trigger from the field Trigger

{% hint style="info" %}
**Note:** Trigger option is only available in Advanced Mode. You may want to assign the servers to a custom Trigger if target server is in an Isolated network or if you want to setup a scalable infrastructure. You will only see available Triggers in this field.&#x20;
{% endhint %}

4. Add **FQDN / IP** Address.
5. Select a **Credential Type** from the drop down:

* **None** – Select this type and add **Username** and **Password**&#x20;
* **Basic** – Selecting this option provides you with another Field called Credential from where you can select an appropriate option.
* **Key-based** – Selecting this option provides you with another Field called Credential from where you can select an appropriate option.&#x20;
* **Cyberark** – Selecting this option provides you with another Field called Credential from where you can select an appropriate option.&#x20;

6. Select the checkbox **key-Based Authentication** to enable SSH key-based authentication.
7.  Enter your SSH private key.

    <div align="left">

    <figure><img src="../../../.gitbook/assets/image (551).png" alt="" width="375"><figcaption></figcaption></figure>

    </div>
8. If your private key requires a passphrase, select the checkbox Enable Passphrase. This would bring up a field to enter the passphrase.
9. Enter the passphrase and click Submit to apply changes and add your Linux server.
10. If you want to add more advanced setting to your Linux server, select the checkbox Advanced Settings. You get the additional fields: Refer to the section [Advance Settings](add-new-server.md#advance-settings-refer-to-the-following-table-to-understand-the-fields-in-the-above-screen.).

### Add a VMWare Server

To add **VMWare** server, go to **Server Operations > Add Server** > then click the + button on the right corner, you get the **Add New Server** screen, where you need to select the **Server Type** as VMWare. Refer to the section **Add a Windows Server and Advance Settings.**
