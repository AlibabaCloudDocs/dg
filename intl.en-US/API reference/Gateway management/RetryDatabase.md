# RetryDatabase

Retries a database connection.

## Debugging

[OpenAPI Explorer automatically calculates the signature value. For your convenience, we recommend that you call this operation in OpenAPI Explorer. OpenAPI Explorer dynamically generates the sample code of the operation for different SDKs.](https://api.aliyun.com/#product=dg&api=RetryDatabase&type=RPC&version=2019-03-27)

## Request parameters

|Parameter|Type|Required|Example|Description|
|---------|----|--------|-------|-----------|
|Action|String|Yes|RetryDatabase|The operation that you want to perform. Set the value to RetryDatabase. |
|DbPassword|String|Yes|123|The password that is used to log on to the database. |
|DbType|String|Yes|MySQL|The type of the database. |
|DbUserName|String|Yes|abcd|The username that is used to log on to the database. |
|GatewayId|String|Yes|dg-yhss6sdlaff\*\*\*\*|The ID of the gateway. |
|Host|String|Yes|127.0.0.1|The IP address of the host. |
|Port|Integer|Yes|3306|The port number. |
|RegionId|String|Yes|cn-hangzhou|The ID of the region. |
|DbDescription|String|No|123|The description of the database. |
|DbName|String|No|abcd|The name of the database. |
|ClientToken|String|No|ETnLKlblzczshOTUbOCzxxxx|You must ensure that the token is unique among different requests. The token is case-sensitive and can contain only ASCII characters. It must be 1 to 64 characters in length. |

## Response parameters

|Parameter|Type|Example|Description|
|---------|----|-------|-----------|
|Code|String|200|The HTTP status code. |
|Data|String|SUCCESS|The returned result. |
|ErrorMsg|String|Error|The error message. |
|RequestId|String|CDDAAA07-D806-AG67-BEE8-1E43AAE024DD|The ID of the request. |
|Success|Boolean|true|Indicates whether the call is successful. |

## Examples

Sample requests

```
http(s)://[Endpoint]/? Action=RetryDatabase
&DbPassword=123
&DbType=MySQL
&DbUserName=abcd
&GatewayId=dg-yhss6sdlaff****
&Host=127.0.0.1
&Port=3306
&RegionId=cn-hangzhou
&<Common request parameters>
```

Sample responses

`XML` format

```
<RequestId>CDDAAA07-D806-AG67-BEE8-1E43AAE024DD</RequestId>
<ErrorMsg>Error</ErrorMsg>
<Data>SUCCESS</Data>
<Code>200</Code>
<Success>true</Success>
```

`JSON` format

```
{"RequestId":"CDDAAA07-D806-AG67-BEE8-1E43AAE024DD","ErrorMsg":"Error","Data":"SUCCESS","Code":"200","Success":"true"}
```

## Error codes

|HttpCode|Error code|Error message|Description|
|--------|----------|-------------|-----------|
|500|Error|The requested service is unavailable. Please try again later.|The error message returned because a service exception occurred. Try again.|

For a list of error codes, visit the [API Error Center](https://error-center.alibabacloud.com/status/product/dg).

