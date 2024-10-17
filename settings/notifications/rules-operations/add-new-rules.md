# Add new Rules

Before adding new Rule, you should create a new Rule entry.

1\.      Click to **Rules** on the left pane.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (627).png" alt=""><figcaption></figcaption></figure>

</div>

2\.      On **Rules Management** screen, click **Add (+)** button on the right top section.

<figure><img src="../../../.gitbook/assets/image (628).png" alt=""><figcaption></figcaption></figure>

3\.      Select type of Rule.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (630).png" alt="" width="288"><figcaption></figcaption></figure>

</div>

4\.      Fields will change based on type.

## <mark style="color:red;">Type: Inventory</mark>

_Refer to the following table to understand the fields of **inventory type** in the above screen._&#x20;

<table><thead><tr><th width="218">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a Rule. </td></tr><tr><td>Severity</td><td><p>Select a proper severity.</p><p>·       <strong>Critical</strong></p><p>·       <strong>High</strong></p><p>·       <strong>Medium</strong></p><p>·       <strong>Low</strong></p></td></tr><tr><td>Groups</td><td>This field is <strong>Global</strong> by default. It cannot be changed. </td></tr><tr><td>Modules</td><td>Select a proper module from dropdown.</td></tr><tr><td>Parent Group</td><td>Select a proper parent group from dropdown.</td></tr><tr><td>Filter</td><td><p>Condition of the rule will be defined in this field.</p><p></p><p>Select a proper field and condition. <strong>And/or</strong> statements <strong>Add Rule/Add Group</strong> statement can be added.</p><p><img src="../../../.gitbook/assets/image (631).png" alt=""></p></td></tr><tr><td>Trigger</td><td><p>Select a proper trigger from dropdown. </p><p>·       When condition occurs </p><p>·       If the condition returns no result </p><p>·       If the condition returns x or more results</p></td></tr></tbody></table>

### <mark style="color:blue;">Trigger: When condition occurs</mark>

<div align="left">

<figure><img src="../../../.gitbook/assets/image (637).png" alt="" width="278"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields of **trigger** in the above screen._&#x20;

<table><thead><tr><th width="200">Fields</th><th>Description</th></tr></thead><tbody><tr><td>State Changes </td><td><p>Select a proper option from dropdown. </p><p>·       <strong>Ignore state change:</strong> If selected column is changed don't notify</p><p>·       <strong>Notify on state change:</strong> If selected column is changed notify</p></td></tr><tr><td>State Column</td><td>Select a proper state column from dropdown.</td></tr><tr><td>Set a reminder for every...</td><td><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not resolved</strong> notify every selected <strong>time range</strong>. </p></td></tr><tr><td>Resolve Condition</td><td><p>Select a proper module from dropdown.</p><p>·       If the rule does not match the condition.</p><p>·       If the rule match the custom condition. Create a resolve condition.</p><p><img src="../../../.gitbook/assets/image (634).png" alt=""> </p></td></tr></tbody></table>

###

### <mark style="color:blue;">Trigger: If the condition return no results</mark>

<div align="left">

<figure><img src="../../../.gitbook/assets/image (636).png" alt="" width="274"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields of **trigger** in the above screen._&#x20;

<table><thead><tr><th width="200">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Set a reminder for every...</td><td><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not resolved</strong> notify every selected <strong>time range</strong>. </p></td></tr><tr><td>Resolve Condition</td><td><p>Select a proper module from dropdown.</p><p>·       If the rule does not match the condition.</p><p>·       If the rule match the custom condition. Create a resolve condition.</p><p><img src="../../../.gitbook/assets/image (634).png" alt=""> </p></td></tr></tbody></table>

### <mark style="color:blue;">Trigger: If the condition returns x or more results</mark>

<div align="left">

<figure><img src="../../../.gitbook/assets/image (638).png" alt="" width="286"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields of **trigger** in the above screen._&#x20;

