# CreateGateway

调用CreateGateway创建一个新网关。

## 调试

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=dg&api=CreateGateway&type=RPC&version=2019-03-27)

## 请求参数

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|CreateGateway|系统规定参数。取值：**CreateGateway**。 |
|GatewayDesc|String|是|用于线上环境的网关|网关描述。 |
|GatewayName|String|是|线上环境|网关名称。 |
|RegionId|String|否|cn-hangzhou|地域ID。 |

## 返回数据

|名称|类型|示例值|描述|
|--|--|---|--|
|Code|String|OK|响应码。 |
|Data|String|dg-yhss6sdlaff\*\*\*\*|网关ID。 |
|ErrorMsg|String|无|异常信息。 |
|RequestId|String|A7D17E3E-358C-4A80-986C-F6C3B048AD17|请求ID。 |
|Success|Boolean|true|是否成功。 |

## 示例

请求示例

```
http(s)://dg.[regionId].aliyuncs.com/?Action=CreateGateway
&GatewayDesc=用于线上环境的网关
&GatewayName=线上环境
&<公共请求参数>
```

正常返回示例

`XML`格式

```
<RequestId>A7D17E3E-358C-4A80-986C-F6C3B048AD17</RequestId>
<ErrorMsg>无</ErrorMsg>
<Data>dg-yhss6sdlaff****</Data>
<Code>OK</Code>
<Success>true</Success>
```

`JSON`格式

```
{"RequestId":"A7D17E3E-358C-4A80-986C-F6C3B048AD17","ErrorMsg":"无","Data":"dg-yhss6sdlaff****","Code":"OK","Success":"true"}
```

## 错误码

访问[错误中心](https://error-center.alibabacloud.com/status/product/dg)查看更多错误码。

