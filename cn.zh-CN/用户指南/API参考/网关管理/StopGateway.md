# StopGateway {#concept_878745 .concept}

调用StopGateway接口停止网关服务。

|名称|类型|是否必选|示例|描述|
|--|--|----|--|--|
|GatewayId|String|是|111111|网关ID|

**返回参数**：SUCCESS或异常信息

**示例**

请求示例

``` {#codeblock_faq_oa7_kx0}
http(s)://dg.aliyuncs.com/?Action=StopGateway
&RegionId=cn-hangzhou
&GatewayId=111111xxxxxx
&<公共请求参数>
```

正常返回示例

JSON 格式

``` {#codeblock_u1h_pgh_8vl}
{
    "RequestId":"CDDAAA07-D806-AG67-BEE8-1E43AAE024DE"
}
```

