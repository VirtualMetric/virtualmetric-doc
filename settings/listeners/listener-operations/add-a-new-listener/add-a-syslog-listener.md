# Add a Syslog Listener

1\.      Go to **Listener > Syslog Listener** then, click the **Add (+)** button located in the upper right corner.&#x20;

<figure><img src="../../../../.gitbook/assets/image (310).png" alt=""><figcaption></figcaption></figure>

2\.      You will get the fields as follows.&#x20;

<div align="left">

<figure><img src="../../../../.gitbook/assets/image (311).png" alt="" width="292"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._&#x20;

<table><thead><tr><th width="266">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a listener. </td></tr><tr><td>Trigger</td><td>You may want to assign the servers to a custom Trigger if target server is in an Isolated network or if you want to setup a scalable infrastructure. You will only see available Triggers in this field.</td></tr><tr><td>Authentication Protocol</td><td><p>·       TCP: Transmission Control Protocol is a connection-oriented protocol that provides reliable and ordered delivery of data, making it suitable for applications such as file transfers and web browsing.</p><p>·       UDP: User Datagram Protocol, on the other hand, is a connectionless protocol that offers low-latency, but lacks reliability mechanisms, making it suitable for real-time applications like video streaming and online gaming.</p></td></tr><tr><td>Log Interval</td><td><p>The interval for fetching data.</p><p>·       Realtime</p><p>·       1 Minute</p><p>·       3 Minutes</p><p>·       5 Minutes</p></td></tr><tr><td>IP Address </td><td>The numerical label assigned to each device connected to a computer network is called an "IP address." An IP address is typically represented in the format XXX.XXX.XXX.XX, where each "XXX" is a number ranging from 0 to 255, and the "XX" is a similar two-digit number. IP addresses are used to uniquely identify and locate devices on a network. </td></tr><tr><td>Port Number </td><td> A specific endpoint for data exchange between two devices or applications within a network. </td></tr><tr><td>Forwarding Address </td><td>The forwarding address for syslog is the destination where syslog messages are sent for centralized logging. It can be an IP address or hostname of a server running syslog software or a syslog collector that aggregates log messages from multiple sources in a network. </td></tr><tr><td>Status </td><td><p>To choose a server status such as: </p><p>·       Active: Enables monitoring for server</p><p>·       Maintenance: Enables maintenance mode for server and disables all notifications</p><p>·       Reconnect: Restarts all collectors for server</p><p>·       Disabled: Disables monitoring for server</p></td></tr><tr><td>Debug </td><td><p>To choose debug such as:</p><p>·       Off</p><p>·       On: Collects debug logs for Inventory and Monitoring Collector</p></td></tr></tbody></table>

3\.      After entering all the required info, click the button **SUBMIT**.
