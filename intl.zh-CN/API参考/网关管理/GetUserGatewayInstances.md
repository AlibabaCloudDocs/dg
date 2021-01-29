# GetUserGatewayInstances

调用GetUserGatewayInstances获取网关节点详情。

## 调试

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=dg&api=GetUserGatewayInstances&type=RPC&version=2019-03-27)

## 请求参数

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|GetUserGatewayInstances|系统规定参数。取值：GetUserGatewayInstances。 |
|GatewayId|String|是|dg-123|网关ID。 |

## 返回数据

|名称|类型|示例值|描述|
|--|--|---|--|
|Code|String|200|响应码。 |
|Data|String|\{"RequestId":"8AE40251-3041-4458-95BB-68DE17BDABB6","ErrorMsg":"","Data":"\[\{\\"connectEndpointType\\":\\"INTERNET\\",\\"currentDaemonVersion\\":\\"3.0\\",\\"currentVersion\\":\\"3.0\\",\\"endPoint\\":\\"pub-cn-hangzhou.dg.aliyuncs.com\\",\\"gatewayId\\":\\"dg-123\\",\\"gatewayInstanceId\\":\\"dg-node-123\\",\\"gatewayInstanceStatus\\":\\"RUNNING\\",\\"lastUpdateTime\\":\\"1611232930000\\",\\"localIP\\":\\"172.16.144.173\\",\\"message\\":\\"\\",\\"outputIP\\":\\"172.16.144.173\\"\}\]","Code":"","Success":true\}|返回数据。 |
|ErrorMsg|String|Error|错误信息。 |
|RequestId|String|8AE40251-3041-4458-95BB-68DE17BDABB6|请求ID。 |
|Success|Boolean|true|请求成功标识。 |

## 示例

请求示例

```
http(s)://[Endpoint]/?Action=GetUserGatewayInstances
&GatewayId=dg-123
&<公共请求参数>
```

正常返回示例

`XML`格式

```
<RequestId>8AE40251-3041-4458-95BB-68DE17BDABB6</RequestId>
<ErrorMsg>Error</ErrorMsg>
<Data>{"RequestId":"8AE40251-3041-4458-95BB-68DE17BDABB6","ErrorMsg":"","Data":"[{\"connectEndpointType\":\"INTERNET\",\"currentDaemonVersion\":\"3.0\",\"currentVersion\":\"3.0\",\"endPoint\":\"pub-cn-hangzhou.dg.aliyuncs.com\",\"gatewayId\":\"dg-123\",\"gatewayInstanceId\":\"dg-node-123\",\"gatewayInstanceStatus\":\"RUNNING\",\"lastUpdateTime\":\"1611232930000\",\"localIP\":\"172.16.144.173\",\"message\":\"\",\"outputIP\":\"172.16.144.173\"}]","Code":"","Success":true}</Data>
<Code>200</Code>
<Success>true</Success>
```

`JSON`格式

```
{"RequestId":"8AE40251-3041-4458-95BB-68DE17BDABB6","ErrorMsg":"Error","Data":"{\"RequestId\":\"8AE40251-3041-4458-95BB-68DE17BDABB6\",\"ErrorMsg\":\"\",\"Data\":\"[{\\\"connectEndpointType\\\":\\\"INTERNET\\\",\\\"currentDaemonVersion\\\":\\\"3.0\\\",\\\"currentVersion\\\":\\\"3.0\\\",\\\"endPoint\\\":\\\"pub-cn-hangzhou.dg.aliyuncs.com\\\",\\\"gatewayId\\\":\\\"dg-123\\\",\\\"gatewayInstanceId\\\":\\\"dg-node-123\\\",\\\"gatewayInstanceStatus\\\":\\\"RUNNING\\\",\\\"lastUpdateTime\\\":\\\"1611232930000\\\",\\\"localIP\\\":\\\"172.16.144.173\\\",\\\"message\\\":\\\"\\\",\\\"outputIP\\\":\\\"172.16.144.173\\\"}]\",\"Code\":\"\",\"Success\":true}","Code":"200","Success":"true"}
```

## 错误码

访问[错误中心](https://error-center.alibabacloud.com/status/product/dg)查看更多错误码。

