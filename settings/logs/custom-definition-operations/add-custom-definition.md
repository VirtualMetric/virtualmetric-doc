# Add Custom Definition

Before adding new Custom definition, you should create a new custom definition entry.

1\.      Click to **Custom Definition** on the left pane.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (743).png" alt=""><figcaption></figcaption></figure>

</div>

2\.      On **Custom Definitions Management** screen, click **Add (+)** button on the right top section.

<figure><img src="../../../.gitbook/assets/image (744).png" alt=""><figcaption></figcaption></figure>

3\.      Select type of Server.

<figure><img src="../../../.gitbook/assets/image (745).png" alt=""><figcaption></figcaption></figure>

4\.      Fields will change based on type.

## Type: File Based

File Based server type includes Windows (Server), Windows (Workstation), Linux (Server), Linux (Workstation)

<div align="left">

<figure><img src="../../../.gitbook/assets/image (746).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._

<table><thead><tr><th width="229">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a custom definition. </td></tr><tr><td>Retention Period</td><td>The retention period of logs signifies the duration for which log data is stored or maintained before it's automatically deleted or archived.</td></tr><tr><td>Groups</td><td><p>To provide visibility to either your own organization or all the other organizations. The options are: </p><p>·       My Organizations </p><p>·       All Organizations </p></td></tr><tr><td>Log Path</td><td>The log path represents the directory or location where log files are stored or generated within a system or application.</td></tr><tr><td>Category</td><td>Classification or grouping of log messages based on specific criteria or functionality for easier organization and filtering. </td></tr><tr><td>Collection should begin</td><td><p>Select a proper time frame from dropdown.</p><p>Initiation or start of log data aggregation or recording within a system or application.</p></td></tr><tr><td>Status</td><td>Custom definition can be enabled/disabled from status field.</td></tr></tbody></table>

## Type: Windows Event Based

Event based server type includes Windows (Server), Windows (Workstation)

<div align="left">

<figure><img src="../../../.gitbook/assets/image (214).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._

<table><thead><tr><th width="172">Fields</th><th>Descriptions</th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a custom definition. </td></tr><tr><td>Retention Period </td><td>The retention period of logs signifies the duration for which log data is stored or maintained before it's automatically deleted or archived.</td></tr><tr><td>Event Type</td><td><p>The user has the option to filter logs using Event Type settings. Filter logs based on the following event types: </p><p>·       Critical </p><p>·       Error </p><p>·       Warning </p><p>·       Information </p><p><strong>Note:</strong> If you remove selections of all types, there will be no Event Type filtering. In that case, VirtualMetric Collector will also collect Verbose and Debug logs. </p></td></tr><tr><td>Event ID </td><td>Specific number for specifying event-id.</td></tr><tr><td>Keyword </td><td><p>You can filter logs by using Keyword. Keyword filtering is only available for Windows servers. You can type the keyword that you want to use for filtering. VirtualMetric Collector will use it immediately to filter logs.</p><p>You can use string and integer type of keywords.</p></td></tr><tr><td>Notes </td><td>Additional area for specifying notes.</td></tr><tr><td>Visibility</td><td><p>To provide visibility to either your own organization or all the other organizations. The options are: </p><p>·       My Organizations </p><p>·       All Organizations </p></td></tr></tbody></table>

## Type: SNMP OID

<div align="left">

<figure><img src="../../../.gitbook/assets/image (215).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._

