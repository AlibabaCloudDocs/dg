# DescribeRegions

Queries the available regions.

## Debugging

[OpenAPI Explorer automatically calculates the signature value. For your convenience, we recommend that you call this operation in OpenAPI Explorer. OpenAPI Explorer dynamically generates the sample code of the operation for different SDKs.](https://api.aliyun.com/#product=dg&api=DescribeRegions&type=RPC&version=2019-03-27)

## Request parameters

|Parameter|Type|Required|Example|Description|
|---------|----|--------|-------|-----------|
|Action|String|Yes|DescribeRegions|The operation that you want to perform. Set the value to DescribeRegions. |
|RegionId|String|No|cn-hangzhou|The ID of the region. |

## Response parameters

|Parameter|Type|Example|Description|
|---------|----|-------|-----------|
|Code|String|200|The HTTP status code. |
|ErrorMsg|String|Error|The error message. |
|Regions|Array of Region| |Region |
|Region| | | |
|LocalName|String|China \(Hangzhou\)|The name of the region. |
|RegionEndpoint|String|dg.cn-hangzhou.aliyuncs.com|Region Endpoint |
|RegionId|String|cn-hangzhou|The ID of the region. |
|RequestId|String|41916DEB-F62D-41FA-AB53-FC61D795BC66|The ID of the request. |
|Success|Boolean|true|Indicates whether the call is successful. |

## Examples

Sample requests

```
http(s)://[Endpoint]/? Action=DescribeRegions
&<Common request parameters>
```

Sample responses

`XML` format

```
<RequestId>41916DEB-F62D-41FA-AB53-FC61D795BC66</RequestId>
<ErrorMsg>Error</ErrorMsg>
<Regions>
    <Region>
        <RegionId>cn-hangzhou</RegionId>
        <RegionEndpoint>dg.cn-hangzhou.aliyuncs.com</RegionEndpoint>
        <LocalName>China (Hangzhou)</LocalName>
    </Region>
</Regions>
<Code>200</Code>
<Success>true</Success>
```

`JSON` format

```
{"RequestId":"41916DEB-F62D-41FA-AB53-FC61D795BC66","ErrorMsg":"Error","Regions":{"Region":[{"RegionId":"cn-hangzhou","RegionEndpoint":"dg.cn-hangzhou.aliyuncs.com","LocalName":"China (Hangzhou)"}]},"Code":"200","Success":"true"}
```

## Error codes

For a list of error codes, visit the [API Error Center](https://error-center.alibabacloud.com/status/product/dg).

