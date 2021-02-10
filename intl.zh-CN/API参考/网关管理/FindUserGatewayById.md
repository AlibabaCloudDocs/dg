# FindUserGatewayById

调用FindUserGatewayById根据网关ID获取网关详细信息。

## 调试

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=dg&api=FindUserGatewayById&type=RPC&version=2019-03-27)

## 请求参数

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|FindUserGatewayById|系统规定参数。取值：FindUserGatewayById。 |
|GatewayId|String|是|dg-yhss6sdlaff\*\*\*\*|网关ID |

## 返回数据

|名称|类型|示例值|描述|
|--|--|---|--|
|Code|String|200|响应码 |
|Data|String|\{\\“gatewayDesc\\”:\\ “阿里数据库网关\\”,\\“gatewayId\\”:\\“dg-c34g913zl54f7h7z\\”,\\“gatewayName\\”:\\“生产环境\\”,\\“gmtCreate\\”:1563430627000,\\“gmtCreateString\\”:\\“2019-07-18 14:17\\”,\\“gmtModified\\”:1568881049000,\\“gmtModifiedString\\”:\\“2019-09-19 16:17\\”,\\“hosts\\":\\"10.25.37.78\\”,\\“parentId\\”:\\“123123\\”,\\“status\\”:\\“RUNNING\\”,\\“userId\\”:\\“123123\\”,\\“regionId\\”:\\“cn-hangzhou\\”\}|网关详细信息 |
|ErrorMsg|String|""|错误信息 |
|RequestId|String|31728E14-8164-49C3-928B-044E93B8A11E|请求ID |
|Success|Boolean|true|成功标识 |

## 示例

请求示例

```
http(s)://[Endpoint]/?Action=FindUserGatewayById
&GatewayId=dg-yhss6sdlaff****
&<公共请求参数>
```

正常返回示例

`XML`格式

```
<RequestId>31728E14-8164-49C3-928B-044E93B8A11E</RequestId>
<ErrorMsg>""</ErrorMsg>
<Data>{\“gatewayDesc\”:\ “阿里数据库网关\”,\“gatewayId\”:\“dg-c34g913zl54f7h7z\”,\“gatewayName\”:\“生产环境\”,\“gmtCreate\”:1563430627000,\“gmtCreateString\”:\“2019-07-18 14:17\”,\“gmtModified\”:1568881049000,\“gmtModifiedString\”:\“2019-09-19 16:17\”,\“hosts\":\"10.25.37.78\”,\“parentId\”:\“123123\”,\“status\”:\“RUNNING\”,\“userId\”:\“123123\”,\“regionId\”:\“cn-hangzhou\”} </Data>
<Code>200</Code>
<Success>true</Success>
```

`JSON`格式

```
{"RequestId":"31728E14-8164-49C3-928B-044E93B8A11E","ErrorMsg":"\"\"","Data":"{\\“gatewayDesc\\”:\\ “阿里数据库网关\\”,\\“gatewayId\\”:\\“dg-c34g913zl54f7h7z\\”,\\“gatewayName\\”:\\“生产环境\\”,\\“gmtCreate\\”:1563430627000,\\“gmtCreateString\\”:\\“2019-07-18 14:17\\”,\\“gmtModified\\”:1568881049000,\\“gmtModifiedString\\”:\\“2019-09-19 16:17\\”,\\“hosts\\\":\\\"10.25.37.78\\”,\\“parentId\\”:\\“123123\\”,\\“status\\”:\\“RUNNING\\”,\\“userId\\”:\\“123123\\”,\\“regionId\\”:\\“cn-hangzhou\\”} ","Code":"200","Success":"true"}
```

## 错误码

访问[错误中心](https://error-center.alibabacloud.com/status/product/dg)查看更多错误码。

