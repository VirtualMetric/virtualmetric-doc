# Definitions Operations

Collector Definitions is the group of definitions which can be used to determine which information will be gathered from target servers, the frequency of these information and settings that VirtualMetric will use to collect data. You can enable and disable the group and change the frequency and settings of the definitions, so VirtualMetric Collector can use these definitions to collect the appropriate information from the target servers. Changing definition settings will be immediately applied to VirtualMetric Collectors.

<figure><img src="../../.gitbook/assets/image (755).png" alt=""><figcaption><p><strong>VirtualMetric Collector Definitions Screen</strong></p></figcaption></figure>

VirtualMetric contains built-in collector definitions. You **can not add custom definitions**, but you can modify existing ones to define which information you want to collect from target servers.

Firstly you need to select the **type** of **device.**

<div align="left">

<figure><img src="../../.gitbook/assets/image (272).png" alt="" width="250"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields of definition screen._&#x20;

<table><thead><tr><th width="218">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Collector Type</td><td><p>·       <strong>Stats Collector:</strong> Mostly collects realtime performance data, event logs, TCP connections etc. Change Tracking feature is not available for this collector. Due to the type of this collector, you can not set different intervals for the definitions which are assigned to this collector. The number of enabled definition in this collector may impact the performance of VirtualMetric API and increase resource usage on target servers.</p><p>·       Inventory Collector: Collects inventory based information and reports from target servers. You can set the frequency of these reports by changing their intervals. You can enable or disable Change Tracking feature for the definitions which are assigned to this collector.</p><p>·       German</p><p>·       Turkish</p></td></tr><tr><td>Change Tracking</td><td>VirtualMetric keeps a state of all inventory collections and compares them to find changes. Change Tracking will help you to detect undesired changes and give you brief information of system updates.</td></tr><tr><td>Interval</td><td>You can customize collector frequency for different definitions by changing intervals.</td></tr><tr><td>Settings</td><td><p>It's possible to apply some rules via settings to VirtualMetric Collector. Please check Definition Settings to see what options you have. You can filter inventory collection by changing these settings.</p><p>If settings option is empty for a definition, that means, the definition has no custom filtering support.</p></td></tr></tbody></table>