<table><thead><tr><th width="200">Fields</th><th>Description</th></tr></thead><tbody><tr><td>State Changes </td><td><p>Select a proper option from dropdown. </p><p>·       <strong>Ignore state change:</strong> If selected column is changed don't notify</p><p>·       <strong>Notify on state change:</strong> If selected column is changed notify</p></td></tr><tr><td>State Column</td><td>Select a proper state column from dropdown.</td></tr><tr><td>Set a reminder for every...</td><td><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not resolved</strong> notify every selected <strong>time range</strong>. </p></td></tr><tr><td>Aggregation</td><td><p>Select a proper state column from dropdown</p><p>·       <strong>Last</strong></p><p>·       <strong>First</strong></p></td></tr><tr><td>Event Count</td><td>Set the count of repetitions before the rule activeness. </td></tr><tr><td>Resolve Condition</td><td><p>Select a proper module from dropdown.</p><p>·       If the rule does not match the condition.</p><p>·       If the rule match the custom condition. Create a resolve condition.</p><p><img src="../../../.gitbook/assets/image (634).png" alt=""> </p></td></tr></tbody></table>

## <mark style="color:red;">Type: Counter</mark>

Counter type mostly using for combining different types of condition.

_Refer to the following table to understand the fields of **counter type** in the above screen._&#x20;

<table><thead><tr><th width="218">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a Rule. </td></tr><tr><td>Severity</td><td><p>Select a proper severity.</p><p>·       <strong>Critical</strong></p><p>·       <strong>High</strong></p><p>·       <strong>Medium</strong></p><p>·       <strong>Low</strong></p></td></tr><tr><td>Groups</td><td>Select a proper groups from dropdown.</td></tr><tr><td>Modules</td><td>This field is <strong>All</strong> by default. It cannot be changed. </td></tr><tr><td>Parent Group</td><td>Select a proper parent group from dropdown.</td></tr><tr><td>Filter</td><td><p>Condition of the rule will be defined in this field.</p><p></p><p>Select a proper field and condition. <strong>And/or</strong> statements <strong>Add Rule/Add Group</strong> statement can be added. Firstly, counter must be selected (1), then value must be assigned (2)</p><p><img src="../../../.gitbook/assets/image (640).png" alt="" data-size="original"></p><p></p></td></tr><tr><td>Trigger</td><td><p>Select a proper trigger from dropdown. </p><p>·       When condition occurs </p><p>·       If the condition persists for</p><p>·       If the condition returns no results</p><p></p></td></tr></tbody></table>

### <mark style="color:blue;">Trigger: When condition occurs</mark>

<div align="left">

<figure><img src="../../../.gitbook/assets/image (641).png" alt="" width="278"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields of **trigger** in the above screen._&#x20;

<table><thead><tr><th width="203">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Set a reminder for every...</td><td><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not resolved</strong> notify every selected <strong>time range</strong>. </p></td></tr><tr><td>Notification Delivery</td><td><p>Select a proper option from dropdown. </p><p>·       <strong>Per count</strong></p><p>·       <strong>Per Incident</strong></p></td></tr><tr><td>Fix Count</td><td><p>If you want to avoid from too many down/resolved notifications, you can use fix count. If notification rule item is down, you can use fix count option to ignore X times of healthier samples. For example:</p><p>·       If fix count is 0, <mark style="color:red;">down down</mark> <mark style="color:green;">up</mark> <mark style="color:red;">down down down</mark> <mark style="color:green;">up</mark> -> <strong>will set status as resolved</strong> for first and second up. </p><p>·       If fix count is 1, <mark style="color:red;">down down</mark> <mark style="color:green;">up</mark> <mark style="color:red;">down down</mark> <mark style="color:green;">up</mark> <mark style="color:red;">down</mark> <strong>-> will not set any resolved</strong>. </p><p>·       If fix count is 1, <mark style="color:red;">down down</mark> <mark style="color:green;">up up</mark> <mark style="color:red;">down down</mark> <mark style="color:green;">up</mark> <mark style="color:red;">down</mark> -> <strong>will set resolved</strong> for <mark style="color:green;">up up</mark>, but not for <mark style="color:red;">down</mark> <mark style="color:green;">up</mark> <mark style="color:red;">down</mark>. </p></td></tr><tr><td>When counter matches with the condition, use..</td><td><p>This field is active when <strong>notification delivery is Per Count</strong>, Select a proper option from dropdown. </p><p>·       If defined, use Counter Threshold, otherwise use Rule Severity</p><p>·       Counter Threshold</p><p>·       Rule Severity</p></td></tr><tr><td>Resolve Condition</td><td><p>Select a proper module from dropdown.</p><p>·       If the rule does not match the condition.</p><p>·       If the rule match the custom condition. Create a resolve condition.</p><p><img src="../../../.gitbook/assets/image (634).png" alt=""> </p></td></tr></tbody></table>

