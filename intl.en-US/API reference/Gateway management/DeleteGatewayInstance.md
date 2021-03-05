# DeleteGatewayInstance

Deletes a database gateway node.

## Debugging

[OpenAPI Explorer automatically calculates the signature value. For your convenience, we recommend that you call this operation in OpenAPI Explorer. OpenAPI Explorer dynamically generates the sample code of the operation for different SDKs.](https://api.aliyun.com/#product=dg&api=DeleteGatewayInstance&type=RPC&version=2019-03-27)

## Request parameters

|Parameter|Type|Required|Example|Description|
|---------|----|--------|-------|-----------|
|Action|String|Yes|DeleteGatewayInstance|The operation that you want to perform. Set the value to DeleteGatewayInstance. |
|GatewayId|String|Yes|dg-123|The ID of the gateway. |
|GatewayInstanceId|String|Yes|dg-node-123|The ID of the gateway node. |
|RegionId|String|Yes|cn-hangzhou|The ID of the region. |

## Response parameters

|Parameter|Type|Example|Description|
|---------|----|-------|-----------|
|Code|String|200|The HTTP status code. |
|Data|String|SUCCESS|The response data. |
|ErrorMsg|String|Error|The error message. |
|RequestId|String|41916DEB-F62D-41FA-AB53-FC61D795BC66|The ID of the request. |
|Success|Boolean|true|Indicates whether the call is successful. |

## Examples

Sample requests

```
http(s)://[Endpoint]/? Action=DeleteGatewayInstance
&GatewayId=dg-123
&GatewayInstanceId=dg-node-123
&RegionId=cn-hangzhou
&<Common request parameters>
```

Sample responses

`XML` format

```
<RequestId>41916DEB-F62D-41FA-AB53-FC61D795BC66</RequestId>
<ErrorMsg>Error</ErrorMsg>
<Data>SUCCESS</Data>
<Code>200</Code>
<Success>true</Success>
```

`JSON` format

```
{"RequestId":"41916DEB-F62D-41FA-AB53-FC61D795BC66","ErrorMsg":"Error","Data":"SUCCESS","Code":"200","Success":"true"}
```

## Error codes

For a list of error codes, visit the [API Error Center](https://error-center.alibabacloud.com/status/product/dg).

