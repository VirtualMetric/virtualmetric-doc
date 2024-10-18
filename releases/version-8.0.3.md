# Version 8.0.3

**Release Date:** 08.10.2024

**New Features:**

* **Enhanced Cluster Management**: Introduced improved synchronization controls and refined permission checks for retrieving cluster and host group members.
* **SCVMM Node Maintenance Detection**: Added the ability to detect node maintenance to prevent false alarms and warnings.
* **Azure Communication Service Integration**: Added support for Azure Communication Service as an additional SMS provider.
* **Load Balancer Active/Passive Support**: Added active/passive configuration support for load balancers, controlled by the new "IsRoundRobin" parameter.

**Bug Fixes:**

* **SQLJobs for Clickhouse**: Resolved issues with SQLJobs not functioning properly and improved SQL recommendation jobs along with jobs for deleting older data.
* **Networklog Regex**: Corrected regex checks in network logs.
* **VirtualMetricGateway**: Resolved the bug that caused a failure when redirecting traffic from port 80 to 443.
* **Bulk Rule Enable/Disable**: Fixed an issue where enabling/disabling rules in bulk would cause them to disappear.
* **Performance Issue**: Fixed API performance issues that were causing high CPU usage.
* **Ping Loss Alarm**: Implemented a fix to resolve Ping Loss alarm testing and queue handling in Clickhouse.
* **Device Group Query**: Resolved an issue preventing the deletion of cluster queries when the list was empty.

**Improvements:**

* **Inventory Processing**: Streamlined logic for better status updates and logging.
* **User Authentication**: Enhanced user authentication by integrating LDAP for Active Directory validation.
* **Duplicate IP Handling**: A new parameter named ManagerNameSync has been added to prevent duplicates when adding SCVMM manager clusters. When enabled in the configuration, the system will check for cluster names across different triggers to avoid creating duplicates.

You can download the full update [here](https://virtualmetric.blob.core.windows.net/downloads/builds/release/v8.0.3/setup/virtualmetric-update-full.exe)

You can download the web sites update [here](https://virtualmetric.blob.core.windows.net/downloads/builds/release/v8.0.3/setup/virtualmetric-update-websites.exe):
