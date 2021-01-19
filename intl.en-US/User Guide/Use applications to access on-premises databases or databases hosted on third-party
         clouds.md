# Use applications to access on-premises databases or databases hosted on third-party clouds



## Background information

Database Gateway \(DG\) provides database access points. In Alibaba Cloud virtual private clouds \(VPCs\), you can use applications to access on-premises databases and databases hosted on third-party clouds. This ensures secure and reliable access to databases that are deployed on multiple clouds. This also helps you meet the requirements in various scenarios, such as data integration in hybrid cloud environments and data migration.

![Background information](../images/p208292.png)

## Prerequisites

-   A local agent is started and a database is added. For more information, see [Quick Start](/intl.en-US/.md).
-   A VPC and a vSwitch are created in the same region where Database Gateway is deployed.

## Procedure

1.  Log on to the [Database Gateway console](https://account.aliyun.com/login/login.htm?oauth_callback=https%3A%2F%2Fdg.console.aliyun.com%2Fgateway&lang=zh).
2.  In the left-side navigation pane, click **Gateway List**.

    ![Gateway list](../images/p208324.png)

3.  Navigate to the page that shows the details about the added database. In the **Operation** column on this page, click **Create a database access point**.

    ![Gateway details](../images/p208328.png)

4.  Select the **VPC ID** and the **vSwitch**. Click **OK**. Then, you can use the VPC endpoint to establish connections.

    ![Add a database](../images/p208342.png)

5.  Log on to an Elastic Compute Service \(ECS\) instance that is connected to the VPC and test whether the displayed VPC endpoint is valid. If the connection is successful, you can use methods such as the Java Database Connectivity \(JDBC\) method to access on-premises databases and databases that are hosted on third-party clouds.

    ![The output returned on the ECS instance](../images/p208345.png)