###

### Trigger: If the condition persist for

<div align="left">

<figure><img src="../../../.gitbook/assets/image (642).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields of **trigger** in the above screen._&#x20;

<table><thead><tr><th width="203">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Time frame</td><td>Select a proper time frame</td></tr><tr><td>Set a reminder for every...</td><td><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not resolved</strong> notify every selected <strong>time range</strong>. </p></td></tr><tr><td>Notification Delivery</td><td><p>Select a proper option from dropdown. </p><p>·       <strong>Per count</strong></p><p>·       <strong>Per Incident</strong></p></td></tr><tr><td>Fix Count</td><td><p>If you want to avoid from too many down/resolved notifications, you can use fix count. If notification rule item is down, you can use fix count option to ignore X times of healthier samples. For example:</p><p>·       If fix count is 0, <mark style="color:red;">down down</mark> <mark style="color:green;">up</mark> <mark style="color:red;">down down down</mark> <mark style="color:green;">up</mark> -> <strong>will set status as resolved</strong> for first and second up. </p><p>·       If fix count is 1, <mark style="color:red;">down down</mark> <mark style="color:green;">up</mark> <mark style="color:red;">down down</mark> <mark style="color:green;">up</mark> <mark style="color:red;">down</mark> <strong>-> will not set any resolved</strong>. </p><p>·       If fix count is 1, <mark style="color:red;">down down</mark> <mark style="color:green;">up up</mark> <mark style="color:red;">down down</mark> <mark style="color:green;">up</mark> <mark style="color:red;">down</mark> -> <strong>will set resolved</strong> for <mark style="color:green;">up up</mark>, but not for <mark style="color:red;">down</mark> <mark style="color:green;">up</mark> <mark style="color:red;">down</mark>. </p></td></tr><tr><td>When counter matches with the condition, use..</td><td><p>This field is active when <strong>notification delivery is Per Count</strong>, Select a proper option from dropdown. </p><p>·       If defined, use Counter Threshold, otherwise use Rule Severity</p><p>·       Counter Threshold</p><p>·       Rule Severity</p></td></tr><tr><td>Resolve Condition</td><td><p>Select a proper module from dropdown.</p><p>·       If the rule does not match the condition.</p><p>·       If the rule match the custom condition. Create a resolve condition.</p><p><img src="../../../.gitbook/assets/image (634).png" alt=""> </p></td></tr></tbody></table>

### <mark style="color:blue;">Trigger: If the condition returns no results</mark>

<div align="left">

<figure><img src="../../../.gitbook/assets/image (652).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields of **trigger** in the above screen._&#x20;

<table><thead><tr><th width="200">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Set a reminder for every...</td><td><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not resolved</strong> notify every selected <strong>time range</strong>. </p></td></tr><tr><td>Resolve Condition</td><td><p>Select a proper module from dropdown.</p><p>·       If the rule does not match the condition.</p><p>·       If the rule match the custom condition. Create a resolve condition.</p><p><img src="../../../.gitbook/assets/image (634).png" alt=""> </p></td></tr></tbody></table>

## <mark style="color:red;">Type: Analytics</mark>

Analytics type mostly using for creating log condition.

_Refer to the following table to understand the fields of **counter type** in the above screen._&#x20;

