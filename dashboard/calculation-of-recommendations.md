# Calculation of Recommendations

In this section you will learn how VirtualMetric is calculating the recommendation under analysis.&#x20;

## CPU Recommendation&#x20;

The cpu recommendation report shows the cpu usage of devices and the recommendations provided by VirtualMetric.

<div align="left">

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

</div>

### VM



<table data-full-width="false"><thead><tr><th width="180">Metric Name</th><th width="379">Calculation</th><th>Statistical Operation</th></tr></thead><tbody><tr><td>CPU Limit (MHz)</td><td>Max Clock Speed * Processor Count * CPU Maximum / 100</td><td>MAX</td></tr><tr><td>CPU Usage (MHz)</td><td>(Max Clock Speed * Processor Count * CPU Maximum / 100) * Cpu Usage MHZ Percent/100</td><td>AVG</td></tr><tr><td>Recommended (MHz)</td><td>1.0 / 0.6 * Avg CPU Usage</td><td></td></tr><tr><td>Reclaimed (MHz)</td><td>Max CPU Limit - Recommended Limit MHz</td><td></td></tr><tr><td>Recommendation</td><td><p>◆ If Max CPU Limit - Recommended  = 0 <strong>No Change</strong></p><p>◆ If Max CPU Limit > Recommended <strong>Lower</strong></p><p>◆ If Max CPU Limit &#x3C; Recommended <strong>Increase</strong></p></td><td></td></tr></tbody></table>

***

### VMWare & Host

<table data-full-width="false"><thead><tr><th width="187">Metric Name</th><th width="362">Calculation</th><th>Statistical Operation</th></tr></thead><tbody><tr><td>CPU Limit (MHz)</td><td>Max Clock Speed * Processor Count</td><td>MAX</td></tr><tr><td>CPU Usage (MHz)</td><td>Average of Cpu Usage</td><td>AVG </td></tr><tr><td>Recommended (MHz)</td><td> 1.0 / 0.6 * Avg CPU Usage </td><td></td></tr><tr><td>Reclaimed (MHz)</td><td>Max CPU Limit - Recommended Limit MHz</td><td></td></tr><tr><td>Recommendation</td><td><p>◆ If Max CPU Limit - Recommended  = 0, <strong>No Change</strong></p><p>◆ If Max CPU Limit > Recommended, <strong>Lower</strong></p><p>◆ If Max CPU Limit &#x3C; Recommended, <strong>Increase</strong></p></td><td></td></tr></tbody></table>

***

## Memory Recommendation (VM, VMWare, Host)

The memory recommendation report shows the memory usage of devices and the recommendations provided by VirtualMetric.

<div align="left">

<figure><img src="../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

</div>

<table data-full-width="false"><thead><tr><th width="181">Metric Name</th><th width="374">Calculation</th><th>Statistical Operation</th></tr></thead><tbody><tr><td>Current Memory</td><td>Memory Capacity</td><td>AVG</td></tr><tr><td>Memory Usage</td><td>Memory Usage</td><td>AVG </td></tr><tr><td>Recommended (MB)</td><td> 1.0 / 0.6 * Avg CPU Usage </td><td></td></tr><tr><td>Reclaimed (MB)</td><td>Memory Capacity - Recommended Limit</td><td></td></tr><tr><td>Recommendation</td><td><p>◆ If Memory Capacity - Recommended Limit  = 0, <strong>No Change</strong></p><p>◆ If Memory Capacity > Recommended Limit, <strong>Lower</strong></p><p>◆ If Memory Capacity &#x3C; Recommended Limit, <strong>Increase</strong></p></td><td></td></tr></tbody></table>

***

## Powered off Report (VM, VMWare, Host)

The power-off report shows inactive devices and how long they have been off.

<div align="left">

<figure><img src="../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

</div>

<table data-full-width="false"><thead><tr><th width="214">Metric Name</th><th width="227">Calculation</th><th>Statistical Operation</th></tr></thead><tbody><tr><td>Duration</td><td>Current Date - Power Off Since</td><td></td></tr><tr><td>Powered Off Since</td><td>Epoch</td><td><p>◆ When counter value returns 0, MAX</p><p>◆ When counter value returns 1, MIN</p></td></tr><tr><td>Used Disk (MB)</td><td>Storage Used</td><td>MAX</td></tr><tr><td>Provisioned Disk (MB)</td><td>Total Storage</td><td>MAX</td></tr></tbody></table>

{% hint style="info" %}
All of the powered off reports have common condition;

State = 'Off' and Record Status > 0 and Since off > 0&#x20;
{% endhint %}

***

## Idle Report (VM, VMWare, Host)

<figure><img src="../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

This report displays idle machines in the environment. The report checks data from 14 days ago, and if the following rules are met, it marks the machines as idle:

1\)      The proportion of host, which has average CPU MHz below 100, is greater than 90%.

2\)     The proportion of host, which has average IO below 20, is greater than 90%.

2\)     The proportion of host, which has average network kbps below 1, is greater than 90%.

<table data-full-width="false"><thead><tr><th width="200">Metric Name</th><th width="260">Calculation</th><th>Statistical Operation</th></tr></thead><tbody><tr><td>Duration</td><td>Current Date - Date of Idle</td><td></td></tr><tr><td>Current CPU</td><td>Avg CPU</td><td>AVG</td></tr><tr><td>Memory Used</td><td>Storage Used</td><td>MAX</td></tr><tr><td>Memory Capacity</td><td>Total Storage</td><td>MAX</td></tr><tr><td>Used Disk (MB)</td><td>Consumed Memory</td><td>MAX</td></tr><tr><td>Disk Capacity (MB)</td><td>Total Memory</td><td>MAX</td></tr></tbody></table>

{% hint style="info" %}
All of the idle reports have common condition;

State = 'Running' and RecordStatus > 0&#x20;
{% endhint %}

