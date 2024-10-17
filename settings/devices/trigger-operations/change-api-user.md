# Change API User

VirtualMetric Trigger uses API accounts to connect VirtualMetric API and query server list. For security reasons, you may need to change API account password or delete the account.

{% hint style="info" %}
**Information:** Please read _**API User Operations**_ section to learn more about API account operations
{% endhint %}

1\.      After you make your changes on API account, you should modify VirtualMetric Trigger config file:

```
C:\Program Files\VirtualMetric\Trigger\VirtualMetricTrigger.exe.config
```

2\.      On the config file, you will see following lines:

```xml
<appSettings>
	<add key="primaryApiUrl" value="https://api.virtualmetric.com:8080/API/"/>
	<add key="failoverApiUrl" value="" />
	<add key="triggerId" value="3080487f-f3f6-43e2-bd27-7f1886a12816" />
	<add key="apiUser" value="vmapi" />	
	<add key="apiPassword" value="727c9b3a51eb3407c7cc21c45d84bb28" />
</appSettings>
```

3\.      After changing these Trigger options, you should restart VirtualMetric Trigger scheduled task.\
Please open Task Scheduler on VirtualMetric Standalone Server.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (443).png" alt=""><figcaption></figcaption></figure>

</div>

4\.      Right click on VirtualMetric Trigger and click End from menu.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (444).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

5\.      Click Yes to confirm dialog.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (446).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

6\.      Wait for a few seconds. Then right click on VirtualMetric Trigger and click Run from menu.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (449).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

7\.      VirtualMetric Trigger will connect to VirtualMetric API and start monitoring in a few seconds.
