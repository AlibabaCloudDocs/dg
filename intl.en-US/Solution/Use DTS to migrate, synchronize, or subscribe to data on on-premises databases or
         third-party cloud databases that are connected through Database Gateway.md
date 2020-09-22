# Use DTS to migrate, synchronize, or subscribe to data on on-premises databases or third-party cloud databases that are connected through Database Gateway

This topic describes how to connect an on-premises database or a database that is hosted on a third-party cloud to Alibaba Cloud by using Database Gateway. When you migrate, synchronize, or subscribe to data by using Data Transmission Service \(DTS\), you can select the database that is connected to Alibaba Cloud through Database Gateway as the source or destination database.

An AccessKey pair is created. The AccessKey pair consists of an AccessKey ID and AccessKey secret. For more information, see [Create an AccessKey pair](https://www.alibabacloud.com/help/doc-detail/53045.htm).

You can connect an on-premises database or a database that is hosted on a third-party cloud to Alibaba Cloud by using one of the following methods:

-   Connect over Express Connect, VPN Gateway, or Smart Access Gateway: This method is not suitable for individual users because it requires high costs.
-   Connect to the service port of the database over the Internet: This method incurs potential security risks.
-   Forward service requests by using a user-created proxy: This method requires high costs and provides low stability.

In addition to the preceding methods, you can use Database Gateway to connect an on-premises database or a database that is hosted on a third-party cloud to Alibaba Cloud at a lower cost. For more information about the design concept of Database Gateway, see [How it works](https://www.alibabacloud.com/help/doc-detail/121986.htm).

## Precautions

Database Gateway is in public preview and is available only in the following regions: China \(Hangzhou\), Singapore \(Singapore\), Indonesia \(Jakarta\), UK \(London\), and US \(Virginia\).

## Billing

Database Gateway incurs no fees in public preview.

## Procedure

1.  Log on to the [Database Gateway console](https://dg.console.aliyun.com/).

    **Note:** If you are using Database Gateway for the first time, the **Enable Service** page appears. On this page, read and agree to the Database Gateway Service Agreement, and then click **Enable Now**.

2.  Click **Create Gateway**.

3.  In the Create Gateway dialog box, enter the name and description of the database gateway, and then click **Next step**.

4.  Download the gateway program.

    **Note:** The server that is used to deploy the gateway program must meet the following requirements:

    -   Performance: At least one CPU core and 1 GB memory are available. You can use higher-performance devices.
    -   Software environment: JRE 1.7 or later is installed. We recommend that you use a 64-bit operating system.
    -   Network:
        -   The server can connect to the target database. If the server and the database are deployed in the same internal network, the network latency is minimal.
        -   The server can access the Internet. The service port of the server does not need to be accessible over the Internet. To ensure the channel rate and stability, the outbound bandwidth must be at least 10 Mbit/s.
    1.  In the Create Gateway dialog box, download the gateway program for the target operating system based on the runtime environment.

        ![Download the gateway program](https://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/en-US/3623097951/p97926.png)

    2.  Copy the downloaded installation file to the server where you want to deploy the gateway program, and decompress the file.

5.  Start the gateway program.

    1.  Log on to the server where the gateway program is deployed, and go to the directory where the gateway program is decompressed.

    2.  Select one of the following methods to start the gateway program based on your operating system:

        -   For Linux or Mac, run the `bin/start.bat` command.
        -   For Windows, double-click the db\_agent.bat file in the bin directory.
    3.  Enter the AccessKey ID and AccessKey secret.

        ![Install Database Gateway](https://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/en-US/3623097951/p97928.png)

    4.  After the verification is successful, return to the Database Gateway console and click **Next step** to obtain a random verification code.

        ![Obtain a verification code](https://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/en-US/3623097951/p97931.png)

    5.  Enter the verification code in the CLI of the gateway program and press the Enter key. Wait until the connection is established.

        ![Start Database Gateway](https://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/en-US/3623097951/p97932.png)

6.  Add a database.

    **Note:** You can repeat this step to add multiple databases.

    1.  Return to the Database Gateway console and click **Add database**.

    2.  In the dialog box that appears, specify the database address, service port number, and description, and then click **OK**.

        ![Add a database](https://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/en-US/3623097951/p97933.png)


When you configure data migration, data synchronization, or change tracking, select **Database without public IP:Port \(Accessed through database gateway\)** as the instance type. Select the database address from the drop-down list. You can select the database that is connected over Database Gateway as the source database or destination database.

**Note:** If you select **Database without public IP:Port \(Accessed through database gateway\)** as the instance type when you configure data migration, the source and destination instances must reside in the same region.

![Select an instance type](https://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/en-US/3623097951/p97936.png)

