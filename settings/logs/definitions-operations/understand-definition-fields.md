# Understand Definition Fields

1\.      To view the Definitions, go to **Logs > Definitions**. You get the following screen:&#x20;

<figure><img src="../../../.gitbook/assets/image (736).png" alt=""><figcaption></figcaption></figure>

2\.      Select type of the device.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (727).png" alt=""><figcaption></figcaption></figure>

</div>

3\.      Refer to the following table to understand the elements on the above screen.&#x20;

<table><thead><tr><th width="172">Fields</th><th>Descriptions</th></tr></thead><tbody><tr><td>Name </td><td><p>This field cannot be changed. </p><p>Provider Name determines which log provider will be collected by VirtualMetric. Provider name is only required for Windows and Linux servers. VMware Hosts does not have any log providers.</p></td></tr><tr><td>Retention Period </td><td><p>This field cannot be changed.</p><p>The retention period of logs signifies the duration for which log data is stored or maintained before it's automatically deleted or archived.</p></td></tr><tr><td>Event Type</td><td><p>The user has the option to filter logs using Event Type settings. Filter logs based on the following event types: </p><p>·       Critical </p><p>·       Error </p><p>·       Warning </p><p>·       Information </p><p><strong>Note:</strong> If you remove selections of all types, there will be no Event Type filtering. In that case, VirtualMetric Collector will also collect Verbose and Debug logs. </p></td></tr><tr><td>Event ID </td><td>Specific number for specifying event-id.</td></tr><tr><td>Keyword </td><td><p>You can filter logs by using Keyword. Keyword filtering is only available for Windows servers. You can type the keyword that you want to use for filtering. VirtualMetric Collector will use it immediately to filter logs.</p><p>You can use string and integer type of keywords.</p></td></tr><tr><td>Notes </td><td>Additional area for specifying notes.</td></tr><tr><td>Status </td><td>Displays the status whether active or disabled </td></tr></tbody></table>
