# 使用高速通道/VPN网关/CEN接入数据库网关

## 背景信息

高速通道使用物理专线连接实现云下IDC专线接入云上，需要在数据库上配置可访问数据库的白名单。当IDC内部数据库想要接入云上产品（如DMS，DTS，DBS等）则需要将云上产品的网段添加到数据库的白名单中。当出现网段变更，则需要同步更改数据库白名单配置，运维成本比较高。

通过数据库网关可以减少数据库白名单的配置，仅需要将本地安装的DG Agent配置到数据库白名单即可使用。当云上产品发生网段变化，也不需要同步变更数据库白名单配置。同时使用高速通道接入时，DG会复用原有专线链路，相比于公网接入方式会有更强的网络质量。

![图片](https://static-aliyun-doc.oss-accelerate.aliyuncs.com/assets/img/zh-CN/8576330061/p167479.png)

## 前提条件

1.  您已经开通阿里云数据库网关服务，详情请参见[准备工作](/intl.zh-CN/用户指南/准备工作.md)。
2.  您已配置高速通道/VPN网关/CEN。

## 操作步骤

1.  在新建数据网关时，勾选**使用已有专线/云企业网/VPN网关接入**，如何新建数据库网关请参见[新建数据库网关](/intl.zh-CN/用户指南/新建数据库网关.md)。

    ![tp](https://static-aliyun-doc.oss-accelerate.aliyuncs.com/assets/img/zh-CN/8576330061/p167407.png)

2.  输入IDC内目标数据库的主机和端口号添加数据库，然后单击**完成**。

    ![图片](https://static-aliyun-doc.oss-accelerate.aliyuncs.com/assets/img/zh-CN/8576330061/p167410.png)


