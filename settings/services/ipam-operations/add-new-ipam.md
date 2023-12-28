# Add new IPAM

Before start monitoring IPAM, you should create a new IPAM entry.

1\.      Click to **IPAM** on the left pane.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (587).png" alt=""><figcaption></figcaption></figure>

</div>

2\.      On **IPAM Management** screen, click **Add (+)** button on the right top section.

<figure><img src="../../../.gitbook/assets/image (588).png" alt=""><figcaption></figcaption></figure>

3\.      You will get the fields as follows.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (589).png" alt="" width="292"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._&#x20;

<table><thead><tr><th width="206">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a IPAM. </td></tr><tr><td>IP Address</td><td>The numerical label assigned to each device connected to a computer network is called an "IP address." An IP address is typically represented in the format XXX.XXX.XXX.XX, where each "XXX" is a number ranging from 0 to 255, and the "XX" is a similar two-digit number. IP addresses are used to uniquely identify and locate devices on a network.</td></tr><tr><td>Trigger</td><td>You may want to assign the servers to a custom Trigger if target server is in an Isolated network or if you want to setup a scalable infrastructure. You will only see available Triggers in this field.</td></tr><tr><td>CIDR</td><td>Classless Inter-Domain Routing (CIDR) enables efficient allocation and management of IP addresses by utilizing variable-length subnet masking to group and organize IP addresses in a flexible and scalable manner.</td></tr><tr><td>Inventory Interval</td><td><p>This option defines frequency of Inventory Collector. Inventory Collector is responsible for: </p><p>·       Collecting server inventory like pending updates, installed applications, local administrators etc. </p><p>·       Collecting module inventory like virtual machines, web sites, databases etc. </p><p>·       Hardware Health Monitoring </p><p>·       Windows Firewall Logs </p><p>·       Change Tracking </p></td></tr><tr><td>Debug</td><td><p>To choose debug such as:</p><p>·       <strong>Off</strong></p><p>·       <strong>Inventory:</strong> Only collects debug logs for Inventory Collector</p><p>·       <strong>Monitoring:</strong> Only collects debug logs for Monitoring Collector</p><p>·       <strong>On:</strong> Collects debug logs for Inventory and Monitoring Collector</p></td></tr><tr><td>Status</td><td><p>To choose a server status such as: </p><p>·       <strong>Active:</strong> Enables monitoring for server</p><p>·       <strong>Maintenance:</strong> Enables maintenance mode for server and disables all notifications</p><p>·       <strong>Reconnect:</strong> Restarts all collectors for server</p><p>·       <strong>Disabled:</strong> Disables monitoring for server</p></td></tr><tr><td>Logging Type</td><td>Logging Levels determine the frequency at which statistic queries occur, the length of time statistical data is stored in the database and the type of statistical data that is collected.</td></tr></tbody></table>

4\.      After entering all the required info, click the button **SUBMIT**.
