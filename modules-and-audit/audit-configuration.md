# Audit Configuration

You can easily change default settings of following audit reports:

* &#x20; Windows Defender
* &#x20; Windows Firewall
* &#x20; Object Access
* &#x20; File Change Tracking
* &#x20; Best Practice Analyzer
* &#x20; User Authentication

\
In this section, you will see configuration settings for these audit reports.

## Windows Defender

In order to enable Windows Defender reports, please make sure that Collector ID: 137 is enabled.

**Windows Defender Collector (ID: 137)**

<div align="left">

<figure><img src="../.gitbook/assets/image (887).png" alt=""><figcaption></figcaption></figure>

</div>

If Windows Defender collector is enabled, VirtualMetric also tracks Windows Event Logs for Windows Defender activities. VirtualMetric collects following events of Windows Defender:

**Windows Defender: Scan (ID: 82)**

<div align="left">

<figure><img src="../.gitbook/assets/image (888).png" alt=""><figcaption></figcaption></figure>

</div>

| Group                  | Event ID | Message                                             |
| ---------------------- | -------- | --------------------------------------------------- |
| Windows Defender: Scan | 1000     | An antimalware scan started.                        |
| Windows Defender: Scan | 1001     | An antimalware scan finished.                       |
| Windows Defender: Scan | 1002     | An antimalware scan was stopped before it finished. |
| Windows Defender: Scan | 1003     | An antimalware scan was paused.                     |
| Windows Defender: Scan | 1004     | An antimalware scan was resumed.                    |
| Windows Defender: Scan | 1005     | An antimalware scan started.                        |

**Windows Defender: Action (ID: 83)**

<div align="left">

<figure><img src="../.gitbook/assets/image (889).png" alt=""><figcaption></figcaption></figure>

</div>

<table><thead><tr><th width="258">Group</th><th width="107.33333333333331">Event ID</th><th>Message</th></tr></thead><tbody><tr><td>Windows Defender: Action</td><td>1007</td><td>The antimalware platform performed an action to protect your system from malware or other potentially unwanted software.</td></tr><tr><td>Windows Defender: Action</td><td>1008</td><td>The antimalware platform attempted to perform an action to protect your system from malware or other potentially unwanted software, but the action failed.</td></tr><tr><td>Windows Defender: Action</td><td>1117</td><td>The antimalware platform performed an action to protect your system from malware or other potentially unwanted software.</td></tr><tr><td>Windows Defender: Action</td><td>1118</td><td>The antimalware platform attempted to perform an action to protect your system from malware or other potentially unwanted software, but the action failed.</td></tr><tr><td>Windows Defender: Action</td><td>1119</td><td>The antimalware platform encountered a critical error when trying to take action on malware or other potentially unwanted software. There are more details in the event message.</td></tr></tbody></table>

**Windows Defender: Detection (ID: 84)**

<figure><img src="../.gitbook/assets/image (890).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="283">Group</th><th width="123.33333333333331">Event ID</th><th>Message</th></tr></thead><tbody><tr><td>Windows Defender: Detection</td><td>1006</td><td>The antimalware engine found malware or other potentially unwanted software.</td></tr><tr><td>Windows Defender: Detection</td><td>1015</td><td>The antimalware platform detected suspicious behavior.</td></tr><tr><td>Windows Defender: Detection</td><td>1116</td><td>The antimalware platform detected malware or other potentially unwanted software.</td></tr></tbody></table>

**Windows Defender: Quarantine (ID: 86)**

<figure><img src="../.gitbook/assets/image (891).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="289">Group</th><th width="121.33333333333331">Event ID</th><th>Message</th></tr></thead><tbody><tr><td>Windows Defender: Quarantine</td><td>1009</td><td>The antimalware platform restored an item from quarantine.</td></tr><tr><td>Windows Defender: Quarantine</td><td>1010</td><td>The antimalware platform could not restore an item from quarantine.</td></tr><tr><td>Windows Defender: Quarantine</td><td>1011</td><td>The antimalware platform deleted an item from quarantine.</td></tr><tr><td>Windows Defender: Quarantine</td><td>1012</td><td>The antimalware platform could not delete an item from quarantine.</td></tr></tbody></table>

