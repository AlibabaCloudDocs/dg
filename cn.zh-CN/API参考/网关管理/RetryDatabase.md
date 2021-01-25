# RetryDatabase

调用RetryDatabase接口重试数据库。

## 调试

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=dg&api=RetryDatabase&type=RPC&version=2019-03-27)

## 请求参数

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|RetryDatabase|系统规定参数。取值：RetryDatabase。 |
|DbPassword|String|是|123|数据库密码。 |
|DbType|String|是|MySQL|数据库类型。 |
|DbUserName|String|是|abcd|数据库用户名。 |
|GatewayId|String|是|dg-yhss6sdlaff\*\*\*\*|网关ID。 |
|Host|String|是|127.0.0.1|主机地址。 |
|Port|Integer|是|3306|端口号。 |
|RegionId|String|是|cn-hangzhou|地域ID。 |
|DbDescription|String|否|123|描述信息。 |
|DbName|String|否|abcd|数据库名称。 |
|ClientToken|String|否|123|Token。 |

## 返回数据

|名称|类型|示例值|描述|
|--|--|---|--|
|Code|String|200|响应码。 |
|Data|String|SUCCESS|返回结果。 |
|ErrorMsg|String|Error|异常信息。 |
|RequestId|String|CDDAAA07-D806-AG67-BEE8-1E43AAE024DD|请求ID。 |
|Success|Boolean|true|是否成功。 |

## 示例

请求示例

```
http(s)://[Endpoint]/?Action=RetryDatabase
&DbPassword=123
&DbType=MySQL
&DbUserName=abcd
&GatewayId=dg-yhss6sdlaff****
&Host=127.0.0.1
&Port=3306
&RegionId=cn-hangzhou
&<公共请求参数>
```

正常返回示例

`XML`格式

```
<RequestId>CDDAAA07-D806-AG67-BEE8-1E43AAE024DD</RequestId>
<ErrorMsg>Error</ErrorMsg>
<Data>SUCCESS</Data>
<Code>200</Code>
<Success>true</Success>
```

`JSON`格式

```
{"RequestId":"CDDAAA07-D806-AG67-BEE8-1E43AAE024DD","ErrorMsg":"Error","Data":"SUCCESS","Code":"200","Success":"true"}
```

## 错误码

|HttpCode|错误码|错误信息|描述|
|--------|---|----|--|
|500|Error|The requested service is unavailable. Please try again later.|服务异常，请重试|

访问[错误中心](https://error-center.aliyun.com/status/product/dg)查看更多错误码。

