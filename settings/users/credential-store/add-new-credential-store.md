# Add New Credential Store

1\.      Click to **Users Groups** on the **left pane** to navigate to the User Settings.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (342).png" alt=""><figcaption></figcaption></figure>

</div>

2\.      On User Management screen, click **Add (+)** button on the right top section.

<figure><img src="../../../.gitbook/assets/image (343).png" alt=""><figcaption></figcaption></figure>

3\.      Select the action type and fill the other fields, then click **Submit**

<div align="left">

<figure><img src="../../../.gitbook/assets/image (344).png" alt="" width="293"><figcaption></figcaption></figure>

</div>

Select an Action Type from the field. The Action Type refers to a different method or mechanism for authentication, and each has its own set of actions or operations associated with it. You can see an array of Action Type such as Basic, SSH key based, Cyberark, SNMPv2, SNMPv3, API Key, Bearer Token, HMAC, HTTP Header, etc. Let's see how we can create each of these Action Type.&#x20;

## **Basic**&#x20;

Select Basic option from the dropdown menu. You get the following screen:&#x20;

<div align="left">

<figure><img src="../../../.gitbook/assets/image (345).png" alt="" width="293"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._&#x20;

<table><thead><tr><th width="218">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Action Type </td><td>This is the basic authentication method which involves username and password. </td></tr><tr><td>Visibility  </td><td><p>To provide visibility to either your own organization or all the other organizations. The options are: </p><p>1) My Organizations </p><p>2) All Organizations </p><p> </p></td></tr><tr><td>Friendly Name </td><td>Any name which user wants to use. </td></tr><tr><td>Description  </td><td>Provide a description about the Credential Store  </td></tr><tr><td>Username </td><td>Add an appropriate username as you like </td></tr><tr><td>Password  </td><td>Add a password  </td></tr></tbody></table>

## **SSH Key Based**&#x20;

<div align="left">

<figure><img src="../../../.gitbook/assets/image (347).png" alt="" width="291"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._&#x20;

<table><thead><tr><th width="237">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Action Type </td><td>SSH key-based authentication is a method used for securely connecting to remote servers and services over SSH (Secure Shell) without the need to enter a password. </td></tr><tr><td>Visibility  </td><td><p>To provide visibility to either your own organization or all the other organizations. The options are: </p><p>1) My Organizations </p><p>2) All Organizations </p><p> </p></td></tr><tr><td>Friendly Name </td><td>Any name which user wants to use. </td></tr><tr><td>Description  </td><td>Provide a description about the Credential Store  </td></tr><tr><td>Username </td><td>Add an appropriate username as you like </td></tr><tr><td>SSH Private Key </td><td>Add a password which should be the OpenSSH key in PEM format </td></tr><tr><td>Enable Passphrase </td><td>Select the checkbox, you will get an additional field to add a Passphrase of your choice. </td></tr></tbody></table>

## **Cyberark**&#x20;

<div align="left">

<figure><img src="../../../.gitbook/assets/image (348).png" alt="" width="291"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._&#x20;

<table><thead><tr><th width="199">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Action Type </td><td>Cyberark is an authentication method which involves storing, retrieving, rotating, and managing privileged credentials (e.g., usernames and passwords) for sensitive systems and accounts. It also includes monitoring and auditing access to privileged accounts. </td></tr><tr><td>Visibility  </td><td><p>To provide visibility to either your own organization or all the other organizations. The options are: </p><p>1) My Organizations </p><p>2) All Organizations </p><p> </p></td></tr><tr><td>Friendly Name </td><td>Any name which user wants to use. </td></tr><tr><td>Description  </td><td>Provide a description about the Credential Store  </td></tr><tr><td>Name </td><td>Name of an object or resource which typically refers to a specific identifier used to uniquely designate items such as encryption keys, database servers, etc. </td></tr><tr><td>Application </td><td><p>This term denotes the application or system component linked to the associated resource. Particularly in a complex IAM (Identity and Access Management) enviornment where multiple applications or systems are utilized, it becomes vital to specify the affiliation of each resource to a particular application. This allows for more granular management of authorization and permissions. </p><p> </p></td></tr><tr><td>Safe </td><td>Safe represents a secure repository or vault where privileged credentials, such as usernames and passwords, SSH keys, and other sensitive information, are stored and managed </td></tr><tr><td>Folder </td><td>Folder serves as a way to organize and categorize objects within a Safe. Objects can include credentials, secrets, and other sensitive information. </td></tr><tr><td>Port </td><td>A specific endpoint for data exchange between two devices or applications within a network. </td></tr><tr><td>Object Name </td><td>This term typically refers to a specific resource or object within an application. It could be a file, folder, database table, or another entity within an application. Object names are used when creating access control lists or configuring authentication and authorization processes. </td></tr></tbody></table>

## **SNMPv2**&#x20;

<div align="left">

<figure><img src="../../../.gitbook/assets/image (349).png" alt="" width="290"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._&#x20;

<table><thead><tr><th width="209">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Action Type </td><td>This authentication method is used to monitor and manage networked devices, such as routers, switches, servers, and network printers. </td></tr><tr><td>Visibility  </td><td><p>To provide visibility to either your own organization or all the other organizations. The options are: </p><p>1) My Organizations </p><p>2) All Organizations </p></td></tr><tr><td>Friendly Name </td><td>Any name which user wants to use. </td></tr><tr><td>Description  </td><td>Provide a description about the Credential Store  </td></tr><tr><td>Community String </td><td><p>The Community String is a basic form of authentication and access control used to manage and monitor network devices. It acts like a password or a shared secret that SNMP agents and managers use to authenticate and authorize SNMP requests. </p><p>Example: public, private</p></td></tr></tbody></table>

## **SNMPv3**&#x20;