<table><thead><tr><th width="218">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a Rule. </td></tr><tr><td>Severity</td><td><p>Select a proper severity.</p><p>·       <strong>Critical</strong></p><p>·       <strong>High</strong></p><p>·       <strong>Medium</strong></p><p>·       <strong>Low</strong></p></td></tr><tr><td>Groups</td><td>This field is <strong>Global</strong> by default. It cannot be changed. </td></tr><tr><td>Definitions</td><td>Select a proper definitions from dropdown.</td></tr><tr><td>Parent Group</td><td>Select a proper parent group from dropdown.</td></tr><tr><td>Filter</td><td><p>Condition of the rule will be defined in this field.</p><p></p><p>Select a proper field and condition. <strong>And/or</strong> statements <strong>Add Rule/Add Group</strong> statement can be added.</p><p><img src="../../../.gitbook/assets/image (643).png" alt="" data-size="original"></p><p></p></td></tr><tr><td>Trigger</td><td><p>Select a proper trigger from dropdown. </p><p>·       When condition occurs </p><p>·       If the condition occurs x or more in the last</p><p>·       If the condition returns no results in the last</p><p></p></td></tr></tbody></table>

### <mark style="color:blue;">Trigger: When condition occurs</mark>

<div align="left">

<figure><img src="../../../.gitbook/assets/image (644).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields of **trigger** in the above screen._&#x20;

<table><thead><tr><th width="203">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Resolve the issue if there no event for </td><td><p>This field only active when resolve condition is <strong>if the rule remains active for the specified period of time</strong>.</p><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not matching for selected time period then resolve the event</strong> </p></td></tr><tr><td>When a new event arrives</td><td><p>This field only active when resolve condition is <strong>if the rule remains active for the specified period of time</strong>.</p><p>Select a proper option from dropdown. </p><p>·       <strong>Do not notify</strong></p><p>·       <strong>Notify</strong></p></td></tr><tr><td>Resolve Condition</td><td><p>Select a proper module from dropdown.</p><p>·       If the rule remains active for the specified period of time.</p><p>·       If the rule match the custom condition. Create a resolve condition.</p><p><img src="../../../.gitbook/assets/image (634).png" alt=""> </p></td></tr></tbody></table>

###

### <mark style="color:blue;">Trigger: If the condition occurs x times or more in the last</mark>

<div align="left">

<figure><img src="../../../.gitbook/assets/image (647).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields of **trigger** in the above screen._&#x20;

<table><thead><tr><th width="203">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Time frame</td><td>Select a proper time frame</td></tr><tr><td>Set a reminder for every...</td><td><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not resolved</strong> notify every selected <strong>time range</strong>. </p></td></tr><tr><td>Event Count</td><td>Set the count of repetitions before the rule activeness. </td></tr><tr><td>Aggregation</td><td><p>Select a proper state column from dropdown</p><p>·       <strong>Last</strong></p><p>·       <strong>First</strong></p></td></tr><tr><td>Resolve the issue if there no event for </td><td><p>This field only active when resolve condition is <strong>if the rule remains active for the specified period of time</strong>.</p><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not matching for selected time period then resolve the event</strong> </p></td></tr><tr><td>When a new event arrives</td><td><p>This field only active when resolve condition is <strong>if the rule remains active for the specified period of time</strong>.</p><p>Select a proper option from dropdown. </p><p>·       <strong>Do not notify</strong></p><p>·       <strong>Notify</strong></p></td></tr><tr><td>Resolve Condition</td><td><p>Select a proper module from dropdown.</p><p>·       If the rule remains active for the specified period of time.</p><p>·       If the rule match the custom condition. Create a resolve condition.</p><p><img src="../../../.gitbook/assets/image (634).png" alt=""> </p></td></tr></tbody></table>

### <mark style="color:blue;">Trigger: If the condition returns no results in last</mark>

<div align="left">

<figure><img src="../../../.gitbook/assets/image (645).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields of **trigger** in the above screen._&#x20;

<table><thead><tr><th width="203">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Time frame</td><td>Select a proper time frame</td></tr><tr><td>Set a reminder for every...</td><td><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not resolved</strong> notify every selected <strong>time range</strong>. </p></td></tr><tr><td>Resolve the issue if there no event for </td><td><p>This field only active when resolve condition is <strong>if the rule remains active for the specified period of time</strong>.</p><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not matching for selected time period then resolve the event</strong> </p></td></tr><tr><td>When a new event arrives</td><td><p>This field only active when resolve condition is <strong>if the rule remains active for the specified period of time</strong>.</p><p>Select a proper option from dropdown. </p><p>·       <strong>Do not notify</strong></p><p>·       <strong>Notify</strong></p></td></tr><tr><td>Resolve Condition</td><td><p>Select a proper module from dropdown.</p><p>·       If the rule remains active for the specified period of time.</p><p>·       If the rule match the custom condition. Create a resolve condition.</p><p><img src="../../../.gitbook/assets/image (634).png" alt=""> </p></td></tr></tbody></table>