<table><thead><tr><th width="172">Fields</th><th>Descriptions</th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a custom definition. </td></tr><tr><td>Retention Period </td><td>The retention period of logs signifies the duration for which log data is stored or maintained before it's automatically deleted or archived.</td></tr><tr><td>OID (1)</td><td>OID can be imported from an internal system (1)</td></tr><tr><td>OID (2)</td><td><p>OID can be added by adding manually (2)</p><p><img src="../../../.gitbook/assets/image (216).png" alt="" data-size="original"></p><p>·       <strong>Name:</strong> A label or name that is assigned to an OID. </p><p>·       <strong>OID:</strong> Unique sequence of numbers used in network management systems like SNMP to identify managed objects in a hierarchical tree structure.</p><p>·       <strong>Regex:</strong> Sequence of characters that defines a search pattern, aiding in string matching and manipulation within text.</p><p>·       <strong>Type:</strong> Select the type of OID between <strong>String</strong> and <strong>Number</strong></p></td></tr><tr><td>Visibility</td><td><p>To provide visibility to either your own organization or all the other organizations. The options are: </p><p>·       My Organizations </p><p>·       All Organizations </p></td></tr><tr><td>Status</td><td>Custom definition can be enabled/disabled from status field.</td></tr></tbody></table>

## Type: Syslog

<div align="left">

<figure><img src="../../../.gitbook/assets/image (217).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._

<table><thead><tr><th width="172">Fields</th><th>Descriptions</th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a custom definition. </td></tr><tr><td>Retention Period </td><td>The retention period of logs signifies the duration for which log data is stored or maintained before it's automatically deleted or archived.</td></tr><tr><td>Event Type</td><td><p>The user has the option to filter logs using Event Type settings. Filter logs based on the following event types: </p><p>·       Critical </p><p>·       Error </p><p>·       Warning </p><p>·       Information </p><p><strong>Note:</strong> If you remove selections of all types, there will be no Event Type filtering. In that case, VirtualMetric Collector will also collect Verbose and Debug logs. </p></td></tr><tr><td>Source IP Address</td><td>Unique numerical label assigned to a device initiating a data packet in a network, indicating the origin of the communication.</td></tr><tr><td>Visibility</td><td><p>To provide visibility to either your own organization or all the other organizations. The options are: </p><p>·       My Organizations </p><p>·       All Organizations </p></td></tr><tr><td>Category</td><td>Classification or grouping of log messages based on specific criteria or functionality for easier organization and filtering. </td></tr><tr><td>Status</td><td>Custom definition can be enabled/disabled from status field.</td></tr></tbody></table>

## Type: Stream Based

Stream Based server type includes TCP, UDP, HTTP, SMTP

<div align="left">

<figure><img src="../../../.gitbook/assets/image (218).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._

<table><thead><tr><th width="172">Fields</th><th>Descriptions</th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a custom definition. </td></tr><tr><td>Retention Period </td><td>The retention period of logs signifies the duration for which log data is stored or maintained before it's automatically deleted or archived.</td></tr><tr><td>Source IP Address</td><td>Unique numerical label assigned to a device initiating a data packet in a network, indicating the origin of the communication.</td></tr><tr><td>Visibility</td><td><p>To provide visibility to either your own organization or all the other organizations. The options are: </p><p>·       My Organizations </p><p>·       All Organizations </p></td></tr><tr><td>Category</td><td>Classification or grouping of log messages based on specific criteria or functionality for easier organization and filtering. </td></tr><tr><td>Status</td><td>Custom definition can be enabled/disabled from status field.</td></tr></tbody></table>

## Type: SNMP Trap

<div align="left">

<figure><img src="../../../.gitbook/assets/image (219).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._

<table><thead><tr><th width="172">Fields</th><th>Descriptions</th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a custom definition. </td></tr><tr><td>Retention Period </td><td>The retention period of logs signifies the duration for which log data is stored or maintained before it's automatically deleted or archived.</td></tr><tr><td>Source IP Address</td><td>Unique numerical label assigned to a device initiating a data packet in a network, indicating the origin of the communication.</td></tr><tr><td>SNMP Trap OID</td><td>Unique identifier used to categorize and identify specific events or conditions reported through SNMP traps in network management systems.</td></tr><tr><td>Visibility</td><td><p>To provide visibility to either your own organization or all the other organizations. The options are: </p><p>·       My Organizations </p><p>·       All Organizations </p></td></tr><tr><td>Category</td><td>Classification or grouping of log messages based on specific criteria or functionality for easier organization and filtering. </td></tr><tr><td>Status</td><td>Custom definition can be enabled/disabled from status field.</td></tr></tbody></table>