<div align="left">

<figure><img src="../../../.gitbook/assets/image (350).png" alt="" width="292"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._&#x20;

<table><thead><tr><th width="196">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Action Type </td><td><p></p><p>This authentication method is used to monitor and manage networked devices, such as routers, switches, servers, and network printers. It is an enhanced and more secure version of SNMP compared to its predecessors, SNMPv1 and SNMPv2c. </p></td></tr><tr><td>Visibility  </td><td><p>To provide visibility to either your own organization or all the other organizations. The options are: </p><p>1) My Organizations </p><p>2) All Organizations </p></td></tr><tr><td>Friendly Name </td><td>Any name which user wants to use. </td></tr><tr><td>Description  </td><td>Provide a description about the Credential Store  </td></tr><tr><td>Authentication Protocol </td><td>The authentication protocol used for SNMPv3 includes MD5, SHA, SHA224, SHA256, SHA384, SHA512, etc. </td></tr><tr><td>Username </td><td>Add an appropriate username as you like </td></tr><tr><td>Password  </td><td>Add a password  </td></tr><tr><td>Privacy Protocol </td><td>The privacy protocols are used for encrypting SNMP payloads, protecting sensitive information from unauthorized access or eavesdropping. There are two primary privacy protocols in SNMPv3: DES and AES. You can also choose other options such as None, AES192, AES192C, AES256, AES256 from the dropdowns. </td></tr></tbody></table>

## **API Key**&#x20;

<div align="left">

<figure><img src="../../../.gitbook/assets/image (351).png" alt="" width="291"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._&#x20;

<table data-header-hidden><thead><tr><th width="217">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Action Type </td><td>This is another authentication method used to authenticate and authorize access to an API. </td></tr><tr><td>Visibility  </td><td><p>To provide visibility to either your own organization or all the other organizations. The options are: </p><p>1) My Organizations </p><p>2) All Organizations </p></td></tr><tr><td>Friendly Name </td><td>Any name which user wants to use. </td></tr><tr><td>Description  </td><td>Provide a description about the Credential Store  </td></tr><tr><td>Key </td><td>Unique identifier used to connect to, or perform, an API call. </td></tr><tr><td>Value </td><td><p>Refers to the actual alphanumeric code that makes up the API key </p><p> </p></td></tr><tr><td>Add To </td><td><p>There are 2 options: </p><p>Header and Query Params. You can add the API Key to the API Header or in the Query Parameters as needed. </p></td></tr></tbody></table>

## **Bearer Token**&#x20;

<div align="left">

<figure><img src="../../../.gitbook/assets/image (352).png" alt="" width="292"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._&#x20;

<table><thead><tr><th width="223">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Action Type </td><td>The Bearer Token authentication method is a widely used approach for securing APIs and web services. </td></tr><tr><td>Visibility  </td><td><p>To provide visibility to either your own organization or all the other organizations. The options are: </p><p>1) My Organizations </p><p>2) All Organizations </p></td></tr><tr><td>Friendly Name </td><td>Any name which user wants to use. </td></tr><tr><td>Description  </td><td>Provide a description about the Credential Store  </td></tr><tr><td>Token </td><td>The token that is used for authentication. </td></tr></tbody></table>

## **HMAC**&#x20;

<div align="left">

<figure><img src="../../../.gitbook/assets/image (353).png" alt="" width="288"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._&#x20;

<table><thead><tr><th width="237">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Action Type </td><td>HMAC is a specific type of message authentication code (MAC) that uses a cryptographic hash function along with a secret key to create a fixed-size hash value (digest) from the input data. HMAC is commonly used in various security protocols and applications, including securing network communications (e.g., in VPNs and IPsec), web authentication (e.g., OAuth), message authentication in cryptography, and more.</td></tr><tr><td>Visibility  </td><td><p>To provide visibility to either your own organization or all the other organizations. The options are: </p><p>1) My Organizations </p><p>2) All Organizations </p></td></tr><tr><td>Friendly Name </td><td>Any name which user wants to use. </td></tr><tr><td>Description  </td><td>Provide a description about the Credential Store  </td></tr><tr><td>Http header </td><td>HTTP headers contain additional information about the request or response, facilitating communication between a client and a server by conveying details like content type, caching directives, authentication credentials, and more.</td></tr><tr><td>Key </td><td>In HAMC, key is a secret cryptographic key that is used to generate the authentication tag and to verify the authenticity and integrity of a message or data.  </td></tr><tr><td>Type </td><td><p>There are different types HAMC to select from the dropdowns: </p><p>SHA1, SHA256, SHA512 </p></td></tr><tr><td>Prefix </td><td>Refers to a sequence of characters added to the beginning of a string, variable, or identifier. </td></tr></tbody></table>

&#x20;

## **HTTP Header**&#x20;

<div align="left">

<figure><img src="../../../.gitbook/assets/image (354).png" alt="" width="289"><figcaption></figcaption></figure>

</div>

_Refer to the following table to understand the fields in the above screen._&#x20;

<table><thead><tr><th width="207">Fields</th><th>Description</th></tr></thead><tbody><tr><td>Action Type </td><td><p></p><p>This is another authentication method which is included in the HTTP message as key-value pairs and is transmitted as part of the HTTP protocol. </p></td></tr><tr><td>Visibility  </td><td><p>To provide visibility to either your own organization or all the other organizations. The options are:</p><p>1) My Organizations </p><p>2) All Organizations </p></td></tr><tr><td>Friendly Name </td><td>Any name which user wants to use. </td></tr><tr><td>Description  </td><td>Provide a description about the Credential Store  </td></tr><tr><td>Header </td><td>Name of secret </td></tr><tr><td>Value </td><td>Value (password of secret) </td></tr></tbody></table>