## <mark style="color:red;">Type: SQL Content</mark>

SQL Content type mostly using for creating conditions by query.

_Refer to the following table to understand the fields of **counter type** in the above screen._&#x20;

<table><thead><tr><th width="218">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a Rule. </td></tr><tr><td>Severity</td><td><p>Select a proper severity.</p><p>·       <strong>Critical</strong></p><p>·       <strong>High</strong></p><p>·       <strong>Medium</strong></p><p>·       <strong>Low</strong></p></td></tr><tr><td>Groups</td><td>This field is <strong>Global</strong> by default. It cannot be changed. </td></tr><tr><td>Definitions</td><td>Select a proper definitions from dropdown.</td></tr><tr><td>Parent Group</td><td>Select a proper parent group from dropdown.</td></tr><tr><td>Query</td><td><p>Write your condition by query</p><p><img src="../../../.gitbook/assets/image (646).png" alt="" data-size="original"></p><p></p></td></tr><tr><td>Trigger</td><td><p>Select a proper trigger from dropdown. </p><p>·       When condition occurs </p><p>·       If the condition occurs x or more in the last</p><p>·       If the condition returns no results in the last</p><p></p></td></tr></tbody></table>

### <mark style="color:blue;">Trigger: When condition occurs</mark>

<div align="left">

<figure><img src="../../../.gitbook/assets/image (644).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields of **trigger** in the above screen._&#x20;

<table><thead><tr><th width="203">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Resolve the issue if there no event for </td><td><p>This field only active when resolve condition is <strong>if the rule remains active for the specified period of time</strong>.</p><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not matching for selected time period then resolve the event</strong> </p></td></tr><tr><td>When a new event arrives</td><td><p>This field only active when resolve condition is <strong>if the rule remains active for the specified period of time</strong>.</p><p>Select a proper option from dropdown. </p><p>·       <strong>Do not notify</strong></p><p>·       <strong>Notify</strong></p></td></tr><tr><td>Resolve Condition</td><td><p>Select a proper module from dropdown.</p><p>·       If the rule remains active for the specified period of time.</p><p>·       If the rule match the custom condition. Create a resolve condition.</p><p><img src="../../../.gitbook/assets/image (634).png" alt=""> </p></td></tr></tbody></table>

###

### <mark style="color:blue;">Trigger: If the condition occurs x times or more in the last</mark>

<div align="left">

<figure><img src="../../../.gitbook/assets/image (648).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields of **trigger** in the above screen._&#x20;

<table><thead><tr><th width="203">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Time frame</td><td>Select a proper time frame</td></tr><tr><td>Set a reminder for every...</td><td><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not resolved</strong> notify every selected <strong>time range</strong>. </p></td></tr><tr><td>Event Count</td><td>Set the count of repetitions before the rule activeness. </td></tr><tr><td>Aggregation</td><td><p>Select a proper state column from dropdown</p><p>·       <strong>Last</strong></p><p>·       <strong>First</strong></p></td></tr><tr><td>Resolve the issue if there no event for </td><td><p>This field only active when resolve condition is <strong>if the rule remains active for the specified period of time</strong>.</p><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not matching for selected time period then resolve the event</strong> </p></td></tr><tr><td>When a new event arrives</td><td><p>This field only active when resolve condition is <strong>if the rule remains active for the specified period of time</strong>.</p><p>Select a proper option from dropdown. </p><p>·       <strong>Do not notify</strong></p><p>·       <strong>Notify</strong></p></td></tr><tr><td>Resolve Condition</td><td><p>Select a proper module from dropdown.</p><p>·       If the rule remains active for the specified period of time.</p><p>·       If the rule match the custom condition. Create a resolve condition.</p><p><img src="../../../.gitbook/assets/image (634).png" alt=""> </p></td></tr></tbody></table>

### <mark style="color:blue;">Trigger: If the condition returns no results</mark>

<div align="left">

