# Bare Metal Hardware

VirtualMetric uses the management agents of manufacturers to monitor hardware health and to get hardware inventory. If management agent is not installed on the monitored server, then VirtualMetric uses [ IPMI](https://www.intel.com/content/www/us/en/servers/ipmi/ipmi-home.html) protocol and Microsoft Providers to get hardware health. You can find required management agents for supported manufacturers in this section.

## HP

VirtualMetric supports HP hardware to monitor hardware health and provide inventory information. Please check Model Coverage to see supported Models. Feature Coverage indicates supported feature sets for this manufacturer.

{% hint style="warning" %}
You need to install HP Insight Management Agents for Windows Server x64 Editions to monitor hardware health on Windows. Please download 9.6.0 or later versions.
{% endhint %}

**Model Coverage**

```markup
HP ProLiant BL460c Gen8 Server Blade
HP ProLiant BL460c Gen9 Server Blade
HP ProLiant BL465c Gen8 Server Blade
HP ProLiant BL660c Gen8 Server Blade
HP ProLiant BL660c Gen9 Server Blade
HP ProLiant BL685c Gen7 Server Blade
HP ProLiant DL120 Gen9
HP ProLiant DL160 Gen8
HP ProLiant DL160 Gen9
HP ProLiant DL180 Gen9
HP ProLiant DL320e Gen8 v2
HP ProLiant DL360 Gen9
HP ProLiant DL380e Gen8
HP ProLiant DL380 Gen9
HP ProLiant DL380p Gen8
HP ProLiant DL385p Gen8
HP ProLiant DL560 Gen8
HP ProLiant DL560 Gen9
HP ProLiant DL580 Gen7
HP ProLiant DL580 Gen8
HP ProLiant DL60 Gen9
HP ProLiant DL80 Gen9
HP ProLiant DL980 Gen7
HP ProLiant m300 Server Cartridge
HP ProLiant m350 Server Cartridge
HP ProLiant m400 Server Cartridge
HP ProLiant m700 Server Cartridge
HP ProLiant m800 Server Cartridge
HP ProLiant ML10 v2
HP ProLiant ML110 Gen9
HP ProLiant ML150 Gen9
HP ProLiant ML310e Gen8
HP ProLiant ML350 Gen9
HP ProLiant WS460c Gen8
HP ProLiant WS460c Gen9
```

**Feature Coverage**

<table><thead><tr><th width="192">Feature</th><th width="110" align="center">Windows</th><th width="128" align="center">VMware</th><th width="128" align="center">Linux</th><th align="center">Notes</th></tr></thead><tbody><tr><td>Processor</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"></td></tr><tr><td>Memory</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"></td></tr><tr><td>Hard Disk</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"></td></tr><tr><td>Array Controller</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"></td></tr><tr><td>Host Bus Adapter</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"></td></tr><tr><td>Network Adapter</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"></td></tr><tr><td>Power Supply</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"></td></tr><tr><td>Fan</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"></td></tr><tr><td>Model Images</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"></td></tr><tr><td>Specification Sheet</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"></td></tr></tbody></table>

***

## DELL

VirtualMetric supports DELL hardware to monitor hardware health and provide inventory information. Please check Model Coverage to see supported Models. Feature Coverage indicates supported feature sets for this manufacturer.

{% hint style="warning" %}
You need to install Dell OpenManage for Microsoft Windows x64 to monitor hardware health on Windows. Please download 7.4 or later versions.
{% endhint %}

**Model Coverage**

```markup
Dell PowerEdge M420
Dell PowerEdge M620
Dell PowerEdge M820
Dell PowerEdge R210
Dell PowerEdge R220
Dell PowerEdge R310
Dell PowerEdge R320
Dell PowerEdge R410
Dell PowerEdge R420
Dell PowerEdge R430
Dell PowerEdge R510
Dell PowerEdge R520
Dell PowerEdge R530
Dell PowerEdge R610
Dell PowerEdge R620
Dell PowerEdge R630
Dell PowerEdge R710
Dell PowerEdge R720
Dell PowerEdge R730
Dell PowerEdge R730xd
Dell PowerEdge R810
Dell PowerEdge R820
Dell PowerEdge R910
Dell PowerEdge R920
Dell PowerEdge T110
Dell PowerEdge T320
Dell PowerEdge T420
Dell PowerEdge T430
Dell PowerEdge T630
Dell PowerEdge R715
Dell PowerEdge R415
Dell PowerEdge R515
Dell PowerEdge R815
```

**Feature Coverage**

<table><thead><tr><th width="182">Feature</th><th width="104" align="center">Windows</th><th width="103" align="center">VMware</th><th width="102" align="center">Linux</th><th align="center">Notes</th></tr></thead><tbody><tr><td>Processor</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"></td></tr><tr><td>Memory</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"></td></tr><tr><td>Hard Disk</td><td align="center"><mark style="color:orange;">⚠️</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center">Requires LSI SMIS Windows Provider for MegaRAID support.</td></tr><tr><td>Array Controller</td><td align="center"><mark style="color:orange;">⚠️</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center">Requires LSI SMIS Windows Provider for MegaRAID support.</td></tr><tr><td>Host Bus Adapter</td><td align="center"><mark style="color:red;">✖︎</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"></td></tr><tr><td>Network Adapter</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"></td></tr><tr><td>Power Supply</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"></td></tr><tr><td>Fan</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"></td></tr><tr><td>Model Images</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"></td></tr><tr><td>Specification Sheet</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"></td></tr></tbody></table>

***

## IBM - LENOVO

VirtualMetric supports IBM / Lenovo hardware to monitor hardware health and provide inventory information. Please check Model Coverage to see supported Models. Feature Coverage indicates supported feature sets for this manufacturer.

{% hint style="warning" %}
You need to install IBM System Director Platform Agent to monitor hardware health on Windows. Please download 6.3.5 or later versions.
{% endhint %}

**Model Coverage**

```markup
IBM BladeCenter HS23
IBM BladeCenter HS23e
Lenovo ThinkServer RD350
Lenovo ThinkServer RD450
Lenovo ThinkServer RD550
Lenovo ThinkServer RD650
Lenovo ThinkServer RS140
IBM Flex System x220
IBM Flex System x222
IBM Flex System x240
IBM Flex System x240 M5
IBM System x3250 M4
IBM System x3250 M5
IBM System x3300 M4
IBM System x3500 M4
IBM System x3500 M5
IBM System x3530 M4
IBM System x3550 M3
IBM System x3550 M4
IBM System x3550 M5
IBM System x3630 M3
IBM System x3630 M4
IBM System x3650 M3
IBM System x3650 M4
IBM System x3650 M4 BD
IBM System x3650 M4 HD
IBM System x3650 M5
IBM System x3750 M4
IBM System x3850 x5
IBM System x3850 x6
IBM System x3950 x6
```

**Feature Coverage**

<table><thead><tr><th width="174">Feature</th><th width="110" align="center">Windows</th><th width="113" align="center">VMware</th><th width="91" align="center">Linux</th><th>Notes</th></tr></thead><tbody><tr><td>Processor</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr><tr><td>Memory</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr><tr><td>Hard Disk</td><td align="center"><mark style="color:orange;">⚠️</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>Requires LSI SMIS Windows Provider for MegaRAID support.</td></tr><tr><td>Array Controller</td><td align="center"><mark style="color:orange;">⚠️</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>Requires LSI SMIS Windows Provider for MegaRAID support.</td></tr><tr><td>Host Bus Adapter</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr><tr><td>Network Adapter</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr><tr><td>Power Supply</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr><tr><td>Fan</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr><tr><td>Model Images</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr><tr><td>Specification Sheet</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr></tbody></table>

## FUJITSU

VirtualMetric supports Fujitsu hardware to monitor hardware health and provide inventory information. Please check Model Coverage to see supported Models. Feature Coverage indicates supported feature sets for this manufacturer.

**Component Required**

You need to install Fujitsu ServerView Agent & CIM Providers for Windows to monitor hardware health on Windows. Please download 6.31.03 or later versions.

**Model Coverage**

```markup
Fujitsu Server Primergy BX400 S1
Fujitsu Server Primergy BX900 S2
Fujitsu Server Primergy RX1330 M1
Fujitsu Server Primergy RX2520 M1
Fujitsu Server Primergy RX2530 M1
Fujitsu Server Primergy RX2540 M1
Fujitsu Server Primergy RX2560 M1
Fujitsu Server Primergy RX300 S8
Fujitsu Server Primergy RX350 S8
Fujitsu Server Primergy RX4770 M1
Fujitsu Server Primergy RX4770 M2
Fujitsu Server Primergy TX1310 M1
Fujitsu Server Primergy TX1320 M1
Fujitsu Server Primergy TX1330 M1
Fujitsu Server Primergy TX150 S8
Fujitsu Server Primergy TX2540 M1
Fujitsu Server Primergy TX2560 M1
Fujitsu Server Primergy TX300 S8
```

**Feature Coverage**

<table><thead><tr><th>Feature</th><th width="108" align="center">Windows</th><th width="98" align="center">VMware</th><th width="87" align="center">Linux</th><th>Notes</th></tr></thead><tbody><tr><td>Processor</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr><tr><td>Memory</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr><tr><td>Hard Disk</td><td align="center"><mark style="color:orange;">⚠️</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>Requires LSI SMIS Windows Provider for MegaRAID support.</td></tr><tr><td>Array Controller</td><td align="center"><mark style="color:orange;">⚠️</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>Requires LSI SMIS Windows Provider for MegaRAID support.</td></tr><tr><td>Host Bus Adapter</td><td align="center"><mark style="color:red;">✖︎</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr><tr><td>Network Adapter</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr><tr><td>Power Supply</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr><tr><td>Fan</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr><tr><td>Model Images</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr><tr><td>Specification Sheet</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr></tbody></table>

***

## CISCO

VirtualMetric supports Cisco hardware to monitor hardware health and provide inventory information. Please check Model Coverage to see supported Models. Feature Coverage indicates supported feature sets for this manufacturer.

**Model Coverage**

```markup
Cisco UCS B22 M3
Cisco UCS B200 M3
Cisco UCS B200 M4
Cisco UCS B230 M2
Cisco UCS B260 M4
Cisco UCS B420 M3
Cisco UCS B420 M4
Cisco UCS B440 M2
Cisco UCS B460 M4
Cisco UCS C22 M3
Cisco UCS C24 M3
Cisco UCS C220 M3
Cisco UCS C220 M4
Cisco UCS C240 M3
Cisco UCS C240 M4
Cisco UCS C260 M2
```

**Feature Coverage**

<table><thead><tr><th width="208">Feature</th><th width="106" align="center">Windows</th><th width="95" align="center">VMware</th><th width="77" align="center">Linux</th><th>Notes</th></tr></thead><tbody><tr><td>Processor</td><td align="center"><mark style="color:red;">✖︎</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>Windows IPMI support is available for this feature.</td></tr><tr><td>Memory</td><td align="center"><mark style="color:red;">✖︎</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>Windows IPMI support is available for this feature.</td></tr><tr><td>Hard Disk</td><td align="center"><mark style="color:red;">✖︎</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>Windows IPMI support is available for this feature.</td></tr><tr><td>Array Controller</td><td align="center"><mark style="color:red;">✖︎</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>Windows IPMI support is available for this feature.</td></tr><tr><td>Host Bus Adapter</td><td align="center"><mark style="color:red;">✖︎</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>Windows IPMI support is available for this feature.</td></tr><tr><td>Network Adapter</td><td align="center"><mark style="color:red;">✖︎</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>Windows IPMI support is available for this feature.</td></tr><tr><td>Power Supply</td><td align="center"><mark style="color:red;">✖︎</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>Windows IPMI support is available for this feature.</td></tr><tr><td>Fan</td><td align="center"><mark style="color:red;">✖︎</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>Windows IPMI support is available for this feature.</td></tr><tr><td>Model Images</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr><tr><td>Specification Sheet</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr></tbody></table>

***

## SUPERMICRO

VirtualMetric supports SuperMicro hardware to monitor hardware health and provide inventory information. Feature Coverage indicates supported feature sets for this manufacturer.

{% hint style="warning" %}
You need to install SuperMicro SuperDoctor to monitor hardware health on Windows. Please download 5 or later versions.
{% endhint %}

**Feature Coverage**

<table><thead><tr><th width="187">Feature</th><th width="107" align="center">Windows</th><th width="100" align="center">VMware</th><th width="79" align="center">Linux</th><th>Notes</th></tr></thead><tbody><tr><td>Processor</td><td align="center"><mark style="color:red;">✖︎</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>Windows IPMI support is available for this feature.</td></tr><tr><td>Memory</td><td align="center"><mark style="color:red;">✖︎</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>Windows IPMI support is available for this feature.</td></tr><tr><td>Hard Disk</td><td align="center"><mark style="color:orange;">⚠️</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>Requires LSI SMIS Windows Provider for MegaRAID support.</td></tr><tr><td>Array Controller</td><td align="center"><mark style="color:orange;">⚠️</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>Requires LSI SMIS Windows Provider for MegaRAID support.</td></tr><tr><td>Host Bus Adapter</td><td align="center"><mark style="color:red;">✖︎</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr><tr><td>Network Adapter</td><td align="center"><mark style="color:red;">✖︎</mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td>Windows IPMI support is available for this feature.</td></tr><tr><td>Power Supply</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr><tr><td>Fan</td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td align="center"><mark style="color:green;"><strong>✓</strong></mark></td><td></td></tr><tr><td>Model Images</td><td align="center"><mark style="color:red;">✖︎</mark></td><td align="center"><mark style="color:red;">✖︎</mark></td><td align="center"><mark style="color:red;">✖︎</mark></td><td></td></tr><tr><td>Specification Sheet</td><td align="center"><mark style="color:red;">✖︎</mark></td><td align="center"><mark style="color:red;">✖︎</mark></td><td align="center"><mark style="color:red;">✖︎</mark></td><td></td></tr></tbody></table>

