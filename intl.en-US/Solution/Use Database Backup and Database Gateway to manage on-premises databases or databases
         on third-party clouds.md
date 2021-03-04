# Use Database Backup and Database Gateway to manage on-premises databases or databases on third-party clouds

Database Backup allows you to use Database Gateway to back up on-premises databases or private databases on third-party clouds to Alibaba Cloud. You can connect your databases to Alibaba Cloud at a low cost in a few simple steps. Then, you can specify a database that is connected to a database gateway as the source database when you configure a backup schedule of the logical backup mode. This topic describes how to use Database Gateway to back up on-premises databases or private databases on third-party clouds to Alibaba Cloud.

You can connect an on-premises database or a database that is hosted on a third-party cloud to Alibaba Cloud by using one of the following methods. However, each method has limits.

-   Use a dedicated connection, a VPN gateway, or a smart access gateway. This method is not suitable for individual users because of high costs.
-   Use the service port of the database over the Internet. This method causes potential security risks.
-   Use a user-created proxy to forward service requests. This method provides low stability and requires that you can create a proxy.

For more information about Database Gateway, see [What is Database Gateway?](~~124253~~)

1.  Create a database gateway. For more information, see [Create a database gateway](~~122129~~).

2.  Add a database that you want to connect to Alibaba Cloud. For more information, see [Add databases](~~123189~~).

    When you use the Database Gateway service, no fees are charged. Make sure that the following requirements are met:

    -   The server where the database gateway is installed can access the Internet. The service port of the server does not need to be open to the Internet. To ensure stable data transmission over channels, the outbound public bandwidth must be at least 10 Mbit/s.
    -   The server where the database gateway is installed can connect to the database. If the server and the database are deployed in the same internal network, the network latency is minimal.
3.  Configure a backup schedule in the Database Backup console. For more information, see [Configure a backup schedule](~~59609~~).

    Set **Database Location** to **No public network IP: Port's self-built database \(accessed through the database gateway\)**. This allows you to specify the database that is connected to the database gateway as the source database.

    ![Select an instance type](https://static-aliyun-doc.oss-accelerate.aliyuncs.com/assets/img/en-US/3623097951/p97936.png)

    **Note:** If you select **No public network IP: Port's self-built database \(accessed through the database gateway\)**, cross-region backup is not supported. The source database instance must be in the same region as the Object Storage Service \(OSS\) bucket where the backup data is stored.


