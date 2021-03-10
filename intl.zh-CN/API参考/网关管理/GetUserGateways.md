# GetUserGateways

调用GetUserGateways获取网关列表。

## 调试

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=dg&api=GetUserGateways&type=RPC&version=2019-03-27)

## 请求参数

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|GetUserGateways|系统规定参数。取值：GetUserGateways。 |
|PageSize|Integer|否|20|分页大小，大小不要超过3000。 |
|PageNumber|Integer|否|1|页数，从1开始。 |
|SearchKey|String|否|test|按照名称或者备注模糊查询。 |

## 返回数据

|名称|类型|示例值|描述|
|--|--|---|--|
|Code|String|200|响应码。 |
|Count|Integer|50|总条数。 |
|Data|String|\[\{\\"gatewayDesc\\":\\"i-11x8wqo6w\\",\\"gatewayId\\":\\"dg-c5n5913zl54f7h7z\\",\\"gatewayName\\":\\"TestLinux\\",\\"gmtCreate\\":1563430627000,\\"gmtCreateString\\":\\"2019-07-18 14:17\\",\\"gmtModified\\":1568881049000,\\"gmtModifiedString\\":\\"2019-09-19 16:17\\",\\"hosts\\":\\"10.\*.\*.78\\",\\"parentId\\":\\"1673826650152166\\",\\"status\\":\\"RUNNING\\",\\"userId\\":\\"1673826650152166\\"\}\]|网关信息。 |
|ErrorMsg|String|String|异常信息。 |
|RequestId|String|E68F1794-354B-4F18-AA6D-1F00353E632E|请求ID。 |
|Success|Boolean|true|成功标识。 |

## 示例

请求示例

```
http(s)://[Endpoint]/?Action=GetUserGateways
&<公共请求参数>
```

正常返回示例

`XML`格式

```
<RequestId>E68F1794-354B-4F18-AA6D-1F00353E632E</RequestId>
<ErrorMsg>String</ErrorMsg>
<Data>[{\"gatewayDesc\":\"i-11x8wqo6w\",\"gatewayId\":\"dg-c5n5913zl54f7h7z\",\"gatewayName\":\"TestLinux\",\"gmtCreate\":1563430627000,\"gmtCreateString\":\"2019-07-18 14:17\",\"gmtModified\":1568881049000,\"gmtModifiedString\":\"2019-09-19 16:17\",\"hosts\":\"10.*.*.78\",\"parentId\":\"1673826650152166\",\"status\":\"RUNNING\",\"userId\":\"1673826650152166\"}]</Data>
<Count>50</Count>
<Code>200</Code>
<Success>true</Success>
```

`JSON`格式

```
{"RequestId":"E68F1794-354B-4F18-AA6D-1F00353E632E","ErrorMsg":"String","Data":"[{\\\"gatewayDesc\\\":\\\"i-11x8wqo6w\\\",\\\"gatewayId\\\":\\\"dg-c5n5913zl54f7h7z\\\",\\\"gatewayName\\\":\\\"TestLinux\\\",\\\"gmtCreate\\\":1563430627000,\\\"gmtCreateString\\\":\\\"2019-07-18 14:17\\\",\\\"gmtModified\\\":1568881049000,\\\"gmtModifiedString\\\":\\\"2019-09-19 16:17\\\",\\\"hosts\\\":\\\"10.*.*.78\\\",\\\"parentId\\\":\\\"1673826650152166\\\",\\\"status\\\":\\\"RUNNING\\\",\\\"userId\\\":\\\"1673826650152166\\\"}]","Count":"50","Code":"200","Success":"true"}
```

## 错误码

访问[错误中心](https://error-center.alibabacloud.com/status/product/dg)查看更多错误码。

