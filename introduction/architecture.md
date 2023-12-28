# Architecture

All VirtualMetric components work on Windows platform and uses Microsoft technologies that you are already familiar.

<figure><img src="../.gitbook/assets/image (184).png" alt=""><figcaption></figcaption></figure>

## **VirtualMetric API**

All VirtualMetric components use VirtualMetric API to communicate with VirtualMetric DB. VirtualMetric API adds additional authentication layer called [ OWIN](https://github.com/owin/owin/wiki/FAQ#what-is-owin). All performance and inventory queries, authentication, dashboard and monitoring operations process on VirtualMetric API. VirtualMetric API uses Microsoft IIS Server for the web server role.\
\
You can access VirtualMetric API from your web browser. Default VirtualMetric API port is **8080**.

```
http://localhost:8080
```

If VirtualMetric API stops, then all operations would fail including Dashboard logins and monitoring. Notification system works directly from VirtualMetric Database via VirtualMetric SQL Jobs. When VirtualMetric API is offline, still you will be able to get notifications. You can check [Maintenance](https://cloud.virtualmetric.com/Documentation#installation-maintenance) section to repair VirtualMetric API.

{% hint style="info" %}
You can change default VirtualMetric API port during first setup. Please check [Installation](https://cloud.virtualmetric.com/Documentation#installation-section) section to change it during setup. You can also read [Maintenance](https://cloud.virtualmetric.com/Documentation#installation-maintenance) section to change the port later.
{% endhint %}

## VirtualMetric Dashboard

VirtualMetric Dashboard is the HTML based web interface to access VirtualMetric. You can use it to configure servers, to set up notifications, to review monitoring results and to create reports. This web interface is highly interactive, using Javascript to deliver a powerful and easy-to-use user experience. While you are logged in, the VirtualMetric Dashboard permanently refreshes the data on the screen permanently (via Ajax calls) so it always shows the current monitoring results (you can set refresh interval). VirtualMetric Dashboard uses Microsoft IIS Server for the web server role.\
\
Default VirtualMetric Dashboard port is **80**.

```markup
http://localhost
```

## **VirtualMetric Database**

VirtualMetric Database is the main datastore to hold all inventory and monitoring data. VirtualMetric Database is the most critical component. If VirtualMetric Database becomes unresponsive, you could not do any query via VirtualMetric API. VirtualMetric Database uses Microsoft SQL Server for the database role.

## **VirtualMetric Trigger**

VirtualMetric Trigger is the main component to connect servers, clusters and managers for monitoring and inventory collection. This component opens required TCP connections to initialize collector process, therefore, we also refer that as VirtualMetric Collector. You can install many VirtualMetric Triggers to monitor servers in the isolated networks like NAT, NVGRE, Virtual Network etc.

## **VirtualMetric Observer**

VirtualMetric Observer is the notification component of VirtualMetric. This component connects to VirtualMetric API to process active notification queue and execute the notification actions.
