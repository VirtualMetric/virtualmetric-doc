---
layout:
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Add New Organization

To create a new Organization, you should go to Settings tab.

1\.      Click to **Organizations** on the left pane to navigate to the Organization Settings.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (316).png" alt=""><figcaption></figcaption></figure>

</div>

2\.      On Organization Management screen, click **Add (+)** button on the right top section.

<figure><img src="../../../.gitbook/assets/image (317).png" alt=""><figcaption></figcaption></figure>

3\.      Enter Organization properties, then click **Submit** button.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (318).png" alt="" width="291"><figcaption></figcaption></figure>

</div>

<table><thead><tr><th width="199">Fields</th><th>Descriptions</th></tr></thead><tbody><tr><td>Organization Name</td><td>Here you can enter your desired Organization Name.</td></tr><tr><td>Status</td><td>Status of organization. If you make it Disabled, then the organization and all organization users will not be able to login VirtualMetric Dashboard. You can change organization status to Active / Disabled anytime.</td></tr><tr><td>Username</td><td>Organization will use this username to login to VirtualMetric Dashboard.</td></tr><tr><td>Email Address</td><td>VirtualMetric will use this email address for Password Recovery email.</td></tr><tr><td>First Name</td><td>First name of organization's primary contact. VirtualMetric will use it in notification emails.</td></tr><tr><td>Last name</td><td>Last name of organization's primary contact. VirtualMetric will use it in notification emails.</td></tr><tr><td>Password</td><td>Organization will use this password to login to VirtualMetric Dashboard. If you select <strong>Active Directory Authentication</strong>, then you don't have to type password. VirtualMetric will authenticate this organization with the Active Directory authentication.</td></tr><tr><td>Language</td><td>VirtualMetric will use this language for VirtualMetric Dashboard and VirtualMetric API localization. </td></tr></tbody></table>

## **When Active Directory Enabled;**&#x20;

Change username as Active Directory logon name like **DOMAIN\username** (pre-Windows 2000 style).

You can find User logon name under User Properties in Active Directory Users and Computers. Click to **Account** tab to see User logon name (pre-Windows 2000).

<div align="left">

<figure><img src="../../../.gitbook/assets/image (319).png" alt="" width="213"><figcaption></figcaption></figure>

</div>

{% hint style="warning" %}
If you don't type username as Active Directory Logon Name (pre-Windows 2000 style), VirtualMetric will not use Active Directory Authentication.
{% endhint %}
