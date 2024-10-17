# Add New Cluster

Select **Cluster Type,** enter **FQDN** of the server and other fields, then click **Submit** button.

{% hint style="info" %}
You should use FQDN of Cluster for monitoring. If you use IP Address, you may have connectivity issues.
{% endhint %}

<div align="left">

<figure><img src="../../../.gitbook/assets/image (514).png" alt="" width="309"><figcaption></figcaption></figure>

</div>

## Add a new Windows Cluster

1\.      Go to **Cluster** > **Add Cluster** > then click the **+** button located in the upper right corner.&#x20;

<figure><img src="../../../.gitbook/assets/image (473).png" alt=""><figcaption></figcaption></figure>

2\.      Select **Windows** from the **Cluster Type** field.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (470).png" alt=""><figcaption></figcaption></figure>

</div>

3\.      Select an appropriate trigger from the field **Trigger**.

4\.      Add **FQDN**

5\.      Select the checkbox **Active Directory Authentication** to use delegation of VirtualMetric service user credentials if target server is in same Active Directory.

When **Active Directory Authentication** is **disabled**, please select **credential type**.

6\.      Select the checkbox [Advance Settings](add-new-cluster.md#advance-settings). You get the fields as follows.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (472).png" alt="" width="292"><figcaption></figcaption></figure>

</div>

#### Advance Settings: Refer to the following table to understand the fields in the above screen.  <a href="#advance-settings" id="advance-settings"></a>

<table data-header-hidden><thead><tr><th width="287"></th><th></th></tr></thead><tbody><tr><td>Fields </td><td>Description </td></tr><tr><td>Cluster Name </td><td>A label or name that is assigned to a cluster. </td></tr><tr><td>Server Type </td><td>Cluster types such as Windows, VMWare, Openshift. </td></tr><tr><td>Trigger</td><td>You may want to assign the servers to a custom Trigger if target server is in an Isolated network or if you want to setup a scalable infrastructure. You will only see available Triggers in this field.</td></tr><tr><td>FQDN / IP Address </td><td><p> <br>FQDN represents the complete domain name of a machine or application on a network.  For example: <a href="http://www.example.com/">www.example.com.</a> </p><p> </p><p>The numerical label assigned to each device connected to a computer network is called an "IP address." An IP address is typically represented in the format XXX.XXX.XXX.XX, where each "XXX" is a number ranging from 0 to 255, and the "XX" is a similar two-digit number. IP addresses are used to uniquely identify and locate devices on a network. </p></td></tr><tr><td>Port Number </td><td> A specific endpoint for data exchange between two devices or applications within a network. </td></tr><tr><td>Inventory Interval </td><td><p>This option defines frequency of Inventory Collector. Inventory Collector is responsible for: </p><p>·       Collecting server inventory like pending updates, installed applications, local administrators etc. </p><p>·       Collecting module inventory like virtual machines, web sites, databases etc. </p><p>·       Hardware Health Monitoring </p><p>·       Windows Firewall Logs </p><p>·       Change Tracking </p><p> </p></td></tr><tr><td>Stats Interval </td><td><p>This option defines frequency of Monitoring Collector. Monitoring Collector is responsible for: </p><p>·       Collecting all performance counters results </p><p>·       Collecting Event Logs </p><p>·       Collecting TCP Connections </p><p> </p></td></tr><tr><td>Logging Type </td><td>Logging Levels determine the frequency at which statistic queries occur, the length of time statistical data is stored in the database and the type of statistical data that is collected.</td></tr><tr><td>Debug </td><td><p>To choose debug such as:</p><p>·       Off</p><p>·       Inventory: Only collects debug logs for Inventory Collector</p><p>·       Monitoring: Only collects debug logs for Monitoring Collector</p><p>·       On: Collects debug logs for Inventory and Monitoring Collector</p></td></tr><tr><td>Status </td><td><p>To choose a server status such as: </p><p>·       Active: Enables monitoring for server</p><p>·       Maintenance: Enables maintenance mode for server and disables all notifications</p><p>·       Reconnect: Restarts all collectors for server</p><p>·       Disabled: Disables monitoring for server</p></td></tr><tr><td><p> </p><p>HP 3ParInfo </p><p> </p></td><td><p>This is a hardware Integration component. You can set them as per the need.  Click the toggle button to get the field to add info. Type HP3ParInfo.exe path on server to activate HP 3Par Integration. </p><p>Example: </p><p><img src="../../../.gitbook/assets/image (474).png" alt="" data-size="original"></p></td></tr><tr><td><p> </p><p>SuperMicro SuperDoctor 5 </p><p> </p></td><td><p>This is a hardware Integration component. You can set them as per the need.  Click the toggle button to get the field to add info. Type sdc.bat path on server to activate SuperMicro Integration. </p><p>Example:  </p><p><img src="../../../.gitbook/assets/image (475).png" alt="" data-size="original"></p></td></tr></tbody></table>

&#x20;

7\.      After entering all the required info, click the button **SUBMIT**. The Windows cluster will be added now.

## Add a new VMware Cluster

1\.      Go to **Cluster** > **Add Cluster** > then click the **+** button located in the upper right corner.&#x20;

<figure><img src="../../../.gitbook/assets/image (476).png" alt=""><figcaption></figcaption></figure>

2\.      Select **VMware** from the Cluster Type field.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (477).png" alt="" width="293"><figcaption></figcaption></figure>

</div>

3\.      Select an appropriate trigger from the field **Trigger**.

4\.      Add **FQDN**

5\.      Select a **Credential Type** from the drop down:&#x20;

* **None** – Select this type and add Username and Password.
* **Basic** – Selecting this option provides you with another Field called Credential from where you can select an appropriate option. &#x20;
* **Cyberark** – Selecting this option provides you with another Field called Credential from where you can select an appropriate option.&#x20;

6\.      If you want to add more advanced setting to your Linux server, select the checkbox **Advanced Settings**. You get the additional fields: Refer to the section [Advance Settings](add-new-cluster.md#advance-settings).

## Add a new Openshift Cluster

1\.      Go to **Cluster** > **Add Cluster** > then click the **+** button located in the upper right corner.&#x20;

<figure><img src="../../../.gitbook/assets/image (478).png" alt=""><figcaption></figcaption></figure>

2\.      Select **Openshift** from the Cluster Type field.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (479).png" alt="" width="293"><figcaption></figcaption></figure>

</div>

3\.      Select an appropriate trigger from the field **Trigger**.

4\.      Add **FQDN**

5\.      Select a Credential Type from the drop down:&#x20;

* **None** – Select this type and add **API Key**
* **Bearer Token** – Selecting this option provides you with another Field called Credential from where you can select an appropriate option. &#x20;

{% hint style="info" %}
To get Openshift API Key, please follow the below commands.&#x20;
{% endhint %}

```
oc create sa virtualmetric
oc policy add-role-to-user cluster-reader system:serviceaccount:default:virtualmetric
oc adm policy add-cluster-role-to-user cluster-reader -z virtualmetric -n default
oc create token virtualmetric --duration=$((365*24))h -n default
```

6\.      If you want to add more advanced setting to your Linux server, select the checkbox Advanced Settings. You get the additional fields: Refer to the section [Advance Settings](add-new-cluster.md#advance-settings).