## Type: TFTP

<div align="left">

<figure><img src="../../../.gitbook/assets/image (220).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._

<table><thead><tr><th width="172">Fields</th><th>Descriptions</th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a custom definition. </td></tr><tr><td>Retention Period </td><td>The retention period of logs signifies the duration for which log data is stored or maintained before it's automatically deleted or archived.</td></tr><tr><td>Event Type</td><td><p>The user has the option to filter logs using Event Type settings. Filter logs based on the following event types: </p><p>·       Critical </p><p>·       Error </p><p>·       Warning </p><p>·       Information </p><p><strong>Note:</strong> If you remove selections of all types, there will be no Event Type filtering. In that case, VirtualMetric Collector will also collect Verbose and Debug logs. </p></td></tr><tr><td>Event ID </td><td>Specific number for specifying event-id.</td></tr><tr><td>Keyword </td><td><p>You can filter logs by using Keyword. Keyword filtering is only available for Windows servers. You can type the keyword that you want to use for filtering. VirtualMetric Collector will use it immediately to filter logs.</p><p>You can use string and integer type of keywords.</p></td></tr><tr><td>Notes </td><td>Additional area for specifying notes.</td></tr><tr><td>Visibility</td><td><p>To provide visibility to either your own organization or all the other organizations. The options are: </p><p>·       My Organizations </p><p>·       All Organizations </p></td></tr></tbody></table>

## Type: Stream Based Queue Systems

Stream Based queue systems includes Redis, Kafka, RabbitMQ, Nats

<div align="left">

<figure><img src="../../../.gitbook/assets/image (221).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._

<table><thead><tr><th width="172">Fields</th><th>Descriptions</th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a custom definition. </td></tr><tr><td>Retention Period </td><td>The retention period of logs signifies the duration for which log data is stored or maintained before it's automatically deleted or archived.</td></tr><tr><td>Visibility</td><td><p>To provide visibility to either your own organization or all the other organizations. The options are: </p><p>·       My Organizations </p><p>·       All Organizations </p></td></tr><tr><td>Category</td><td>Classification or grouping of log messages based on specific criteria or functionality for easier organization and filtering. </td></tr><tr><td>Status</td><td>Custom definition can be enabled/disabled from status field.</td></tr></tbody></table>

## Type: Synthetic Check

<div align="left">

<figure><img src="../../../.gitbook/assets/image (222).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._

<table><thead><tr><th width="172">Fields</th><th>Descriptions</th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a custom definition. </td></tr><tr><td>Retention Period </td><td>The retention period of logs signifies the duration for which log data is stored or maintained before it's automatically deleted or archived.</td></tr><tr><td>Visibility</td><td><p>To provide visibility to either your own organization or all the other organizations. The options are: </p><p>·       My Organizations </p><p>·       All Organizations </p></td></tr><tr><td>Transaction Definitions</td><td>A transaction definition outlines a set of operations treated as a single, atomic unit of work within a database, ensuring all actions either succeed or fail together.</td></tr><tr><td>Time Period</td><td><p>Select a proper time period from dropdown.</p><p>Specific duration or interval between two points in time. </p></td></tr><tr><td>Timeout</td><td>Duration within which an operation or process is expected to complete before being considered unsuccessful or interrupted.</td></tr><tr><td>Status</td><td>Custom definition can be enabled/disabled from status field.</td></tr></tbody></table>

## Type: HTTP Check

<div align="left">

<figure><img src="../../../.gitbook/assets/image (223).png" alt="" width="290"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._

