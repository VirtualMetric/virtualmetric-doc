# Add a SMTP Listener

1\.      Go to **Listener > SMTP Listener** then click the **Add (+)** button located in the upper right corner.&#x20;

<figure><img src="../../../../.gitbook/assets/image (296).png" alt=""><figcaption></figcaption></figure>

2\.      You will get the fields as follows.

<div align="left">

<figure><img src="../../../../.gitbook/assets/image (297).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._&#x20;

<table><thead><tr><th width="185">Fields</th><th></th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a listener. </td></tr><tr><td>Trigger</td><td>You may want to assign the servers to a custom Trigger if target server is in an Isolated network or if you want to setup a scalable infrastructure. You will only see available Triggers in this field.</td></tr><tr><td>IP Address </td><td>The numerical label assigned to each device connected to a computer network is called an "IP address." An IP address is typically represented in the format XXX.XXX.XXX.XX, where each "XXX" is a number ranging from 0 to 255, and the "XX" is a similar two-digit number. IP addresses are used to uniquely identify and locate devices on a network. </td></tr><tr><td>Port Number </td><td> A specific endpoint for data exchange between two devices or applications within a network. </td></tr><tr><td>SSL Public Key</td><td>This field only appears when enabled TLS is active. An SSL (Secure Sockets Layer) public key is used for encryption and is shared openly, allowing others to encrypt data that can only be decrypted by the corresponding private key.</td></tr><tr><td>SSL Private Key</td><td>This field only appears when enabled TLS is active. The SSL private key, kept confidential, is used for decrypting data encrypted with the associated public key, ensuring secure communication between parties.</td></tr><tr><td>Log Interval</td><td><p>The interval for fetching data.</p><p>·       Realtime</p><p>·       1 Minute</p><p>·       3 Minutes</p><p>·       5 Minutes</p></td></tr><tr><td>Status </td><td><p>To choose a server status such as: </p><p>·       <strong>Active:</strong> Enables monitoring for server</p><p>·       <strong>Maintenance:</strong> Enables maintenance mode for server and disables all notifications</p><p>·       <strong>Reconnect:</strong> Restarts all collectors for server</p><p>·       <strong>Disabled:</strong> Disables monitoring for server</p></td></tr><tr><td>Debug </td><td><p>To choose debug such as:</p><p>·       <strong>Off</strong></p><p>·      <strong>On:</strong> Collects debug logs for Inventory and Monitoring Collector</p></td></tr></tbody></table>

&#x20;

&#x20;

3\.      After entering all the required info, click the button SUBMIT.
