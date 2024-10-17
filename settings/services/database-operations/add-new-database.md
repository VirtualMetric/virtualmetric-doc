# Add new Database

Before start monitoring Database, you should create a new Database entry.

1\.      Click to **Database** on the left pane.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (616).png" alt=""><figcaption></figcaption></figure>

</div>

2\.      On **Database Management** screen, click **Add (+)** button on the right top section.

<figure><img src="../../../.gitbook/assets/image (617).png" alt=""><figcaption></figcaption></figure>

3\.      You will get the fields as follows.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (618).png" alt="" width="292"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._&#x20;

<table><thead><tr><th width="206">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Database Type</td><td><p>Select proper type from dropdown.</p><p>·       <strong>Microsoft SQL:</strong> Relational database management system (RDBMS) developed by Microsoft, offering comprehensive data storage, retrieval, and management capabilities for various applications and industries.</p><p>·       <strong>SAP HANA:</strong> SAP HANA is an in-memory database platform that accelerates data processing and analytics, providing real-time insights and enabling rapid application development for businesses.</p></td></tr><tr><td>Name </td><td>A label or name that is assigned to a Database. </td></tr><tr><td>IP Address / Instance</td><td>The numerical label assigned to each device connected to a computer network is called an "IP address." An IP address is typically represented in the format XXX.XXX.XXX.XX, where each "XXX" is a number ranging from 0 to 255, and the "XX" is a similar two-digit number. IP addresses are used to uniquely identify and locate devices on a network.</td></tr><tr><td>Database Name</td><td>Unique identifier for a collection of organized data within a database management system, distinguishing it from other databases within the same environment.</td></tr><tr><td>Credential Type</td><td><p>Select a proper credential type and credential.</p><p>·       <strong>None:</strong> Select this type and add Username and Password </p><p>·       <strong>Basic:</strong> Selecting this option provides you with another Field called Credential from where you can select an appropriate option.  </p><p>·       <strong>Cyberark:</strong> Selecting this option provides you with another Field called Credential from where you can select an appropriate option. </p></td></tr><tr><td>Trigger</td><td>You may want to assign the servers to a custom Trigger if target server is in an Isolated network or if you want to setup a scalable infrastructure. You will only see available Triggers in this field.</td></tr><tr><td>Port</td><td>A specific endpoint for data exchange between two devices or applications within a network.</td></tr><tr><td>Inventory Interval</td><td><p>This option defines frequency of Inventory Collector. Inventory Collector is responsible for: </p><p>·       Collecting server inventory like pending updates, installed applications, local administrators etc. </p><p>·       Collecting module inventory like virtual machines, web sites, databases etc. </p><p>·       Hardware Health Monitoring </p><p>·       Windows Firewall Logs </p><p>·       Change Tracking </p></td></tr><tr><td>Stats Interval</td><td><p>This option defines frequency of Monitoring Collector. Monitoring Collector is responsible for: </p><p>·       Collecting all performance counters results </p><p>·       Collecting Event Logs </p><p>·       Collecting TCP Connections </p></td></tr><tr><td>Debug</td><td><p>To choose debug such as:</p><p>·       <strong>Off</strong></p><p>·       <strong>Inventory:</strong> Only collects debug logs for Inventory Collector</p><p>·       <strong>Monitoring:</strong> Only collects debug logs for Monitoring Collector</p><p>·       <strong>On:</strong> Collects debug logs for Inventory and Monitoring Collector</p></td></tr><tr><td>Status</td><td><p>To choose a server status such as: </p><p>·       <strong>Active:</strong> Enables monitoring for server</p><p>·       <strong>Maintenance:</strong> Enables maintenance mode for server and disables all notifications</p><p>·       <strong>Reconnect:</strong> Restarts all collectors for server</p><p>·       <strong>Disabled:</strong> Disables monitoring for server</p></td></tr><tr><td>Logging Type</td><td>Logging Levels determine the frequency at which statistic queries occur, the length of time statistical data is stored in the database and the type of statistical data that is collected.</td></tr></tbody></table>

4\.      After entering all the required info, click the button **SUBMIT**.