<figure><img src="../../../.gitbook/assets/image (649).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields of **trigger** in the above screen._&#x20;

<table><thead><tr><th width="203">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Time frame</td><td>Select a proper time frame</td></tr><tr><td>Set a reminder for every...</td><td><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not resolved</strong> notify every selected <strong>time range</strong>. </p></td></tr><tr><td>Resolve the issue if there no event for </td><td><p>This field only active when resolve condition is <strong>if the rule remains active for the specified period of time</strong>.</p><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not matching for selected time period then resolve the event</strong> </p></td></tr><tr><td>When a new event arrives</td><td><p>This field only active when resolve condition is <strong>if the rule remains active for the specified period of time</strong>.</p><p>Select a proper option from dropdown. </p><p>·       <strong>Do not notify</strong></p><p>·       <strong>Notify</strong></p></td></tr><tr><td>Resolve Condition</td><td><p>Select a proper module from dropdown.</p><p>·       If the rule remains active for the specified period of time.</p><p>·       If the rule match the custom condition. Create a resolve condition.</p><p><img src="../../../.gitbook/assets/image (651).png" alt="" data-size="original"></p></td></tr></tbody></table>

## <mark style="color:red;">Type: System</mark>

SQL Content type mostly using for creating conditions by query.

_Refer to the following table to understand the fields of **counter type** in the above screen._&#x20;

<table><thead><tr><th width="218">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Name </td><td>A label or name that is assigned to a Rule. </td></tr><tr><td>Severity</td><td><p>Select a proper severity.</p><p>·       <strong>Critical</strong></p><p>·       <strong>High</strong></p><p>·       <strong>Medium</strong></p><p>·       <strong>Low</strong></p></td></tr><tr><td>Groups</td><td>This field is <strong>Global</strong> by default. It cannot be changed. </td></tr><tr><td>Definitions</td><td>Select a proper definitions from dropdown.</td></tr><tr><td>Parent Group</td><td>Select a proper parent group from dropdown.</td></tr><tr><td>Query</td><td><p>Condition of the rule will be defined in this field.</p><p></p><p>Select a proper field and condition. <strong>And/or</strong> statements <strong>Add Rule/Add Group</strong> statement can be added. </p><p><img src="../../../.gitbook/assets/image (653).png" alt="" data-size="original"></p><p></p></td></tr><tr><td>Trigger</td><td><p>Select a proper trigger from dropdown. </p><p>·       When condition occurs </p><p>·       If the condition occurs x or more in the last</p><p>·       If the condition returns no results in the last</p><p></p></td></tr></tbody></table>

### <mark style="color:blue;">Trigger: When condition occurs</mark>

<div align="left">

<figure><img src="../../../.gitbook/assets/image (644).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields of **trigger** in the above screen._&#x20;

<table><thead><tr><th width="203">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Resolve the issue if there no event for </td><td><p>This field only active when resolve condition is <strong>if the rule remains active for the specified period of time</strong>.</p><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not matching for selected time period then resolve the event</strong> </p></td></tr><tr><td>When a new event arrives</td><td><p>This field only active when resolve condition is <strong>if the rule remains active for the specified period of time</strong>.</p><p>Select a proper option from dropdown. </p><p>·       <strong>Do not notify</strong></p><p>·       <strong>Notify</strong></p></td></tr><tr><td>Resolve Condition</td><td><p>Select a proper module from dropdown.</p><p>·       If the rule remains active for the specified period of time.</p><p>·       If the rule match the custom condition. Create a resolve condition.</p><p><img src="../../../.gitbook/assets/image (634).png" alt=""> </p></td></tr></tbody></table>

###

### <mark style="color:blue;">Trigger: If the condition occurs x times or more in the last</mark>

<div align="left">

<figure><img src="../../../.gitbook/assets/image (648).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields of **trigger** in the above screen._&#x20;

