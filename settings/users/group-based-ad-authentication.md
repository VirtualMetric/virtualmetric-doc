# Group Based AD Authentication

Enterprise customers may create role-based permission by Active Directory and get permission from internal authentication systems.

Virtualmetric can create roles and organizations based on Active Directory.

An organization is created using the organization ID or name.&#x20;

After creating the organization, roles associated with the organization are created.

1\.      VIRTUALMETRIC\_XXXX\_ADMIN: Admin role for specified organization.&#x20;

2\.      VIRTUALMETRIC\_XXXX\_USER: User role for specified organization.&#x20;

3\.      VIRTUALMETRIC\_XXXX\_READONLY: Readonly role for specified organization.&#x20;

{% hint style="info" %}
The "XXXX" expressions could be the name or ID of the organization.
{% endhint %}

Lastly, users can get permission to roles.&#x20;
