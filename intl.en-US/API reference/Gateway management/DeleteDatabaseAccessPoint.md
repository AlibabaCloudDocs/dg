# DeleteDatabaseAccessPoint

Deletes a database access point.

## Debugging

[OpenAPI Explorer automatically calculates the signature value. For your convenience, we recommend that you call this operation in OpenAPI Explorer. OpenAPI Explorer dynamically generates the sample code of the operation for different SDKs.](https://api.aliyun.com/#product=dg&api=DeleteDatabaseAccessPoint&type=RPC&version=2019-03-27)

## Request parameters

|Parameter|Type|Required|Example|Description|
|---------|----|--------|-------|-----------|
|Action|String|Yes|DeleteDatabaseAccessPoint|The operation that you want to perform. Set the value to DeleteDatabaseAccessPoint. |
|DbInstanceId|String|Yes|dg-db-abcd123|The ID of the instance. |
|VpcAZone|String|Yes|cn-hangzhou-i|The zone to which the VPC belongs. |
|VpcId|String|Yes|vpc-123abcd|The ID of the VPC. |
|VpcRegionId|String|Yes|cn-hangzhou|The region ID of the VPC. |
|VSwitchId|String|Yes|vsw-123abcd|The ID of the vSwitch. |
|RegionId|String|No|cn-hangzhou|The ID of the region. |

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
http(s)://[Endpoint]/? Action=DeleteDatabaseAccessPoint
&DbInstanceId=dg-db-abcd123
&VpcAZone=cn-hangzhou-i
&VpcId=vpc-123abcd
&VpcRegionId=cn-hangzhou
&VSwitchId=vsw-123abcd
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

|HttpCode|Error code|Error message|Description|
|--------|----------|-------------|-----------|
|500|Error|The requested service is unavailable. Please try again later.|The error message returned because a service exception occurred. Try again.|

For a list of error codes, visit the [API Error Center](https://error-center.alibabacloud.com/status/product/dg).

