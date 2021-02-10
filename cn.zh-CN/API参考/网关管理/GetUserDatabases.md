# GetUserDatabases

调用GetUserDatabases返回用户数据库列表信息。

## 调试

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=dg&api=GetUserDatabases&type=RPC&version=2019-03-27)

## 请求参数

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|GetUserDatabases|系统规定参数。取值：**GetUserDatabases**。 |
|PageNumber|String|是|1|当前页码。 |
|PageSize|String|是|10|分页大小。 |
|GatewayId|String|否|dg-yhss6sdlaff\*\*\*\*|网关ID。 |
|SearchKey|String|否|网关|搜索关键字。 |
|DbType|String|否|MySQL|数据库类型。

 **说明：** 目前数据库类型仅支持MySQL。 |

## 返回数据

|名称|类型|示例值|描述|
|--|--|---|--|
|Code|String|OK|响应码。 |
|Count|Integer|1|个数。 |
|Data|String|\[\{\\ “dbDescription\\” :\\“开发环境数据库\\” ,\\“dbType\\” :\\“MySQL\\” ,\\“dbUserName\\” :\\“dbatool\\” ,\\“gatewayId\\” :\\ “test\_gateway\\” ,\\“gatewayName\\” :\\“Gateway—1\\” ,\\“gmtCreate\\” :1560736969000,\\“gmtCreateString\\” :\\“2019-06-17 10:02\\” ,\\“host\\” :\\“11.163.23.109\\” ,\\“instanceId\\” :\\“instance\_1\\” ,\\“parentId\\” :\\“1344371\\” ,\\“port\\” :3440,\\“userId\\” :\\“1344371\\” \}\]|数据库列表信息。 |
|ErrorMsg|String|无|异常信息。 |
|RequestId|String|951AE6AA-BFC5-4DD8-8CD6-DFD3D51E4170|请求ID。 |
|Success|String|true|是否成功。 |

## 示例

请求示例

```
http(s)://dg.[regionId].aliyuncs.com/?Action=GetUserDatabases
&PageNumber=1
&PageSize=10
&<公共请求参数>
```

正常返回示例

`XML`格式

```
<RequestId>951AE6AA-BFC5-4DD8-8CD6-DFD3D51E4170</RequestId>
<ErrorMsg>无</ErrorMsg>
<Data>[{\ “dbDescription\” :\“开发环境数据库\” ,\“dbType\” :\“MySQL\” ,\“dbUserName\” :\“dbatool\” ,\“gatewayId\” :\ “test_gateway\” ,\“gatewayName\” :\“Gateway—1\” ,\“gmtCreate\” :1560736969000,\“gmtCreateString\” :\“2019-06-17 10:02\” ,\“host\” :\“11.163.23.109\” ,\“instanceId\” :\“instance_1\” ,\“parentId\” :\“1344371\” ,\“port\” :3440,\“userId\” :\“1344371\” }]</Data>
<Count>1</Count>
<Code>OK</Code>
<Success>true</Success>
```

`JSON`格式

```
{"RequestId":"951AE6AA-BFC5-4DD8-8CD6-DFD3D51E4170","ErrorMsg":"无","Data":"[{\\ “dbDescription\\” :\\“开发环境数据库\\” ,\\“dbType\\” :\\“MySQL\\” ,\\“dbUserName\\” :\\“dbatool\\” ,\\“gatewayId\\” :\\ “test_gateway\\” ,\\“gatewayName\\” :\\“Gateway—1\\” ,\\“gmtCreate\\” :1560736969000,\\“gmtCreateString\\” :\\“2019-06-17 10:02\\” ,\\“host\\” :\\“11.163.23.109\\” ,\\“instanceId\\” :\\“instance_1\\” ,\\“parentId\\” :\\“1344371\\” ,\\“port\\” :3440,\\“userId\\” :\\“1344371\\” }]","Count":"1","Code":"OK","Success":"true"}
```

## 错误码

访问[错误中心](https://error-center.aliyun.com/status/product/dg)查看更多错误码。

