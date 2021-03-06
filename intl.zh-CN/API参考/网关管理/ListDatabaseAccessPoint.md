# ListDatabaseAccessPoint

调用ListDatabaseAccessPoint获取数据库访问点列表。

## 调试

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=dg&api=ListDatabaseAccessPoint&type=RPC&version=2019-03-27)

## 请求参数

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|ListDatabaseAccessPoint|系统规定参数。取值：ListDatabaseAccessPoint。 |
|PageNumber|String|是|1|列表的页码值。 |
|PageSize|String|是|20|分页查询时设置的每页行数。 |
|Port|Integer|是|3306|端口号。 |
|GatewayId|String|否|dg-123|网关ID。 |
|SearchKey|String|否|dg-123|模糊搜索的值。 |
|DbInstanceId|String|否|dg-db-123|数据库实例ID。 |
|RegionId|String|否|cn-hangzhou|地域ID。 |
|Host|String|否|127.0.0.1|主机IP地址。 |
|VpcId|String|否|vpc-123|专有网络VpcId。 |

## 返回数据

|名称|类型|示例值|描述|
|--|--|---|--|
|Code|String|200|响应码。 |
|Count|Integer|1|数据条数。 |
|Data|String|\{"RequestId":"1230314LGD","ErrorMsg":"","Data":"\[\{\\"accessAddr\\":\\"172.16.144.216\\",\\"accessPort\\":3306,\\"dbInstanceId\\":\\"dg-db-123\\",\\"gmtCreate\\":1609906143000,\\"gmtModified\\":1609906143000,\\"routerId\\":\\"cn-hangzhou\\",\\"vpcAzoneId\\":\\"cn-hangzhou-i\\",\\"vpcId\\":\\"vpc-123\\",\\"vswitchId\\":\\"vsw-123\\"\}\]","Count":1,"Code":"","Success":true\}|返回数据。 |
|ErrorMsg|String|Error|错误信息。 |
|RequestId|String|1230314LGD|请求ID。 |
|Success|String|true|请求成功标识。 |

## 示例

请求示例

```
http(s)://[Endpoint]/?Action=ListDatabaseAccessPoint
&PageNumber=1
&PageSize=20
&Port=3306
&<公共请求参数>
```

正常返回示例

`XML`格式

```
<RequestId>1230314LGD</RequestId>
<ErrorMsg>Error</ErrorMsg>
<Data>{"RequestId":"1230314LGD","ErrorMsg":"","Data":"[{\"accessAddr\":\"172.16.144.216\",\"accessPort\":3306,\"dbInstanceId\":\"dg-db-123\",\"gmtCreate\":1609906143000,\"gmtModified\":1609906143000,\"routerId\":\"cn-hangzhou\",\"vpcAzoneId\":\"cn-hangzhou-i\",\"vpcId\":\"vpc-123\",\"vswitchId\":\"vsw-123\"}]","Count":1,"Code":"","Success":true}</Data>
<Count>1</Count>
<Code>200</Code>
<Success>true</Success>
```

`JSON`格式

```
{"RequestId":"1230314LGD","ErrorMsg":"Error","Data":"{\"RequestId\":\"1230314LGD\",\"ErrorMsg\":\"\",\"Data\":\"[{\\\"accessAddr\\\":\\\"172.16.144.216\\\",\\\"accessPort\\\":3306,\\\"dbInstanceId\\\":\\\"dg-db-123\\\",\\\"gmtCreate\\\":1609906143000,\\\"gmtModified\\\":1609906143000,\\\"routerId\\\":\\\"cn-hangzhou\\\",\\\"vpcAzoneId\\\":\\\"cn-hangzhou-i\\\",\\\"vpcId\\\":\\\"vpc-123\\\",\\\"vswitchId\\\":\\\"vsw-123\\\"}]\",\"Count\":1,\"Code\":\"\",\"Success\":true}","Count":"1","Code":"200","Success":"true"}
```

## 错误码

|HttpCode|错误码|错误信息|描述|
|--------|---|----|--|
|500|Error|The requested service is unavailable. Please try again later.|服务异常，请重试|

访问[错误中心](https://error-center.alibabacloud.com/status/product/dg)查看更多错误码。

