# DeleteGatewayInstance

调用DeleteGatewayInstance删除数据库网关节点。

## 调试

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=dg&api=DeleteGatewayInstance&type=RPC&version=2019-03-27)

## 请求参数

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DeleteGatewayInstance|系统规定参数。取值：DeleteGatewayInstance。 |
|GatewayId|String|是|dg-123|网关ID。 |
|GatewayInstanceId|String|是|dg-node-123|网关实例ID。 |
|RegionId|String|是|cn-hangzhou|地域ID。 |

## 返回数据

|名称|类型|示例值|描述|
|--|--|---|--|
|Code|String|200|响应码。 |
|Data|String|SUCCESS|返回数据。 |
|ErrorMsg|String|Error|报错信息。 |
|RequestId|String|41916DEB-F62D-41FA-AB53-FC61D795BC66|请求ID。 |
|Success|Boolean|true|请求成功标识。 |

## 示例

请求示例

```
http(s)://[Endpoint]/?Action=DeleteGatewayInstance
&GatewayId=dg-123
&GatewayInstanceId=dg-node-123
&RegionId=cn-hangzhou
&<公共请求参数>
```

正常返回示例

`XML`格式

```
<RequestId>41916DEB-F62D-41FA-AB53-FC61D795BC66</RequestId>
<ErrorMsg>Error</ErrorMsg>
<Data>SUCCESS</Data>
<Code>200</Code>
<Success>true</Success>
```

`JSON`格式

```
{"RequestId":"41916DEB-F62D-41FA-AB53-FC61D795BC66","ErrorMsg":"Error","Data":"SUCCESS","Code":"200","Success":"true"}
```

## 错误码

访问[错误中心](https://error-center.alibabacloud.com/status/product/dg)查看更多错误码。

