# Connect to Database Gateway by using Express Connect, VPN Gateway, or CEN



## Background information

Express Connect circuits are used in Express Connect to connect on-premises databases to the cloud. You must configure a whitelist for the on-premises databases. If you want to connect on-premises databases to cloud services, you must add the CIDR blocks of the cloud services to the whitelists of the databases. The examples of the cloud services include Data Management \(DMS\), Data Transmission Service \(DTS\), and Database Backup Service \(DBS\). If the CIDR blocks change, you must update the configurations of the database whitelists. This results in high operations and maintenance \(O&M\) costs.

Database Gateway simplifies the configurations of the database whitelists. You need only to add the on-premises Database Gateway agent to the database whitelists. In this case, if the CIDR blocks of a cloud service change, you do not need to update the configurations of the database whitelists. If the on-premises databases are connected to the cloud over Express Connect circuits, the Database Gateway agent reuses the Express Connect circuits. This method provides a higher network quality than that in the scenario where the connections are established over the Internet.

![backgroud](https://static-aliyun-doc.oss-accelerate.aliyuncs.com/assets/img/en-US/4678273161/p241645.png)

## Prerequisites

1.  The Alibaba Cloud Database Gateway service is activated. For more information, see **Preparations**.
2.  The Express Connect, VPN Gateway, or Cloud Enterprise Network \(CEN\) service is configured as required.

## Procedure

1.  When you create a database gateway, select **Using Express/CEN/VPN Gateway to access**. For more information about how to create a database gateway, see **Create a database gateway**.

    ![Create a database gateway](https://static-aliyun-doc.oss-accelerate.aliyuncs.com/assets/img/en-US/4678273161/p241651.png)

2.  Specify the IP address of the host and the port number for the on-premises database. Then, click **Complete**.

    ![Adding a Database](https://static-aliyun-doc.oss-accelerate.aliyuncs.com/assets/img/en-US/4678273161/p241659.png)


