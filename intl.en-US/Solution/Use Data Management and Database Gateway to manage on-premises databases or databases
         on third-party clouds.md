# Use Data Management and Database Gateway to manage on-premises databases or databases on third-party clouds

Database Gateway allows you to connect on-premises databases or databases that are hosted on third-party clouds to Alibaba Cloud services. You do not need to open the service ports of the databases to the Internet. This ensures data security. You can use Database Gateway to register on-premises databases or databases on third-party clouds in Data Management \(DMS\). You can then manage these databases in the DMS console.

DMS is activated. The account that is used to log on to the [DMS console](https://dms.alibabacloud.com/) assumes the administrator or the database administrator role.

You can connect an on-premises database or a database that is hosted on a third-party cloud to Alibaba Cloud by using one of the following methods. However, each method has limits.

-   Use a dedicated connection, a VPN gateway, or a smart access gateway. This method is not suitable for individual users because of high costs.
-   Use the service port of the database over the Internet. This method causes potential security risks.
-   Use a user-created proxy to forward service requests. This method provides low stability and requires that you can create a proxy.

DMS allows you to use Database Gateway to register databases that are hosted on third-party clouds. You do not need to open the service ports of the databases to the Internet. Database Gateway encrypts data transmission and supports simple configurations that do not require firewalls. For more information about Database Gateway, see [What is Database Gateway?](~~124253~~)

1.  Create a database gateway. For more information, see [Create a database gateway](~~122129~~).

2.  Add a database that you want to connect to Alibaba Cloud. For more information, see [Add databases](~~123189~~).

    When you use the Database Gateway service, no fees are charged. Make sure that the following requirements are met:

    -   The server where the database gateway is installed can access the Internet. The service port of the server does not need to be open to the Internet.
    -   The server where the database gateway is installed can connect to the database. If the server and the database are deployed in the same internal network, the network latency is minimal.
3.  Log on to the [DMS console](https://dms.alibabacloud.com/). In the upper-left corner, choose Add instance/Batch entry \> **Add instance**.

    ![tp](../images/p141335.png)

4.  In the Add instance dialog box, select **No public address database**. On the tab that appears, select a database type.

    ![tp](../images/p141336.png)

5.  Configure the instance parameters.

    ![tp](../images/p141337.png)

    The following table lists the instance parameters.

    |**Section**|**Parameter**|**Description**|
    |Basic Information|Database Source|The source of the database instance. Select **No public address database**.|
    |Database type|The type of the database instance.|
    |Instance Area|The region where the database gateway resides.|
    |Gateway ID|The ID of the database gateway. To create a database gateway, click **Click here to add a database gateway**.|
    |Database address|The internal IP address of the database.|
    |Ports|The service port number of the database.|
    |Database account|The username that you can use to log on to the database.|
    |Database password|The password of the username.|
    |Control Mode|The control mode that you can use to manage the database instance in DMS. For more information, see [Control modes](~~151629~~).|
    |Advanced information|Environment type|The type of the environment where the database instance is deployed.|
    |Instance Name|The name of the database instance.|
    |Enable DSQL|Specifies whether to enable the cross-database query feature for the database instance. For more information, see [Cross-database query](~~127641~~).|
    |OnlineDDL|Specifies whether to allow changing schemas without locking tables for the database instance. For more information, see [Change schemas without locking tables](~~98373~~).|
    |DBA|The database administrator of the database instance. The database administrator can grant permissions to users.|
    |query timeout\(s\)|The timeout period for the execution of an SQL query statement. If the execution of an SQL query statement lasts longer than the specified timeout period, the execution of the statement is terminated. This ensures database security.|
    |export timeout\(s\)|The timeout period for the execution of an SQL export statement. If the execution of an SQL export statement lasts longer than the specified timeout period, the execution of the statement is terminated. This ensures database security.|

6.  Click **Test connection**.

    **Note:** If the test fails, check the preceding parameters that you have configured for the instance.

7.  If the test is successful, click **Submit**. Then, the database on the third-party cloud is registered in DMS. You can view and manage the database in the left-side instance list in the DMS console.