\
Please make sure that these Event Log definitions are also enabled. You can always customize these settings to filter Windows Defender events.

## Windows Firewall

In order to enable Windows Firewall reports, please make sure that Collector ID: 54 is enabled.

**Windows Firewall Log Collector (ID: 54)**

<figure><img src="../.gitbook/assets/image (892).png" alt=""><figcaption></figcaption></figure>

If Windows Firewall Log collector is enabled, VirtualMetric uses Windows Firewall Log file or Security Audit events to collect Windows Firewall activities. VirtualMetric collects following events of Windows Defender:

**Windows Firewall Settings**

<div align="left">

<figure><img src="../.gitbook/assets/image (893).png" alt="" width="455"><figcaption></figcaption></figure>

</div>

With default settings, VirtualMetric collects firewall logs via Windows Firewall log file.

```markup
mode=file
```

If you want to enable file logging on Windows Firewall, go to Windows Firewall for configuration.

Right click on Windows Firewall title, and click Properties.

<div align="left">

<figure><img src="../.gitbook/assets/image (894).png" alt="" width="512"><figcaption></figcaption></figure>

</div>

Click on Customize for logging properties.

<div align="left">

<figure><img src="../.gitbook/assets/image (895).png" alt=""><figcaption></figcaption></figure>

</div>

Choose Yes for logging dropped packets. You can also enable logging of successful connections if you need it.

<div align="left">

<figure><img src="../.gitbook/assets/image (896).png" alt=""><figcaption></figcaption></figure>

</div>

After these changes, VirtualMetric will start reading Windows Firewall log file via Inventory Collector. You can also switch collector mode to "Event" for real time collection. Go to collector definition settings and change mode to Event:

```markup
mode=event
```

To activate event logging for Windows Firewall, you should make changes on Local Group Policy settings.

Open Local Group Policy and go to Windows Settings -> Security Settings -> Local Policies -> Audit Policy.

<div align="left">

<figure><img src="../.gitbook/assets/image (897).png" alt="" width="563"><figcaption></figcaption></figure>

</div>

Make sure that Success and Failure events are selected.

<div align="left">

<figure><img src="../.gitbook/assets/image (898).png" alt="" width="563"><figcaption></figcaption></figure>

</div>

VirtualMetric collects following events of Windows Firewall:

**Filtering Platform Connection - Permitted (ID: 88)**

<figure><img src="../.gitbook/assets/image (899).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="283">Group</th><th width="95.33333333333331">Event ID</th><th>Message</th></tr></thead><tbody><tr><td>Filtering Platform Connection: Permitted</td><td>5154</td><td>The Windows Filtering Platform has permitted an application or service to listen on a port for incoming connections.</td></tr><tr><td>Filtering Platform Connection: Permitted</td><td>5156</td><td>The Windows Filtering Platform has permitted a connection.</td></tr><tr><td>Filtering Platform Connection: Permitted</td><td>5158</td><td>The Windows Filtering Platform has permitted a bind to a local port.</td></tr></tbody></table>

**Filtering Platform Packet Drop (ID: 92)**

<div align="left">

<figure><img src="../.gitbook/assets/image (900).png" alt=""><figcaption></figcaption></figure>

</div>

<table><thead><tr><th width="289">Group</th><th width="128.33333333333331">Event ID</th><th>Message</th></tr></thead><tbody><tr><td>Filtering Platform Packet Drop</td><td>5152</td><td>The Windows Filtering Platform blocked a packet.</td></tr><tr><td>Filtering Platform Packet Drop</td><td>5153</td><td>A more restrictive Windows Filtering Platform filter has blocked a packet.</td></tr></tbody></table>

**DDoS Analyzer (ID: 94)**

<div align="left">

<figure><img src="../.gitbook/assets/image (901).png" alt=""><figcaption></figcaption></figure>

</div>

