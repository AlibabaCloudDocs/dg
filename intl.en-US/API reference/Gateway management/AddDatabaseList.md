# AddDatabaseList

Adds multiple databases at a time.

## Debugging

[OpenAPI Explorer automatically calculates the signature value. For your convenience, we recommend that you call this operation in OpenAPI Explorer. OpenAPI Explorer dynamically generates the sample code of the operation for different SDKs.](https://api.aliyun.com/#product=dg&api=AddDatabaseList&type=RPC&version=2019-03-27)

## Request parameters

|Parameter|Type|Required|Example|Description|
|---------|----|--------|-------|-----------|
|Action|String|Yes|AddDatabaseList|The operation that you want to perform. Set the value to AddDatabaseList. |
|DatabaseString|String|Yes|\[\{"host":"127.0.0.1","port":"3306","gatewayId":"dg-xsdasdasdasdasd"\}\]|The information about the database that you want to add. |
|ClientToken|String|No|ETnLKlblzczshOTUbOCzxxxx|The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must ensure that it is unique among different requests. The token is case-sensitive and can contain only ASCII characters. The token must be 1 to 64 characters in length. |

## Response parameters

|Parameter|Type|Example|Description|
|---------|----|-------|-----------|
|Code|String|200|The HTTP status code. |
|Data|String|SUCCESS|The response data. |
|ErrorMsg|String|Error|The error message. |
|RequestId|String|ABCD-1234|The ID of the request. |
|Success|Boolean|true|Indicates whether the call is successful. |

## Examples

Sample requests

```
http(s)://[Endpoint]/? Action=AddDatabaseList
&DatabaseString=[{"host":"127.0.0.1","port":"3306","gatewayId":"dg-xsdasdasdasdasd"}]
&<Common request parameters>
```

Sample responses

`XML` format

```
<RequestId>ABCD-1234</RequestId>
<ErrorMsg>Error</ErrorMsg>
<Data>SUCCESS</Data>
<Code>200</Code>
<Success>true</Success>
```

`JSON` format

```
{"RequestId":"ABCD-1234","ErrorMsg":"Error","Data":"SUCCESS","Code":"200","Success":"true"}
```

## Error codes

|HttpCode|Error code|Error message|Description|
|--------|----------|-------------|-----------|
|500|Error|The requested service is unavailable. Please try again later.|The error message returned because a service exception occurred. Try again.|

For a list of error codes, visit the [API Error Center](https://error-center.alibabacloud.com/status/product/dg).

