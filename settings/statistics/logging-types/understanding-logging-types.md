# Understanding Logging Types

Logging Levels determine the frequency at which statistic queries occur, the length of time statistical data is stored in the database and the type of statistical data that is collected. You can view the collected statistics through the performance charts on the VirtualMetric Dashboard and VirtualMetric Insight.

<figure><img src="../../../.gitbook/assets/image (188).png" alt=""><figcaption></figcaption></figure>

VirtualMetric offers **5 different Logging Levels by default:**

·       **Very Low:** Contains very low number of counters to monitor. Also keeps small amount of historic data in database.

·      **Low:** Contains low number of counters to monitor. Also keeps small amount of historic data in database.

·       **Medium:** Contains medium number of counters to monitor. Also keeps large amount of historic data in database.

·       **High:** Contains high number of counters to monitor. Also keeps large amount of historic data in database.

·       **Very High:** Contains very high number of counters to monitor. Also keeps maximum amount of historic data in database.

Statistics levels determine **counter levels** for monitoring. By modifying statistics level of counters, you can change type of statistical data that is collected and stored in VirtualMetric Database.

***

VirtualMetric offers **4 different Statistics Levels** by default:

·      **Level 1:** Contains critical counters for standard performance monitoring. \*Recommended\*

·      **Level 2:** Contains recommended counters for detailed performance monitoring.

&#x20;                                   Level 2 includes all the Level 1 counters.

·      **Level 3:** Contains deep dive counters for deep dive performance monitoring.

&#x20;                                   Level 3 includes all the Level 2 and Level 1 counters.

·       **Level 4:** Contains debug counters for debug level performance monitoring.

&#x20;                                   Level 4 includes all the Level 3, Level 2 and Level 1 counters.

&#x20;

{% hint style="info" %}
We suggest you to enable Level 4 and Level 3 counters when you only need to do deep dive troubleshooting.
{% endhint %}

***

**Aggregation levels** determine intervals of monitoring and length of time statistical data is stored in the VirtualMetric Database. VirtualMetric uses aggregation tables on VirtualMetric Database to serve you all reports and charts rapidly fast. When you request Average Usage of Last Week for a counter, VirtualMetric does not calculate usage, instead serves you from Hourly Aggregation table because this data is already calculated when counter is collected.

VirtualMetric offers **4 different Aggregation Levels** by default:

·       **Hourly Aggregation:** VirtualMetric aggregates real time monitoring data into hourly aggregation table.

·       **Daily Aggregation:** VirtualMetric aggregates hourly aggregation data into daily aggregation table.

·       **Weekly Aggregation:** VirtualMetric aggregates daily aggregation data into weekly aggregation table.

·       **Monthly Aggregation:** VirtualMetric aggregates weekly aggregation data into monthly aggregation table.

***

_**Aggregation Exercises**_

You can use different scenarios to cover different requirements with aggregation levels and statistics levels.

**Exercise 1:** Detailed monitoring for last hour, recommended monitoring for rest.

·       Hourly Aggregation: Use Level 2 for Statistics Level

·       Daily Aggregation: Use Level 1 for Statistics Level

·       Weekly Aggregation: Use Level 1 for Statistics Level

·       Monthly Aggregation: Use Level 1 for Statistics Level

***

**Exercise 2:** Deep dive monitoring for last hour, detailed monitoring for last week, recommended monitoring for rest.

·       Hourly Aggregation: Use Level 3 for Statistics Level

·       Daily Aggregation: Use Level 2 for Statistics Level

·       Weekly Aggregation: Use Level 2 for Statistics Level

·       Monthly Aggregation: Use Level 1 for Statistics Level

***

**Exercise 3:** Detailed monitoring for last hour, deep dive monitoring for last week, recommended monitoring for rest.

&#x20; _This scenario is not possible! To make this scenario, you supposed to have following configuration:_

·       Hourly Aggregation: Use Level 2 for Statistics Level

·       Daily Aggregation: Use Level 3 for Statistics Level

·       Weekly Aggregation: Use Level 3 for Statistics Level

·       Monthly Aggregation: Use Level 1 for Statistics Level

{% hint style="danger" %}
Could not place Level 3 counters on daily and weekly aggregation tables because we do not have Level 3 counters on Hourly Aggregation. So even if you choose Level 3, VirtualMetric will place Level 2 counters on daily and weekly aggregation tables.
{% endhint %}

***

**Exercise 4:** Deep dive monitoring for all time ranges.

·       Hourly Aggregation: Use Level 3 for Statistics Level

·       Daily Aggregation: Use Level 3 for Statistics Level

·       Weekly Aggregation: Use Level 3 for Statistics Level

·       Monthly Aggregation: Use Level 3 for Statistics Level
