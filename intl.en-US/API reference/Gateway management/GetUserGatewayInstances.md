# GetUserGatewayInstances

Queries the details of a gateway node.

## Debugging

[OpenAPI Explorer automatically calculates the signature value. For your convenience, we recommend that you call this operation in OpenAPI Explorer. OpenAPI Explorer dynamically generates the sample code of the operation for different SDKs.](https://api.aliyun.com/#product=dg&api=GetUserGatewayInstances&type=RPC&version=2019-03-27)

## Request parameters

|Parameter|Type|Required|Example|Description|
|---------|----|--------|-------|-----------|
|Action|String|Yes|GetUserGatewayInstances|The operation that you want to perform. Set the value to GetUserGatewayInstances. |
|GatewayId|String|Yes|dg-123|The ID of the gateway. |

## Response parameters

|Parameter|Type|Example|Description|
|---------|----|-------|-----------|
|Code|String|200|The HTTP status code. |
|Data|String|\{"RequestId":"8AE40251-3041-4458-95BB-68DE17BDABB6","ErrorMsg":"","Data":"\[\{\\"connectEndpointType\\":\\"INTERNET\\",\\"currentDaemonVersion\\":\\"3.0\\",\\"currentVersion\\":\\"3.0\\",\\"endPoint\\":\\"pub-cn-hangzhou.dg.aliyuncs.com\\",\\"gatewayId\\":\\"dg-123\\",\\"gatewayInstanceId\\":\\"dg-node-123\\",\\"gatewayInstanceStatus\\":\\"RUNNING\\",\\"lastUpdateTime\\":\\"1611232930000\\",\\"localIP\\":\\"172.16.144.173\\",\\"message\\":\\"\\",\\"outputIP\\":\\"172.16.144.173\\"\}\]","Code":"","Success":true\}|The response data. |
|ErrorMsg|String|Error|The error message. |
|RequestId|String|8AE40251-3041-4458-95BB-68DE17BDABB6|The ID of the request. |
|Success|Boolean|true|Indicates whether the call is successful. |

## Examples

Sample requests

```
http(s)://[Endpoint]/? Action=GetUserGatewayInstances
&GatewayId=dg-123
&<Common request parameters>
```

Sample responses

`XML` format

```
<RequestId>8AE40251-3041-4458-95BB-68DE17BDABB6</RequestId>
<ErrorMsg>Error</ErrorMsg>
<Data>{"RequestId":"8AE40251-3041-4458-95BB-68DE17BDABB6","ErrorMsg":"","Data":"[{\"connectEndpointType\":\"INTERNET\",\"currentDaemonVersion\":\"3.0\",\"currentVersion\":\"3.0\",\"endPoint\":\"pub-cn-hangzhou.dg.aliyuncs.com\",\"gatewayId\":\"dg-123\",\"gatewayInstanceId\":\"dg-node-123\",\"gatewayInstanceStatus\":\"RUNNING\",\"lastUpdateTime\":\"1611232930000\",\"localIP\":\"172.16.144.173\",\"message\":\"\",\"outputIP\":\"172.16.144.173\"}]","Code":"","Success":true}</Data>
<Code>200</Code>
<Success>true</Success>
```

`JSON` format

```
{"RequestId":"8AE40251-3041-4458-95BB-68DE17BDABB6","ErrorMsg":"Error","Data":"{\"RequestId\":\"8AE40251-3041-4458-95BB-68DE17BDABB6\",\"ErrorMsg\":\"\",\"Data\":\"[{\\\"connectEndpointType\\\":\\\"INTERNET\\\",\\\"currentDaemonVersion\\\":\\\"3.0\\\",\\\"currentVersion\\\":\\\"3.0\\\",\\\"endPoint\\\":\\\"pub-cn-hangzhou.dg.aliyuncs.com\\\",\\\"gatewayId\\\":\\\"dg-123\\\",\\\"gatewayInstanceId\\\":\\\"dg-node-123\\\",\\\"gatewayInstanceStatus\\\":\\\"RUNNING\\\",\\\"lastUpdateTime\\\":\\\"1611232930000\\\",\\\"localIP\\\":\\\"172.16.144.173\\\",\\\"message\\\":\\\"\\\",\\\"outputIP\\\":\\\"172.16.144.173\\\"}]\",\"Code\":\"\",\"Success\":true}","Code":"200","Success":"true"}
```

## Error codes

For a list of error codes, visit the [API Error Center](https://error-center.alibabacloud.com/status/product/dg).

