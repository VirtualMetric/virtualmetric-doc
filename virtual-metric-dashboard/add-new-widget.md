# Add New Widget

VirtualMetric dashboard can be customized by adding different kind of widgets.

To add new widget, click on **Add Widget** button.

<figure><img src="../.gitbook/assets/image (864).png" alt=""><figcaption></figcaption></figure>

## Import Widget

Prepared widgets can be imported.

<div align="left">

<figure><img src="../.gitbook/assets/image (865).png" alt=""><figcaption></figcaption></figure>

</div>

* **Import API Query:** VirtualMetric is an API based application. Every component has an API. To see API of widget, you have to [expand widget](layout-and-common-functinalities.md#expand-widget). After getting the API, write API to query field.

<div align="left">

<figure><img src="../.gitbook/assets/image (867).png" alt="" width="299"><figcaption></figcaption></figure>

</div>

**Example:**&#x20;

{% code overflow="wrap" %}
```
https://devapi.virtualmetric.com/API/Query/Read?columns=inventory:host:name,counter:host:439,counter:host:172&groupBy=host&output=top&allowDBPaging=yes&orderDir=desc&topRows=10&rowsPerPage=10&title=Top+Memory+Usage&icon=fa+fa-memory&export=html&liveMode=3&legendposition=3&tooltipinteraction=0&access_token=***********************
```
{% endcode %}

* **Import Widget:** [Exported widget](layout-and-common-functinalities.md#export) can be imported to dashboard by adding content to request content.&#x20;

<div align="left">

<figure><img src="../.gitbook/assets/image (868).png" alt="" width="298"><figcaption></figcaption></figure>

</div>

**Example:**&#x20;

{% code overflow="wrap" %}
```json
{"IsSystem":false,"ModuleID":0,"LiveMode":1,"ChartType":3,"RecordStatus":1,"SqlQueryStatus":0,"TimeZone":20,"Forecast":-1,"TopRows":0,"DefinitionID":0,"Interval":-1,"RefID":0,"ID":0,"UseExternalAPI":false,"ChartProperties10":null,"ChartProperties09":null,"ChartProperties08":null,"ChartProperties07":null,"ChartProperties06":null,"ChartProperties05":null,"ChartProperties04":1,"ChartProperties03":1,"ChartProperties02":1,"ChartProperties01":1,"SqlQuery":null,"APIToken":null,"APIUser":null,"APIAddress":null,"Unit":"max","Aggregate":"no","OrderDir":"desc","OrderBy":"default","DrillDown":null,"FilterColumn":null,"Filter":null,"GroupBy":"object","ObjectFilter":"genericwebsite-8194","Columns":"inventory:genericwebsite:name,counter:genericwebsite:952","IconName":null,"LanguageKey":"website content","Name":"website content"}
```
{% endcode %}

* **Import Template:** VirtualMetric offers some prepared widgets which can be imported. Select **source, level** and **template** then click **submit**.

<div align="left">

<figure><img src="../.gitbook/assets/image (869).png" alt="" width="300"><figcaption></figcaption></figure>

</div>

## Add new Widget

VirtualMetric offers different kind of widgets.&#x20;

* **Empty widget:** You can create empty widget, select an icon and add a title. After adding the empty widget you have to [edit](edit-widget.md).&#x20;

<div align="left">

<figure><img src="../.gitbook/assets/image (870).png" alt="" width="298"><figcaption></figcaption></figure>

</div>

* **Notes:** Add your notes from notes widget. Fill the **notes** field.

<div align="left">

<figure><img src="../.gitbook/assets/image (871).png" alt="" width="299"><figcaption></figcaption></figure>

</div>

* **Clock:** To add clock widget, you must select mode (Analog and Dijital) and time zone.&#x20;

<div align="left">

<figure><img src="../.gitbook/assets/image (872).png" alt="" width="297"><figcaption></figcaption></figure>

</div>

* **Calendar:** To add calendar widget, you must select time zone.&#x20;

<div align="left">

<figure><img src="../.gitbook/assets/image (873).png" alt="" width="297"><figcaption></figcaption></figure>

</div>

* **Markdown:** Add your markdown expression to markdown field.

<div align="left">

<figure><img src="../.gitbook/assets/image (874).png" alt="" width="297"><figcaption></figcaption></figure>

</div>

* **Editor:** Add your expression to editor field. You can also write your notes in html format by clicking on **< >** (**view html)** option.&#x20;

<div align="left">

<figure><img src="../.gitbook/assets/image (875).png" alt="" width="297"><figcaption></figcaption></figure>

</div>

* **Video:** Youtube and Vimeo videos can be added to VirtualMetric Dashboard. It should be embed format.

<div align="left">

<figure><img src="../.gitbook/assets/image (876).png" alt="" width="298"><figcaption></figcaption></figure>

</div>

* **Title:** You can add title in dashboard.

<div align="left">

<figure><img src="../.gitbook/assets/image (877).png" alt="" width="296"><figcaption></figcaption></figure>

</div>

* **URL Address:** URL can be added to VirtualMetric Dashboard.

<div align="left">

<figure><img src="../.gitbook/assets/image (878).png" alt="" width="298"><figcaption></figcaption></figure>

</div>

* **Heatmap:** VirtualMetric offers a heatmap that shows general health of servers. You must select and size of icons. You can also filter the server.

<div align="left">

<figure><img src="../.gitbook/assets/image (879).png" alt="" width="295"><figcaption></figcaption></figure>

</div>

* **Realtime:** A line chart, that shows metrics in realtime, can be added in dashboard. By default it will show process load, but you can change it by [editing](edit-widget.md) the widget. &#x20;

<div align="left">

<figure><img src="../.gitbook/assets/image (880).png" alt="" width="296"><figcaption></figcaption></figure>

</div>

* **Alarms:** VirtualMetric alarms and alerts can be shown in dashboard. You can change display (table, charts etc.) of alarms and filter.

<div align="left">

<figure><img src="../.gitbook/assets/image (881).png" alt="" width="293"><figcaption></figcaption></figure>

</div>

* **Analytics:** Log table can be added to dashboard. You must add the log **query** to **SQL Content** field.

<div align="left">

<figure><img src="../.gitbook/assets/image (882).png" alt="" width="297"><figcaption></figcaption></figure>

</div>

* **Network Map:** Network Map can be added to dashboards. You can change display from below fields.&#x20;

<div align="left">

<figure><img src="../.gitbook/assets/image (883).png" alt="" width="296"><figcaption></figcaption></figure>

</div>

* **Network Path:** Network path can be shown at dashboard.

<div align="left">

<figure><img src="../.gitbook/assets/image (884).png" alt="" width="294"><figcaption></figcaption></figure>

</div>

**Example:**&#x20;

<figure><img src="../.gitbook/assets/image (885).png" alt=""><figcaption></figcaption></figure>