<table><thead><tr><th width="205.33333333333331">Group</th><th width="132">Event ID</th><th>Message</th></tr></thead><tbody><tr><td>DDoS Analyzer</td><td>5148</td><td>The Windows Filtering Platform has detected a DoS attack and entered a defensive mode; packets associated with this attack will be discarded.</td></tr><tr><td>DDoS Analyzer</td><td>5149</td><td>The DoS attack has subsided and normal processing is being resumed.</td></tr></tbody></table>

\
Please make sure that these Event Log definitions are also enabled. You can always customize these settings to filter Windows Firewall events.

## Object Access

In order to enable Object Access Auditing reports, please make sure that Collector ID: 144 is enabled.\


**Windows Object Access Audit Collector (ID: 144)**

<figure><img src="../.gitbook/assets/image (903).png" alt=""><figcaption></figcaption></figure>

To activate event logging for Object Access Auditing, you should make changes on Local Group Policy settings.

Open Local Group Policy and go to Windows Settings -> Security Settings -> Local Policies -> Audit Policy.

<div align="left">

<figure><img src="../.gitbook/assets/image (904).png" alt="" width="563"><figcaption></figcaption></figure>

</div>

Make sure that Success and Failure events are selected.

<div align="left">

<figure><img src="../.gitbook/assets/image (905).png" alt="" width="563"><figcaption></figcaption></figure>

</div>

For test purposes, go to Properties of the sensitive file.

<div align="left">

<figure><img src="../.gitbook/assets/image (906).png" alt="" width="449"><figcaption></figcaption></figure>

</div>

Switch to Security tab and click on Advanced button.

<div align="left">

<figure><img src="../.gitbook/assets/image (907).png" alt="" width="434"><figcaption></figcaption></figure>

</div>

Switch to Auditing tab and click on Add button.

<div align="left">

<figure><img src="../.gitbook/assets/image (908).png" alt="" width="563"><figcaption></figcaption></figure>

</div>

Click on Select a principal and type Everyone and click OK button.

<div align="left">

<figure><img src="../.gitbook/assets/image (909).png" alt="" width="563"><figcaption></figcaption></figure>

</div>

Select All for type, and switch Advanced Mode. Select the events for logging and click OK button.

<div align="left">

<figure><img src="../.gitbook/assets/image (911).png" alt="" width="563"><figcaption></figcaption></figure>

</div>

Click Apply and click OK button to save changes.

<div align="left">

<figure><img src="../.gitbook/assets/image (910).png" alt="" width="563"><figcaption></figcaption></figure>

</div>

VirtualMetric collects following events of Object Access Auditing:

**Object Access Auditing (ID: 95)**

<div align="left">

<figure><img src="../.gitbook/assets/image (912).png" alt=""><figcaption></figcaption></figure>

</div>

**Object Access Auditing (ID: 96)**

<div align="left">

<figure><img src="../.gitbook/assets/image (913).png" alt=""><figcaption></figcaption></figure>

</div>

<table><thead><tr><th width="224">Group</th><th width="138.33333333333331">Event ID</th><th>Message</th></tr></thead><tbody><tr><td>Object Access Auditing</td><td>4656 / 560</td><td>A handle to an object was requested.</td></tr><tr><td>Object Access Auditing</td><td>4658 / 562</td><td>The handle to an object was closed.</td></tr><tr><td>Object Access Auditing</td><td>4659 / 563</td><td>A handle to an object was requested with intent to delete.</td></tr><tr><td>Object Access Auditing</td><td>4660 / 564</td><td>An object was deleted.</td></tr><tr><td>Object Access Auditing</td><td>4661 / 565</td><td>A handle to an object was requested.</td></tr><tr><td>Object Access Auditing</td><td>4662 / 566</td><td>An operation was performed on an object.</td></tr><tr><td>Object Access Auditing</td><td>4663 / 567</td><td>An attempt was made to access an object.</td></tr><tr><td>Object Access Auditing</td><td>4664 / 568</td><td>An attempt was made to create a hard link.</td></tr></tbody></table>

\
Please make sure that these Event Log definitions are also enabled. You can always customize these settings to filter Object Access events. You can log following audit types via VirtualMetric:\
\


