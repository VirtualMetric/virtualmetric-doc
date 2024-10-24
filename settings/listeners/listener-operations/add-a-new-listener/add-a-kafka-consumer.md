# Add a Kafka Consumer

1\.      Go to **Listener > Kafka Consumer** then click the **Add (+)** button located in the upper right corner.&#x20;

<figure><img src="../../../../.gitbook/assets/image (318).png" alt=""><figcaption></figcaption></figure>

2\.      You will get the fields as follows.

<div align="left">

<figure><img src="../../../../.gitbook/assets/image (319).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._&#x20;

<table><thead><tr><th width="199">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Name </td><td><p>This field only appears when enabled Advanced Settings is active.</p><p>A label or name that is assigned to a listener. </p></td></tr><tr><td>Trigger</td><td><p>This field only appears when enabled Advanced Settings is active.</p><p>You may want to assign the servers to a custom Trigger if target server is in an Isolated network or if you want to setup a scalable infrastructure. You will only see available Triggers in this field.</p></td></tr><tr><td>IP Address </td><td>The numerical label assigned to each device connected to a computer network is called an "IP address." An IP address is typically represented in the format XXX.XXX.XXX.XX, where each "XXX" is a number ranging from 0 to 255, and the "XX" is a similar two-digit number. IP addresses are used to uniquely identify and locate devices on a network. </td></tr><tr><td>Port Number </td><td> A specific endpoint for data exchange between two devices or applications within a network. </td></tr><tr><td>Credential Type</td><td><p>Select a proper credential type and credential.</p><p>·       <strong>None</strong></p><p>·       <strong>Basic:</strong> Selecting this option provides you with another Field called <strong>Credential</strong> from where you can select an appropriate option.</p></td></tr><tr><td>Username</td><td>Username for login redis </td></tr><tr><td>Partition</td><td>A Kafka partition is a portion of a topic's log, serving as the unit of parallelism and enabling distributed data storage and processing across multiple consumers within a consumer group.</td></tr><tr><td>Topic</td><td>A Kafka topic is a logical channel or category where messages are published by producers and consumed by subscribers, organizing related streams of data.</td></tr><tr><td>Algorithm</td><td><p>Choose appropriate Algorithm.</p><p>·       <strong>SHA256:</strong> SHA256 is a cryptographic hash function that generates a 256-bit (32-byte) hash value, widely used in security applications to ensure data integrity and verification.</p><p>·       <strong>SHA512:</strong> SHA512 is a cryptographic hash function that produces a 512-bit (64-byte) hash value, offering a higher level of security and resistance against brute-force attacks compared to shorter hash functions like SHA256.</p></td></tr><tr><td>Log Interval</td><td><p>The interval for fetching data.</p><p>·       Realtime</p><p>·       1 Minute</p><p>·       3 Minutes</p><p>·       5 Minutes</p></td></tr><tr><td>Status </td><td><p>To choose a server status such as: </p><p>·       <strong>Active:</strong> Enables monitoring for server</p><p>·       <strong>Maintenance:</strong> Enables maintenance mode for server and disables all notifications</p><p>·       <strong>Reconnect:</strong> Restarts all collectors for server</p><p>·       <strong>Disabled:</strong> Disables monitoring for server</p></td></tr><tr><td>Debug </td><td><p>To choose debug such as:</p><p>·       <strong>Off</strong></p><p>·       <strong>On:</strong> Collects debug logs for Inventory and Monitoring Collector</p></td></tr></tbody></table>

3\.      After entering all the required info, click the button **SUBMIT**.
