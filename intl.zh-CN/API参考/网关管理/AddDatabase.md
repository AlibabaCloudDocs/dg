# AddDatabase

调用AddDatabase添加数据库。

## 调试

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=dg&api=AddDatabase&type=RPC&version=2019-03-27)

## 请求参数

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|AddDatabase|系统规定参数。取值：**AddDatabase**。 |
|DbPassword|String|是|password|访问数据库所用的密码。

 **说明：** 仅用于验证数据库是否可以连接成功，不做任何其他工作。 |
|DbType|String|是|MySQL|数据库类型。

 **说明：** 目前数据库类型仅支持MySQL。 |
|DbUserName|String|是|dg\_test|访问数据库所用的用户名。 |
|GatewayId|String|是|dg-yhss6sdla\*\*\*\*|网关ID。 |
|Host|String|是|11.\*.\*.109|通过网关所在宿主机去访问数据库的地址。 |
|Port|Integer|是|3440|通过网关所在宿主机去访问数据库的端口。 |
|DbDescription|String|否|开发环境数据库|数据库的描述。 |

## 返回数据

|名称|类型|示例值|描述|
|--|--|---|--|
|Code|String|OK|响应码。 |
|Data|String|string|后端分配的实例ID。 |
|ErrorMsg|String|string|异常信息。 |
|RequestId|String|EAF2AA07-860D-43DA-BEE8-1E43AAE024CD|请求ID。 |
|Success|Boolean|true|是否成功。 |

## 示例

请求示例

```
http(s)://[Endpoint]/?Action=AddDatabase
&DbPassword=password
&DbType=MySQL
&DbUserName=dg_test
&GatewayId=dg-yhss6sdlaffaq68
&Host=11.*.*.109
&Port=3440
&<公共请求参数>
```

正常返回示例

`XML`格式

```
<RequestId>EAF2AA07-860D-43DA-BEE8-1E43AAE024CD</RequestId>
<ErrorMsg>string</ErrorMsg>
<Data>string</Data>
<Code>OK</Code>
<Success>true</Success>
```

`JSON`格式

```
{"RequestId":"EAF2AA07-860D-43DA-BEE8-1E43AAE024CD","ErrorMsg":"string","Data":"string","Code":"OK","Success":"true"}
```

## 错误码

访问[错误中心](https://error-center.alibabacloud.com/status/product/dg)查看更多错误码。

