# CreateDatabaseAccessPoint

Creates a database access point.

## Debugging

[OpenAPI Explorer automatically calculates the signature value. For your convenience, we recommend that you call this operation in OpenAPI Explorer. OpenAPI Explorer dynamically generates the sample code of the operation for different SDKs.](https://api.aliyun.com/#product=dg&api=CreateDatabaseAccessPoint&type=RPC&version=2019-03-27)

## Request parameters

|Parameter|Type|Required|Example|Description|
|---------|----|--------|-------|-----------|
|Action|String|Yes|CreateDatabaseAccessPoint|The operation that you want to perform. Set the value to CreateDatabaseAccessPoint. |
|DbInstanceId|String|Yes|dg-db-abcd1234|The ID of the instance. |
|VpcAZone|String|Yes|cn-hangzhou-i|The zone to which the VPC belongs. |
|VpcId|String|Yes|vpc-123abcd|The ID of the VPC. |
|VpcRegionId|String|Yes|cn-hangzhou|The region ID of the VPC. |
|VSwitchId|String|Yes|vsw-123abcd|The ID of the vSwitch. |
|RegionId|String|No|cn-hangzhou|The ID of the region. |
|ClientToken|String|No|ETnLKlblzczshOTUbOCzxxxx|The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must ensure that it is unique among different requests. The token is case-sensitive and can contain only ASCII characters. The token must be 1 to 64 characters in length. |

## Response parameters

|Parameter|Type|Example|Description|
|---------|----|-------|-----------|
|Code|String|200|The HTTP status code. |
|Data|String|\{"RequestId":"41916DEB-F62D-41FA-AB53-FC61D795BC66","ErrorMsg":"","Data":"\[\{\\"accessAddr\\":\\"172.16.144.216\\",\\"accessPort\\":3306,\\"dbInstanceId\\":\\"dg-db-abcd123\\",\\"gmtCreate\\":1609906765000,\\"gmtModified\\":1609906765000,\\"routerId\\":\\"cn-hangzhou\\",\\"vpcAzoneId\\":\\"cn-hangzhou-i\\",\\"vpcId\\":\\"vpc-123abcd\\",\\"vswitchId\\":\\"vsw-123abcd\\"\}\]","Count":1,"Code":"","Success":true\}|The response data. |
|ErrorMsg|String|Error|The error message. |
|RequestId|String|41916DEB-F62D-41FA-AB53-FC61D795BC66|The ID of the request. |
|Success|Boolean|true|Indicates whether the call is successful. |

## Examples

Sample requests

```
http(s)://[Endpoint]/? Action=CreateDatabaseAccessPoint
&DbInstanceId=dg-db-abcd1234
&VpcAZone=cn-hangzhou-a
&VpcId=vpc-123abcd
&VpcRegionId=cn-hangzhou
&VSwitchId=vswitch-123abcd
&<Common request parameters>
```

Sample responses

`XML` format

```
<RequestId>41916DEB-F62D-41FA-AB53-FC61D795BC66</RequestId>
<ErrorMsg>Error</ErrorMsg>
<Data>{"RequestId":"41916DEB-F62D-41FA-AB53-FC61D795BC66","ErrorMsg":"","Data":"[{\"accessAddr\":\"172.16.144.216\",\"accessPort\":3306,\"dbInstanceId\":\"dg-db-abcd123\",\"gmtCreate\":1609906765000,\"gmtModified\":1609906765000,\"routerId\":\"cn-hangzhou\",\"vpcAzoneId\":\"cn-hangzhou-i\",\"vpcId\":\"vpc-123abcd\",\"vswitchId\":\"vsw-123abcd\"}]","Count":1,"Code":"","Success":true}</Data>
<Code>200</Code>
<Success>true</Success>
```

`JSON` format

```
{"RequestId":"41916DEB-F62D-41FA-AB53-FC61D795BC66","ErrorMsg":"Error","Data":"{\"RequestId\":\"41916DEB-F62D-41FA-AB53-FC61D795BC66\",\"ErrorMsg\":\"\",\"Data\":\"[{\\\"accessAddr\\\":\\\"172.16.144.216\\\",\\\"accessPort\\\":3306,\\\"dbInstanceId\\\":\\\"dg-db-abcd123\\\",\\\"gmtCreate\\\":1609906765000,\\\"gmtModified\\\":1609906765000,\\\"routerId\\\":\\\"cn-hangzhou\\\",\\\"vpcAzoneId\\\":\\\"cn-hangzhou-i\\\",\\\"vpcId\\\":\\\"vpc-123abcd\\\",\\\"vswitchId\\\":\\\"vsw-123abcd\\\"}]\",\"Count\":1,\"Code\":\"\",\"Success\":true}","Code":"200","Success":"true"}
```

## Error codes

|HttpCode|Error code|Error message|Description|
|--------|----------|-------------|-----------|
|500|Error|The requested service is unavailable. Please try again later.|The error message returned because a service exception occurred. Try again.|

For a list of error codes, visit the [API Error Center](https://error-center.alibabacloud.com/status/product/dg).

