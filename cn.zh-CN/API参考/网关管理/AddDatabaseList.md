# AddDatabaseList

调用AddDatabaseList批量添加数据库。

## 调试

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=dg&api=AddDatabaseList&type=RPC&version=2019-03-27)

## 请求参数

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|AddDatabaseList|系统规定参数。取值：AddDatabaseList。 |
|DatabaseString|String|是|\[\{"host":"127.0.0.1","port":"3306","gatewayId":"dg-xsdasdasdasdasd"\}\]|需添加数据库的信息。 |
|ClientToken|String|否|ETnLKlblzczshOTUbOCzxxxx|用于保证请求的幂等性。由客户端生成该参数值，要保证在不同请求间唯一，大小写敏感、不超过64个ASCII字符。 |

## 返回数据

|名称|类型|示例值|描述|
|--|--|---|--|
|Code|String|200|响应码。 |
|Data|String|SUCCESS|返回数据。 |
|ErrorMsg|String|Error|报错信息。 |
|RequestId|String|ABCD-1234|请求ID。 |
|Success|Boolean|true|请求成功标识。 |

## 示例

请求示例

```
http(s)://[Endpoint]/?Action=AddDatabaseList
&DatabaseString=[{"host":"127.0.0.1","port":"3306","gatewayId":"dg-xsdasdasdasdasd"}]
&<公共请求参数>
```

正常返回示例

`XML`格式

```
<RequestId>ABCD-1234</RequestId>
<ErrorMsg>Error</ErrorMsg>
<Data>SUCCESS</Data>
<Code>200</Code>
<Success>true</Success>
```

`JSON`格式

```
{"RequestId":"ABCD-1234","ErrorMsg":"Error","Data":"SUCCESS","Code":"200","Success":"true"}
```

## 错误码

|HttpCode|错误码|错误信息|描述|
|--------|---|----|--|
|500|Error|The requested service is unavailable. Please try again later.|服务异常，请重试|

访问[错误中心](https://error-center.aliyun.com/status/product/dg)查看更多错误码。