<table><thead><tr><th width="221">Access Type</th><th width="126.33333333333331" align="center">Enabled?</th><th>Description</th></tr></thead><tbody><tr><td>ReadData</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>The right to read the corresponding file data.</td></tr><tr><td>ListDirectory</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>The right to list the contents of the directory.</td></tr><tr><td>WriteData</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>The right to write data to the file.</td></tr><tr><td>AddFile</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>The right to create a file in the directory.</td></tr><tr><td>AppendData</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>The right to append data to the file.</td></tr><tr><td>AddSubdirectory</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>The right to create a subdirectory.</td></tr><tr><td>ReadEA</td><td align="center"><mark style="color:red;">✖︎</mark></td><td>The right to read extended file attributes.</td></tr><tr><td>WriteEA</td><td align="center"><mark style="color:red;">✖︎</mark></td><td>The right to write extended file attributes.</td></tr><tr><td>Execute</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>The right to execute the file.</td></tr><tr><td>Traverse</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>The right to traverse the directory.</td></tr><tr><td>DeleteChild</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>The right to delete a directory and all the files it contains, including read-only files.</td></tr><tr><td>ReadAttributes</td><td align="center"><mark style="color:red;">✖︎</mark></td><td>The right to read file attributes.</td></tr><tr><td>WriteAttributes</td><td align="center"><mark style="color:red;">✖︎</mark></td><td>The right to write file attributes.</td></tr><tr><td>ReadMemory</td><td align="center"><mark style="color:red;">✖︎</mark></td><td>The right to read process memory.</td></tr><tr><td>DELETE</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>The right to delete the object.</td></tr><tr><td>READ_CONTROL</td><td align="center"><mark style="color:red;">✖︎</mark></td><td>The right to read the information in the object's security descriptor, not including the information in the system access control list (SACL).</td></tr><tr><td>WRITE_DAC</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>The right to modify the discretionary access control list (DACL) in the object's security descriptor.</td></tr><tr><td>WRITE_OWNER</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>The right to change the owner in the object's security descriptor.</td></tr><tr><td>SYNCHRONIZE</td><td align="center"><mark style="color:red;">✖︎</mark></td><td>The right to use the object for synchronization. This enables a thread to wait until the object is in the signaled state. Some object types do not support this access right.</td></tr><tr><td>ACCESS_SYS_SEC</td><td align="center"><mark style="color:red;">✖︎</mark></td><td>The ACCESS_SYS_SEC access right controls the ability to get or set the SACL in an object's security descriptor.</td></tr></tbody></table>

With default settings, VirtualMetric uses following audit types in collector settings:

{% code overflow="wrap" lineNumbers="true" %}
```markup
accessmode=ReadData,ListDirectory,WriteData,WRITE_DAC,WRITE_OWNER,AddFile,AppendData,AddSubdirectory,Execute,Traverse,DeleteChild,DELETE
```
{% endcode %}

If you want to enable extra access types, you can modify collector settings.

After modifying `accessmode` options, you can click Submit button to apply changes.

<div align="left">

<figure><img src="../.gitbook/assets/image (914).png" alt="" width="455"><figcaption></figcaption></figure>

</div>

## File Change Tracking

In order to enable Windows File Change Tracking reports, please make sure that Collector ID: 139 is enabled.\
**Windows File Change Tracking Collector (ID: 139)**

<div align="left">

<figure><img src="../.gitbook/assets/image (915).png" alt=""><figcaption></figcaption></figure>

</div>

By default, VirtualMetric uses following white list and black list to filter file changes:

```markup
extensionWhiteList=.ps1,.vbs,.exe&extensionBlackList=.log,.evtx
```

If you clear these settings, VirtualMetric logs all file changes. You can use `extensionBlackList` to filter some file extensions like .log or .evtx etc. You can also add some file type extensions to always log via `extensionWhiteList` setting. If you want to set these lists, you can modify collector settings.

<div align="left">

<figure><img src="../.gitbook/assets/image (916).png" alt="" width="452"><figcaption></figcaption></figure>

</div>

After modifying options, you can click Submit button to apply changes.
