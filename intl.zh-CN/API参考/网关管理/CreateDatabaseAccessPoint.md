# CreateDatabaseAccessPoint

调用CreateDatabaseAccessPoint创建数据库访问点。

## 调试

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=dg&api=CreateDatabaseAccessPoint&type=RPC&version=2019-03-27)

## 请求参数

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|CreateDatabaseAccessPoint|系统规定参数。取值：CreateDatabaseAccessPoint。 |
|DbInstanceId|String|是|dg-db-abcd1234|实例ID。 |
|VpcAZone|String|是|cn-hangzhou-i|VpcAZone。 |
|VpcId|String|是|vpc-123abcd|专有网络VpcId。 |
|VpcRegionId|String|是|cn-hangzhou|Vpc地域ID。 |
|VSwitchId|String|是|vsw-123abcd|虚拟交换机Id。 |
|RegionId|String|否|cn-hangzhou|地域ID。 |
|ClientToken|String|否|ETnLKlblzczshOTUbOCzxxxx|用于保证请求的幂等性。由客户端生成该参数值，要保证在不同请求间唯一，大小写敏感、不超过64个ASCII字符。 |

## 返回数据

|名称|类型|示例值|描述|
|--|--|---|--|
|Code|String|200|响应码。 |
|Data|String|\{"RequestId":"41916DEB-F62D-41FA-AB53-FC61D795BC66","ErrorMsg":"","Data":"\[\{\\"accessAddr\\":\\"172.16.144.216\\",\\"accessPort\\":3306,\\"dbInstanceId\\":\\"dg-db-abcd123\\",\\"gmtCreate\\":1609906765000,\\"gmtModified\\":1609906765000,\\"routerId\\":\\"cn-hangzhou\\",\\"vpcAzoneId\\":\\"cn-hangzhou-i\\",\\"vpcId\\":\\"vpc-123abcd\\",\\"vswitchId\\":\\"vsw-123abcd\\"\}\]","Count":1,"Code":"","Success":true\}|返回数据。 |
|ErrorMsg|String|Error|报错信息。 |
|RequestId|String|41916DEB-F62D-41FA-AB53-FC61D795BC66|请求ID |
|Success|Boolean|true|请求成功标识。 |

## 示例

请求示例

```
http(s)://[Endpoint]/?Action=CreateDatabaseAccessPoint
&DbInstanceId=dg-db-abcd1234
&VpcAZone=cn-hangzhou-a
&VpcId=vpc-123abcd
&VpcRegionId=cn-hangzhou
&VSwitchId=vswitch-123abcd
&<公共请求参数>
```

正常返回示例

`XML`格式

```
<RequestId>41916DEB-F62D-41FA-AB53-FC61D795BC66</RequestId>
<ErrorMsg>Error</ErrorMsg>
<Data>{"RequestId":"41916DEB-F62D-41FA-AB53-FC61D795BC66","ErrorMsg":"","Data":"[{\"accessAddr\":\"172.16.144.216\",\"accessPort\":3306,\"dbInstanceId\":\"dg-db-abcd123\",\"gmtCreate\":1609906765000,\"gmtModified\":1609906765000,\"routerId\":\"cn-hangzhou\",\"vpcAzoneId\":\"cn-hangzhou-i\",\"vpcId\":\"vpc-123abcd\",\"vswitchId\":\"vsw-123abcd\"}]","Count":1,"Code":"","Success":true}</Data>
<Code>200</Code>
<Success>true</Success>
```

`JSON`格式

```
{"RequestId":"41916DEB-F62D-41FA-AB53-FC61D795BC66","ErrorMsg":"Error","Data":"{\"RequestId\":\"41916DEB-F62D-41FA-AB53-FC61D795BC66\",\"ErrorMsg\":\"\",\"Data\":\"[{\\\"accessAddr\\\":\\\"172.16.144.216\\\",\\\"accessPort\\\":3306,\\\"dbInstanceId\\\":\\\"dg-db-abcd123\\\",\\\"gmtCreate\\\":1609906765000,\\\"gmtModified\\\":1609906765000,\\\"routerId\\\":\\\"cn-hangzhou\\\",\\\"vpcAzoneId\\\":\\\"cn-hangzhou-i\\\",\\\"vpcId\\\":\\\"vpc-123abcd\\\",\\\"vswitchId\\\":\\\"vsw-123abcd\\\"}]\",\"Count\":1,\"Code\":\"\",\"Success\":true}","Code":"200","Success":"true"}
```

## 错误码

|HttpCode|错误码|错误信息|描述|
|--------|---|----|--|
|500|Error|The requested service is unavailable. Please try again later.|服务异常，请重试|

访问[错误中心](https://error-center.alibabacloud.com/status/product/dg)查看更多错误码。

