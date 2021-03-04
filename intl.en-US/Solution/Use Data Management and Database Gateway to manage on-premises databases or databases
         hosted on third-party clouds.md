# Use Data Management and Database Gateway to manage on-premises databases or databases hosted on third-party clouds

Database Gateway \(DG\) allows you to connect on-premises databases or databases that are hosted on third-party clouds to Alibaba Cloud services. You do not need to use public IP addresses to establish connections. This prevents the security risks of using public IP connections. In Data Management \(DMS\), you can use Database Gateway to register on-premises databases or databases that are hosted on third-party clouds. You can then manage these databases.

You can connect an on-premises database or a database that is hosted on a third-party cloud to Alibaba Cloud by using one of the following methods. However, each of these methods has limits:

-   Use a leased line, a VPN gateway, or a smart access gateway: This method is not suitable for individual users due to high costs.
-   Open the service port of the database to the Internet: This method causes potential security risks.
-   Use a user-created proxy to forward service requests: This method requires high technology costs and does not ensure high stability.

To resolve the preceding issues, DMS allows you to use Database Gateway to register on-premises databases or databases that are hosted on third-party clouds. You do not need to use the public IP addresses of the databases to establish connections. Database Gateway also encrypts data transmission. For more information about Database Gateway, see [What is Database Gateway?](~~124253~~)

1.  Log on to the [Database Gateway console](https://account.aliyun.com/login/login.htm?oauth_callback=https%3A%2F%2Fdg.console.aliyun.com%2Fgateway&lang=en). In the upper-left corner, select the region where the database is deployed. The default region is China \(Hangzhou\). Then, click **Create Gateway**.

2.  In the Create Gateway dialog box, specify the gateway name and the note. Then, click **Next step**.

    ![Great Gateway](https://static-aliyun-doc.oss-accelerate.aliyuncs.com/assets/img/en-US/6354484161/p245506.png)

3.  Install the gateway. Select an installation package based on the type of your operating system. If you use the Windows operating system, click **Download gateway**. If you use other operating systems, copy and paste the command line to the machine where the gateway is to be installed. Then, press Enter to run the command. If the local gateway is started as expected, you are automatically redirected to the Adding a Database page. You can also click **Next step**.

    **Note:** Database Gateway is available for free. You must make sure that the machine where the gateway program is deployed meets the following requirements:

    -   The machine can connect to the database that is to be accessed. If the machine and the database are deployed in the same internal network, the network latency is reduced.
    -   The machine can access the Internet. No public IP address is required. The service port does not need to be open to the Internet. The machine does not need to be accessed by the Internet.
    ![install gateway](https://static-aliyun-doc.oss-accelerate.aliyuncs.com/assets/img/en-US/6354484161/p245507.png)

4.  Add a database. You can click **Add database address** to add a database to the gateway. Alternatively, you can add a database later. For more information about how to add a database, see [Add databases](/intl.en-US/User Guide/Add databases.md).

    ![Edit Gateway](https://static-aliyun-doc.oss-accelerate.aliyuncs.com/assets/img/en-US/7354484161/p245509.png)

5.  Log on to the [DMS](https://dms.aliyun.com/) console. In the upper-left corner of the page, click **Add instance**.

    ![Add instance](https://static-aliyun-doc.oss-accelerate.aliyuncs.com/assets/img/en-US/4455484161/p245521.png)

6.  In the **Add instance** dialog box, click **Local/other cloud database**. Then, select a database type.

    ![Localclouddatabase](https://static-aliyun-doc.oss-accelerate.aliyuncs.com/assets/img/en-US/4455484161/p245523.png)

7.  In the **Add instance** dialog box, specify the instance information based on the descriptions in the following table.

    ![BasicInformation](https://static-aliyun-doc.oss-accelerate.aliyuncs.com/assets/img/en-US/4455484161/p245525.png)

    |Tab name|Parameter name|Description|
    |--------|--------------|-----------|
    |Basic Information|Data source|The source of the database instance. In this example, the Local/other cloud database option is selected.|
    |Database type|The type of the database instance.|
    |Instance Area|The region where the database gateway is deployed.|
    |Gateway ID|The ID of the database gateway. If you have not created database gateways, click **Click here to add a database gateway** to create a database gateway.|
    |Database address|The internal endpoint of the database.|
    |Port|The service port of the database.|
    |Database account|The username that you use to log on to the database.|
    |Database password|The password of the username for the database.|
    |Control Mode|The control mode for the database. For more information, see [Control modes](https://help.aliyun.com/document_detail/151629.html).|
    |Advanced information|Environment type|The type of the environment where the database is deployed.|
    |Instance Name|The custom name of the instance.|
    |Enable DSQL|Specifies whether to enable the cross-database query feature. For more information, see [Cross-database query](https://help.aliyun.com/document_detail/127641.html).|
    |OnlineDDL|Specifies whether to enable the feature of changing schemas without locking tables. For more information, see [Change schemas without locking tables](https://help.aliyun.com/document_detail/98373.html).|
    |DBA|The database administrator who handles subsequent processes, such as the process of applying for permissions.|
    |query timeout\(s\)|The security policy: If a query statement is not fully executed within the specified period, the statement is terminated in the SQL window. This ensures database security.|
    |export timeout\(s\)|The security policy: If an export statement is not fully executed within the specified period, the statement is terminated in the SQL window. This ensures database security.|

8.  In the lower-left corner of the dialog box, click **Test connection** and wait until the connection passes the test.

    **Note:** If the connection fails the test, check the instance information that you specify.

9.  Click **Submit**. Now your on-premises database or database hosted on a third-party cloud has been registered in DMS. In the instance list in the left-side navigation pane of the DMS console, you can view and manage your database.


