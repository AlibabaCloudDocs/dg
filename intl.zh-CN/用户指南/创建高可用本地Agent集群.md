# 创建高可用本地Agent集群

## 背景信息

数据库网关（DG）支持云下部署DG Agent高可用集群，您可以通过在云下不同机器上分别部署DG Agent应用程序，不同DG Agent会自动组成高可用集群，增强链路可靠性。当部分DG Agent不可用时，DG Server将会自动将链路切换到可用的DG Agent上，以达到高可用的特性。

![图片](https://static-aliyun-doc.oss-accelerate.aliyuncs.com/assets/img/zh-CN/7376330061/p167489.png)

## 前提条件

您已经开通数据库网关服务，并且成功启动一个DG Agent，详情请参见[新建数据库网关](/intl.zh-CN/用户指南/新建数据库网关.md)。

## 操作步骤

1.  登录[数据库网关控制台](https://dg.console.aliyun.com/gateway)。
2.  在左侧导航栏单击**网关列表**。
3.  在选择添加高可用节点网关的右侧单击**详情**。

    ![图片](https://static-aliyun-doc.oss-accelerate.aliyuncs.com/assets/img/zh-CN/8376330061/p167356.png)

4.  在网关详情页面单击**添加网关节点**。

    ![图片](https://static-aliyun-doc.oss-accelerate.aliyuncs.com/assets/img/zh-CN/8376330061/p167357.png)

5.  您可以根据操作系统类型，选择不同的安装方式。Windows系统直接点击**下载安装包**，其他操作系统直接复制命令行到需要添加网关节点的机器上，回车执行即可。**注意：每个部署命令仅可以启动一个agent，若需要启动多个agent，可以点击刷新更新部署链接。**

    ![tp](https://static-aliyun-doc.oss-accelerate.aliyuncs.com/assets/img/zh-CN/4825287951/p139203.png)

6.  添加成功后可以在网关详情页面查看网关节点信息。

    ![图片](https://static-aliyun-doc.oss-accelerate.aliyuncs.com/assets/img/zh-CN/8376330061/p167490.png)


