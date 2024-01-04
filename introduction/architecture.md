# Architecture

All VirtualMetric components work on Windows platform and uses Microsoft technologies that you are already familiar.

<figure><img src="../.gitbook/assets/image (184).png" alt=""><figcaption></figcaption></figure>

## **VirtualMetric API**

All VirtualMetric components utilize VirtualMetric API to communicate with VirtualMetric DB. The VirtualMetric API adds additional authentication layer called[ OWIN](https://github.com/owin/owin/wiki/FAQ#what-is-owin). All performance and inventory queries, authentication, dashboard and monitoring operations are processed through the VirtualMetric API. VirtualMetric API uses Microsoft IIS Server for the web server role.

You can access VirtualMetric API from your web browser. The default port for the VirtualMetric API is **8080**.

```
http://localhost:8080
```

If VirtualMetric API stops, all operations, including Dashboard logins and monitoring would fail. However, the notification system continues to function directly from the VirtualMetric Database through VirtualMetric SQL Jobs. Even when the VirtualMetric API is offline, you will still receive notifications. To address issues with the VirtualMetric API, you can refer to the [Maintenance](../installation/maintenance.md) section for repair instructions.

{% hint style="info" %}
You can change default VirtualMetric API port during first setup. Please check [Installation](broken-reference) section to change it during setup. You can also read [Maintenance](../installation/maintenance.md) section to change the port later.
{% endhint %}

## VirtualMetric Dashboard

VirtualMetric Dashboard serves as the HTML-based web interface for accessing VirtualMetric. It enables server configuration, notification setup, monitoring result review, and report creation. This interface offers high interactivity, leveraging Javascript to deliver a powerful and user-friendly experience. When logged in, the VirtualMetric Dashboard continuously refreshes data on the screen (via Ajax calls) to display real-time monitoring results (with a customizable refresh interval). For its web server role, the VirtualMetric Dashboard utilizes the Microsoft IIS Server.\
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