<table><thead><tr><th width="172">Fields</th><th>Descriptions</th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a custom definition. </td></tr><tr><td>Retention Period </td><td>The retention period of logs signifies the duration for which log data is stored or maintained before it's automatically deleted or archived.</td></tr><tr><td>Visibility</td><td><p>To provide visibility to either your own organization or all the other organizations. The options are: </p><p>·       My Organizations </p><p>·       All Organizations </p></td></tr><tr><td>URL</td><td>It is a web address that specifies the location of a resource on the internet.</td></tr><tr><td>Credential Type</td><td><p>Select a proper credential type and credential.</p><p>·       <strong>None</strong></p><p>·       <strong>Basic</strong> – Selecting this option provides you with another Field called Credential from where you can select an appropriate option.</p><p>·       <strong>HMAC</strong> – Selecting this option provides you with another Field called Credential from where you can select an appropriate option.</p><p>·       <strong>HTTP Header</strong> – Selecting this option provides you with another Field called Credential from where you can select an appropriate option.</p></td></tr><tr><td>Content Type</td><td><p>API content type specifies the format of the data being sent or received in an API request or response. </p><p>Examples:</p><p>·       application/json</p><p>·       application/xml</p></td></tr><tr><td>Time Period</td><td><p>Select a proper time period from dropdown.</p><p>Specific duration or interval between two points in time. </p></td></tr><tr><td>Timeout</td><td>Duration within which an operation or process is expected to complete before being considered unsuccessful or interrupted.</td></tr><tr><td>Status</td><td>Custom definition can be enabled/disabled from status field.</td></tr></tbody></table>

## Type: Script Check

<div align="left">

<figure><img src="../../../.gitbook/assets/image (224).png" alt="" width="291"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._

<table><thead><tr><th width="172">Fields</th><th>Descriptions</th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a custom definition. </td></tr><tr><td>Retention Period </td><td>The retention period of logs signifies the duration for which log data is stored or maintained before it's automatically deleted or archived.</td></tr><tr><td>Visibility</td><td><p>To provide visibility to either your own organization or all the other organizations. The options are: </p><p>·       My Organizations </p><p>·       All Organizations </p></td></tr><tr><td>File Name</td><td>The name assigned to a file, identifying it within a file system.</td></tr><tr><td>Interpretor Type</td><td><p>Select a proper interpretor type from dropdown.</p><p>·       <strong>Exe:</strong> An executable file containing machine code that can be run directly by an operating system.</p><p>·       <strong>Shell:</strong> The user interface enabling interaction with an operating system, interpreting commands and executing programs.</p><p>·       <strong>Powershell:</strong> A command-line shell and scripting language designed for task automation and configuration management in Windows environments. </p></td></tr><tr><td>Credential Type</td><td><p>Select a proper credential type and credential.</p><p>·       <strong>None</strong></p><p>·       <strong>Basic</strong> – Selecting this option provides you with another Field called Credential from where you can select an appropriate option.</p><p>·       <strong>HMAC</strong> – Selecting this option provides you with another Field called Credential from where you can select an appropriate option.</p><p>·       <strong>HTTP Header</strong> – Selecting this option provides you with another Field called Credential from where you can select an appropriate option.</p></td></tr><tr><td>Time Period</td><td><p>Select a proper time period from dropdown.</p><p>Specific duration or interval between two points in time. </p></td></tr><tr><td>Timeout</td><td>Duration within which an operation or process is expected to complete before being considered unsuccessful or interrupted.</td></tr><tr><td>Status</td><td>Custom definition can be enabled/disabled from status field.</td></tr></tbody></table>

## Type: Query Based

<div align="left">

<figure><img src="../../../.gitbook/assets/image (225).png" alt="" width="288"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._

