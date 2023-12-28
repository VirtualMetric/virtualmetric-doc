# Add new DNS

Before start monitoring DNS, you should create a new DNS entry.

1\.      Click to **DNS** on the left pane.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (577).png" alt=""><figcaption></figcaption></figure>

</div>

2\.      On **DNS Management** screen, click **Add (+)** button on the right top section.

<figure><img src="../../../.gitbook/assets/image (578).png" alt=""><figcaption></figcaption></figure>

3\.      You will get the fields as follows.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (579).png" alt="" width="293"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._&#x20;

<table><thead><tr><th width="206">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a DNS. </td></tr><tr><td>DNS Server Address</td><td>It is a web address that specifies the location of a resource on the internet.</td></tr><tr><td>Port</td><td>A specific endpoint for data exchange between two devices or applications within a network. </td></tr><tr><td>Domain Name</td><td>Human-readable names to map to specific IP addresses</td></tr><tr><td>DNS Query Result</td><td>A DNS query result provides the mapping between a domain name and its associated IP address or other related information requested by the client querying the DNS server.</td></tr><tr><td>Type</td><td><p>Select proper dns type</p><p>·       <strong>A</strong>: Maps a domain name to an IPv4 address.</p><p>·       <strong>MX</strong>: Identifies mail servers responsible for receiving email on behalf of a domain.</p><p>·       <strong>NS</strong>: Indicates the authoritative name servers for a domain.</p><p>·       <strong>CNAME:</strong> Specifies an alias or canonical name for one domain to another domain name. </p><p>·       <strong>TXT:</strong> Stores text-based information, often used for verification or descriptive purposes. </p></td></tr><tr><td>Trigger</td><td>You may want to assign the servers to a custom Trigger if target server is in an Isolated network or if you want to setup a scalable infrastructure. You will only see available Triggers in this field.</td></tr><tr><td>Stats Interval</td><td><p>This option defines frequency of Monitoring Collector. Monitoring Collector is responsible for: </p><p>·       Collecting all performance counters results </p><p>·       Collecting Event Logs </p><p>·       Collecting TCP Connections </p></td></tr><tr><td>Debug</td><td><p>To choose debug such as:</p><p>·       <strong>Off</strong></p><p>·       <strong>Inventory:</strong> Only collects debug logs for Inventory Collector</p><p>·       <strong>Monitoring:</strong> Only collects debug logs for Monitoring Collector</p><p>·       <strong>On:</strong> Collects debug logs for Inventory and Monitoring Collector</p></td></tr><tr><td>Status</td><td><p>To choose a server status such as: </p><p>·       <strong>Active:</strong> Enables monitoring for server</p><p>·       <strong>Maintenance:</strong> Enables maintenance mode for server and disables all notifications</p><p>·       <strong>Reconnect:</strong> Restarts all collectors for server</p><p>·       <strong>Disabled:</strong> Disables monitoring for server</p></td></tr><tr><td>Logging Type</td><td>Logging Levels determine the frequency at which statistic queries occur, the length of time statistical data is stored in the database and the type of statistical data that is collected.</td></tr></tbody></table>

4\.      After entering all the required info, click the button **SUBMIT**.
