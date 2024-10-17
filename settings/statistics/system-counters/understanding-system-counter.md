# Understanding System Counter

VirtualMetric provides complete visibility with its pre-configured more than 650 performance counters.

<figure><img src="../../../.gitbook/assets/image (209).png" alt=""><figcaption></figcaption></figure>

Select type of server and module.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (210).png" alt=""><figcaption></figcaption></figure>

</div>

***

<div align="left">

<figure><img src="../../../.gitbook/assets/image (211).png" alt=""><figcaption></figcaption></figure>

</div>

VirtualMetric offers **4 different Statistics Levels** by default:

·      **Level 1:** Contains critical counters for standard performance monitoring. \*Recommended\*

·      **Level 2:** Contains recommended counters for detailed performance monitoring.

&#x20;                                   Level 2 includes all the Level 1 counters.

·      **Level 3:** Contains deep dive counters for deep dive performance monitoring.

&#x20;                                   Level 3 includes all the Level 2 and Level 1 counters.

·       **Level 4:** Contains debug counters for debug level performance monitoring.

&#x20;                                   Level 4 includes all the Level 3, Level 2 and Level 1 counters.

{% hint style="info" %}
We suggest you to enable Level 4 and Level 3 counters when you only need to do deep dive troubleshooting.
{% endhint %}

***

_**Notification Options**_

In the System Counter settings, you can enable or disable all alerting systems including Email, SMS and Heatmap. By modifying thresholds of the counters, you can set their threshold limits and enable them on heatmap or activate notifications

<div align="left">

<figure><img src="../../../.gitbook/assets/image (213).png" alt=""><figcaption></figcaption></figure>

</div>

If you enable thresholds for a system counter, you should also set threshold limits to activate. You can also choose to receive notifications or see their health status on Heatmap

<div align="left">

<figure><img src="../../../.gitbook/assets/image (214).png" alt="" width="292"><figcaption></figcaption></figure>

</div>

***

_**Thresholds**_

If thresholds option is enabled, VirtualMetric uses notification thresholds to determine counter health status which are healthy, monitor, warning or critical.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (215).png" alt=""><figcaption></figcaption></figure>

</div>

VirtualMetric offers **4 different** **Thresholds** for alerting:

* &#x20;  _Healthy:_ That means counter is in recommended thresholds and considered as healthy
* &#x20;  _Monitor:_ That means counter is not in recommended thresholds but also it is not in danger zone. You should monitor activity of this counter because soon it may be in warning thresholds.
* &#x20;  _Warning:_ That means counter is in warning thresholds and considered as not healthy. You should troubleshoot issue before counter gets into critical level.
* &#x20;  _Critical:_ That means counter is in critical thresholds and considered as not healthy. Counter is in critical state so you must troubleshoot issue fast before your system becomes unresponsive

{% hint style="info" %}
VirtualMetric comes with some pre-defined threshold limits based on Microsoft and VMware recommendations.
{% endhint %}

***

_**Threshold Exercises**_

We can use different scenarios to cover different threshold configurations.

**Exercise 1:** CPU counter, 0%-60% is healthy, 61%-85% is monitor, 86%-95% is warning, %96-%100 is critical.

* **Healthy Min:** 0%
* **Healthy Max:** 60%
* **Monitor Min:** 61%
* **Monitor Max:** 85%
* **Warning Min:** 86%
* **Warning Max:** 95%
* **Critical Min:** 96%
* **Critical Max:** 100%

***

**Exercise 2:** CPU counter, %96-%100 is critical, other values are healthy.

* **Healthy Min:**
* **Healthy Max:**
* **Monitor Min:**
* **Monitor Max:**
* **Warning Min:**
* **Warning Max:**
* **Critical Min:** 96
* **Critical Max:** 100

{% hint style="info" %}
&#x20;If you don't type % for unit, VirtualMetric will add automatically.
{% endhint %}

***

**Exercise 3:** Disk counter, more than 5000 IOPS is critical, other values are healthy.\


* **Healthy Min:**
* **Healthy Max:**
* **Monitor Min:**
* **Monitor Max:**
* **Warning Min:**
* **Warning Max:**
* **Critical Min:** 5001
* **Critical Max:**

***

Exercise 4: Disk counter, 0-500 IOPS is healthy, 501-1000 IOPS is monitor, more than 1000 IOPS is warning.\


* **Healthy Min**: 0
* **Healthy Max:** 500
* **Monitor Min**: 501
* **Monitor Max:** 1000
* **Warning Min:** 1001
* **Warning Max:**
* **Critical Min:**
* **Critical Max:**

{% hint style="info" %}
&#x20;Using unit is not necessary for units like %, IOPS, packets etc.
{% endhint %}

***

Exercise 5: Paging counter, 0-300 MB is healthy, 300-500 MB is monitor, 500 MB-1 GB is warning, more than 1 GB is critical.

* **Healthy Min:** 0
* **Healthy Max:** 300 MB
* **Monitor Min:** 300 MB
* **Monitor Max:** 500 MB
* **Warning Min:** 500 MB
* **Warning Max:** 1 GB
* **Critical Min:** 1 GB
* **Critical Max:**

{% hint style="info" %}
&#x20;You can use different units like MB, GB in same threshold configuration.
{% endhint %}
