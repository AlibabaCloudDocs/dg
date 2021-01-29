# DescribeRegions

调用DescribeRegions获取支持的Region。

## 调试

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=dg&api=DescribeRegions&type=RPC&version=2019-03-27)

## 请求参数

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DescribeRegions|系统规定参数。取值：DescribeRegions。 |
|RegionId|String|否|cn-hangzhou|地域 ID。 |

## 返回数据

|名称|类型|示例值|描述|
|--|--|---|--|
|Code|String|200|响应码。 |
|ErrorMsg|String|Error|错误信息。 |
|Regions|Array of Region| |Region |
|Region| | | |
|LocalName|String|杭州|地域名称。 |
|RegionEndpoint|String|dg.cn-hangzhou.aliyuncs.com|Region Endpoint |
|RegionId|String|cn-hangzhou|地域 ID。 |
|RequestId|String|41916DEB-F62D-41FA-AB53-FC61D795BC66|请求ID |
|Success|Boolean|true|请求成功标示。 |

## 示例

请求示例

```
http(s)://[Endpoint]/?Action=DescribeRegions
&<公共请求参数>
```

正常返回示例

`XML`格式

```
<RequestId>41916DEB-F62D-41FA-AB53-FC61D795BC66</RequestId>
<ErrorMsg>Error</ErrorMsg>
<Regions>
    <Region>
        <RegionId>cn-hangzhou</RegionId>
        <RegionEndpoint>dg.cn-hangzhou.aliyuncs.com</RegionEndpoint>
        <LocalName>杭州</LocalName>
    </Region>
</Regions>
<Code>200</Code>
<Success>true</Success>
```

`JSON`格式

```
{"RequestId":"41916DEB-F62D-41FA-AB53-FC61D795BC66","ErrorMsg":"Error","Regions":{"Region":[{"RegionId":"cn-hangzhou","RegionEndpoint":"dg.cn-hangzhou.aliyuncs.com","LocalName":"杭州"}]},"Code":"200","Success":"true"}
```

## 错误码

访问[错误中心](https://error-center.aliyun.com/status/product/dg)查看更多错误码。