<table><thead><tr><th width="203">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Time frame</td><td>Select a proper time frame</td></tr><tr><td>Set a reminder for every...</td><td><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not resolved</strong> notify every selected <strong>time range</strong>. </p></td></tr><tr><td>Event Count</td><td>Set the count of repetitions before the rule activeness. </td></tr><tr><td>Aggregation</td><td><p>Select a proper state column from dropdown</p><p>·       <strong>Last</strong></p><p>·       <strong>First</strong></p></td></tr><tr><td>Resolve the issue if there no event for </td><td><p>This field only active when resolve condition is <strong>if the rule remains active for the specified period of time</strong>.</p><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not matching for selected time period then resolve the event</strong> </p></td></tr><tr><td>When a new event arrives</td><td><p>This field only active when resolve condition is <strong>if the rule remains active for the specified period of time</strong>.</p><p>Select a proper option from dropdown. </p><p>·       <strong>Do not notify</strong></p><p>·       <strong>Notify</strong></p></td></tr><tr><td>Resolve Condition</td><td><p>Select a proper module from dropdown.</p><p>·       If the rule remains active for the specified period of time.</p><p>·       If the rule match the custom condition. Create a resolve condition.</p><p><img src="../../../.gitbook/assets/image (634).png" alt=""> </p></td></tr></tbody></table>

### <mark style="color:blue;">Trigger: If the condition returns no results</mark>

<div align="left">

<figure><img src="../../../.gitbook/assets/image (649).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields of **trigger** in the above screen._&#x20;

<table><thead><tr><th width="203">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Time frame</td><td>Select a proper time frame</td></tr><tr><td>Set a reminder for every...</td><td><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not resolved</strong> notify every selected <strong>time range</strong>. </p></td></tr><tr><td>Resolve the issue if there no event for </td><td><p>This field only active when resolve condition is <strong>if the rule remains active for the specified period of time</strong>.</p><p>Select a proper time option from dropdown. </p><p>If condition <strong>is not matching for selected time period then resolve the event</strong> </p></td></tr><tr><td>When a new event arrives</td><td><p>This field only active when resolve condition is <strong>if the rule remains active for the specified period of time</strong>.</p><p>Select a proper option from dropdown. </p><p>·       <strong>Do not notify</strong></p><p>·       <strong>Notify</strong></p></td></tr><tr><td>Resolve Condition</td><td><p>Select a proper module from dropdown.</p><p>·       If the rule remains active for the specified period of time.</p><p>·       If the rule match the custom condition. Create a resolve condition.</p><p><img src="../../../.gitbook/assets/image (654).png" alt="" data-size="original"></p></td></tr></tbody></table>

4\.      After creating the condition of the rule, additional informations and actions can be added from **advanced setting.** That way rule can be understood better.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (655).png" alt="" width="280"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields of **advanced settings** in the above screen._&#x20;

<table><thead><tr><th width="219">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Knowledge Base</td><td>Templete of additional information about rule. <strong>Knowledge Base can be created</strong> under <strong>Notifications</strong>.</td></tr><tr><td>Source</td><td>Select a proper source option from dropdown.</td></tr><tr><td>Affects</td><td>Select a proper affect option from dropdown. </td></tr><tr><td>Applies to</td><td>Select a proper applies to option from dropdown. </td></tr><tr><td>Urgency</td><td>Select a proper urgency option from dropdown. </td></tr><tr><td>Notifications</td><td>Select a proper notification rule option from dropdown. </td></tr><tr><td>Custom String</td><td>You can add custom string into the notification messages. If you are using an orchestration software, you can defines rules based on your custom string. Custom <strong>String is only available in the mail actions</strong>.</td></tr><tr><td>Template</td><td>Mail action template for the notification rule. If you want to do white labeling, you can change default template or add more templates. [In Development] Changing default mail template or adding more templates is currently <strong>not supported</strong> by VirtualMetric.</td></tr><tr><td>Custom Category</td><td>You can add custom category into the notification messages.</td></tr><tr><td>Custom Subcategory</td><td>You can add custom subcategory into the notification messages.</td></tr><tr><td>Enable Active Hours</td><td>You can set the timeperiod of notifications</td></tr><tr><td>Has Priority</td><td>Priority option for the notification rule. T<strong>his feature is only available for "Email" actions</strong>. If you enable it, you will receive emails with the "High Priority" mark.</td></tr><tr><td>Status</td><td>Rule can be enabled/disabled from status field.</td></tr></tbody></table>

5\.      After entering all the required info, click the button **SUBMIT**.
