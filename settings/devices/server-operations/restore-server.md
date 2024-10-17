# Restore Server

If you remove a server mistakenly, you can still revert changes back from VirtualMetric Database. First you should connect to your current Microsoft SQL Server instance via [SQL Server Management Studio.](https://en.wikipedia.org/wiki/SQL\_Server\_Management\_Studio)

## SQL Management

1. Open SQL Server Management Studio.
2.  In the left menu, under **VIRTUALMETRICDB**, select Tables.

    <div align="left">

    <figure><img src="../../../.gitbook/assets/image (552).png" alt="" width="356"><figcaption></figcaption></figure>

    </div>
3.  Locate **dbo.Host** and right-click on it, then choose "**Edit Top 200 Rows**" from the menu.

    <div align="left">

    <figure><img src="../../../.gitbook/assets/image (553).png" alt="" width="375"><figcaption></figcaption></figure>

    </div>
4.  Find the RecordStatus column; it will display a value of **4**.

    <div align="left">

    <figure><img src="../../../.gitbook/assets/image (554).png" alt=""><figcaption></figcaption></figure>

    </div>
5. Change the RecordStatus value to **1** to set the server status as **Active**.

## IIS Manager

You must restart application pool of **VirtualMetric API** via **IIS Manager** to apply server restore.

1.  Open IIS Manager on the VirtualMetric Standalone Server.

    <div align="left">

    <figure><img src="../../../.gitbook/assets/image (555).png" alt="" width="306"><figcaption></figcaption></figure>

    </div>
2.  In the left menu, click on "**Application Pools.**"

    <div align="left">

    <figure><img src="../../../.gitbook/assets/image (556).png" alt="" width="353"><figcaption></figcaption></figure>

    </div>
3. Right-click on "**VirtualMetric API**" and select "**Recycle**" to restart the application pool.

<div align="left">

<figure><img src="../../../.gitbook/assets/image (557).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

4. After the application pool restarts, return to the Server Management screen.
5.  On the Server Management screen, click the **Refresh** button (represented by a circular arrow icon) in the **upper-right section**.

    <div align="left">

    <figure><img src="../../../.gitbook/assets/image (559).png" alt=""><figcaption></figcaption></figure>

    </div>
6. You will see that the server entry is once again restored in the Server List.

{% hint style="info" %}
**Note:** After an accidental removal, you have a **15-minute window** to restore the server. If you don't restore it within this time frame, the VirtualMetric Cleanup Job will permanently remove the server.
{% endhint %}
