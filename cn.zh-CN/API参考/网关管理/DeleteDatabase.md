# DeleteDatabase

调用DeleteDatabase删除数据库。

## 调试

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=dg&api=DeleteDatabase&type=RPC&version=2019-03-27)

## 请求参数

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DeleteDatabase|系统规定参数。取值：**DeleteDatabase**。 |
|InstanceId|String|是|z8gw7qdjm36\*\*\*\*|实例ID。 |

## 返回数据

|名称|类型|示例值|描述|
|--|--|---|--|
|Code|String|OK|响应码。 |
|Data|String|2019-09-12T14:40:46|返回结果。 |
|ErrorMsg|String|无|异常信息。 |
|RequestId|String|CDDAAA07-D806-AG67-BEE8-1E43AAE024DC|请求ID。 |
|Success|Boolean|true|是否成功。 |

## 示例

请求示例

```
http(s)://[Endpoint]/?Action=DeleteDatabase
&InstanceId=z8gw7qdjm36****
&<公共请求参数>
```

正常返回示例

`XML`格式

```
<RequestId>CDDAAA07-D806-AG67-BEE8-1E43AAE024DC</RequestId>
<ErrorMsg>无</ErrorMsg>
<Data>2019-09-12T14:40:46	</Data>
<Code>OK</Code>
<Success>true</Success>
```

`JSON`格式

```
{"RequestId":"CDDAAA07-D806-AG67-BEE8-1E43AAE024DC","ErrorMsg":"无","Data":"2019-09-12T14:40:46\t","Code":"OK","Success":"true"}
```

## 错误码

访问[错误中心](https://error-center.aliyun.com/status/product/dg)查看更多错误码。

