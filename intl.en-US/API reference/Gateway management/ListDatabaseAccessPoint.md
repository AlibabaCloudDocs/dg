# ListDatabaseAccessPoint

Queries database access points.

## Debugging

[OpenAPI Explorer automatically calculates the signature value. For your convenience, we recommend that you call this operation in OpenAPI Explorer. OpenAPI Explorer dynamically generates the sample code of the operation for different SDKs.](https://api.aliyun.com/#product=dg&api=ListDatabaseAccessPoint&type=RPC&version=2019-03-27)

## Request parameters

|Parameter|Type|Required|Example|Description|
|---------|----|--------|-------|-----------|
|Action|String|Yes|ListDatabaseAccessPoint|The operation that you want to perform. Set the value to ListDatabaseAccessPoint. |
|PageNumber|String|Yes|1|The number of the page to return. |
|PageSize|String|Yes|20|The number of entries to return on each page. |
|Port|Integer|Yes|3306|The port number. |
|GatewayId|String|No|dg-123|The ID of the gateway. |
|SearchKey|String|No|dg-123|The key for fuzzy searches. |
|DbInstanceId|String|No|dg-db-123|The ID of the database instance. |
|RegionId|String|No|cn-hangzhou|The ID of the region. |
|Host|String|No|127.0.0.1|The IP address of the host. |
|VpcId|String|No|vpc-123|The ID of the VPC. |

## Response parameters

|Parameter|Type|Example|Description|
|---------|----|-------|-----------|
|Code|String|200|The HTTP status code. |
|Count|Integer|1|The number of entries returned. |
|Data|String|\{"RequestId":"1230314LGD","ErrorMsg":"","Data":"\[\{\\"accessAddr\\":\\"172.16.144.216\\",\\"accessPort\\":3306,\\"dbInstanceId\\":\\"dg-db-123\\",\\"gmtCreate\\":1609906143000,\\"gmtModified\\":1609906143000,\\"routerId\\":\\"cn-hangzhou\\",\\"vpcAzoneId\\":\\"cn-hangzhou-i\\",\\"vpcId\\":\\"vpc-123\\",\\"vswitchId\\":\\"vsw-123\\"\}\]","Count":1,"Code":"","Success":true\}|The response data. |
|ErrorMsg|String|Error|The error message. |
|RequestId|String|1230314LGD|The ID of the request. |
|Success|String|true|Indicates whether the call is successful. |

## Examples

Sample requests

```
http(s)://[Endpoint]/? Action=ListDatabaseAccessPoint
&PageNumber=1
&PageSize=20
&Port=3306
&<Common request parameters>
```

Sample responses

`XML` format

```
<RequestId>1230314LGD</RequestId>
<ErrorMsg>Error</ErrorMsg>
<Data>{"RequestId":"1230314LGD","ErrorMsg":"","Data":"[{\"accessAddr\":\"172.16.144.216\",\"accessPort\":3306,\"dbInstanceId\":\"dg-db-123\",\"gmtCreate\":1609906143000,\"gmtModified\":1609906143000,\"routerId\":\"cn-hangzhou\",\"vpcAzoneId\":\"cn-hangzhou-i\",\"vpcId\":\"vpc-123\",\"vswitchId\":\"vsw-123\"}]","Count":1,"Code":"","Success":true}</Data>
<Count>1</Count>
<Code>200</Code>
<Success>true</Success>
```

`JSON` format

```
{"RequestId":"1230314LGD","ErrorMsg":"Error","Data":"{\"RequestId\":\"1230314LGD\",\"ErrorMsg\":\"\",\"Data\":\"[{\\\"accessAddr\\\":\\\"172.16.144.216\\\",\\\"accessPort\\\":3306,\\\"dbInstanceId\\\":\\\"dg-db-123\\\",\\\"gmtCreate\\\":1609906143000,\\\"gmtModified\\\":1609906143000,\\\"routerId\\\":\\\"cn-hangzhou\\\",\\\"vpcAzoneId\\\":\\\"cn-hangzhou-i\\\",\\\"vpcId\\\":\\\"vpc-123\\\",\\\"vswitchId\\\":\\\"vsw-123\\\"}]\",\"Count\":1,\"Code\":\"\",\"Success\":true}","Count":"1","Code":"200","Success":"true"}
```

## Error codes

|HttpCode|Error code|Error message|Description|
|--------|----------|-------------|-----------|
|500|Error|The requested service is unavailable. Please try again later.|The error message returned because a service exception occurred. Try again.|

For a list of error codes, visit the [API Error Center](https://error-center.alibabacloud.com/status/product/dg).