<table><thead><tr><th width="172">Fields</th><th>Descriptions</th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a custom definition. </td></tr><tr><td>Retention Period </td><td>The retention period of logs signifies the duration for which log data is stored or maintained before it's automatically deleted or archived.</td></tr><tr><td>Visibility</td><td><p>To provide visibility to either your own organization or all the other organizations. The options are: </p><p>·       My Organizations </p><p>·       All Organizations </p></td></tr><tr><td>Query Editor</td><td>A query editor is a tool or interface that allows users to write, modify, and execute database queries, typically providing features for syntax highlighting and error checking.</td></tr><tr><td>Time Period</td><td><p>Select a proper time period from dropdown.</p><p>Specific duration or interval between two points in time. </p></td></tr><tr><td>Timeout</td><td>Duration within which an operation or process is expected to complete before being considered unsuccessful or interrupted.</td></tr><tr><td>Status</td><td>Custom definition can be enabled/disabled from status field.</td></tr></tbody></table>

5\.      After adding fields of the custom definition, additional configuration can be added from **advance settings** for some of the types.

## Advanced Settings

<div align="left">

<figure><img src="../../../.gitbook/assets/image (226).png" alt="" width="155"><figcaption></figcaption></figure>

</div>

### Timezone

<div align="left">

<figure><img src="../../../.gitbook/assets/image (227).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

1\) Select a proper time zone mode.

* Use time zone from log file. If none is detected use
* Ignore time zone from log file and instead use

2\) Select a proper time zone from dropdown.

### Custom Date Format

<div align="left">

<figure><img src="../../../.gitbook/assets/image (228).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

Sometimes log files can contain different types of date format. Custom date format can be added from this field.

**Example 1:** &#x20;

**Date:** 2022-09-06 05:48:20&#x20;

**Pattern:** \d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}&#x20;

**Date Format:** YYYY-MM-DD HH:mm:ss&#x20;

**Example 2:**&#x20;

**Date:** 202209060548&#x20;

**Pattern:** \d{12}n&#x20;

**Date Format:** YYYYMMDDHHmm&#x20;

**Example 3:** &#x20;

**Date:** 05:48 06.09.2022&#x20;

**Pattern:** \d{2}:\d{2} \d{4}-\d{2}-\d{2}&#x20;

**Date Format:** YYYYMMDDHHmm

### Custom Field Parser

<div align="left">

<figure><img src="../../../.gitbook/assets/image (229).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

Sometimes log files can contain different types of field formats. Custom field parser can be added from this field. After adding a sample you will see data columns under the sample field. Columns can be selected.

**Example 1:**&#x20;

<div align="left">

<figure><img src="../../../.gitbook/assets/image (230).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

**Example 2:**

<div align="left">

<figure><img src="../../../.gitbook/assets/image (231).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

**Example 3:**&#x20;

<div align="left">

<figure><img src="../../../.gitbook/assets/image (232).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

### Custom Line Parser

<div align="left">

<figure><img src="../../../.gitbook/assets/image (233).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

Regex can be written for parse the line

**Example:**&#x20;

<div align="left">

<figure><img src="../../../.gitbook/assets/image (234).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

### Data Masking Rule

There are two modes in this part. Users can write any word or regex.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (236).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

<div align="left">

<figure><img src="../../../.gitbook/assets/image (237).png" alt="" width="294"><figcaption></figcaption></figure>

</div>

**Example:**&#x20;

<div align="left">

<figure><img src="../../../.gitbook/assets/image (239).png" alt="" width="294"><figcaption></figcaption></figure>

</div>

### Data Filter Rules

There are two modes in this part. Users can write any word or regex.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (240).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

1. Select a proper reader mode.

* Ingest all except matched lines: Shows logs which contain written pattern.
* Ingest only matched lines: Shows logs which do not contain written pattern.

2. Click Add button

<div align="left">

<figure><img src="../../../.gitbook/assets/image (241).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

Example:

<div align="left">

<figure><img src="../../../.gitbook/assets/image (243).png" alt="" width="296"><figcaption></figcaption></figure>

</div>

### Encoding

This is the process of converting data from one format or representation to another. For example, in computing, encoding can refer to converting text characters into binary code for storage or transmission, such as ASCII or UTF-8 encoding.&#x20;

Select a proper encoding type from dropdown.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (244).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

6\.      After adding all required fields click **SUBMIT.**
