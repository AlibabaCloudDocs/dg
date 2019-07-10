# ModifyGateway {#concept_878728 .concept}

调用ModifyGateway接口修改网关的基本信息。

|名称|类型|是否必选|示例|描述|
|--|--|----|--|--|
|GatewayId|String|是|111111|网关ID|
|GatewayName|String|是|线上环境|网关名称|
|GatewayDesc|String|否|用于线上环境的网关|网关描述|

**返回参数**：SUCCESS或异常信息

**示例**

请求示例

``` {#codeblock_sja_qos_h9c}
http(s)://dg.aliyuncs.com/?Action=ModifyGateway
&RegionId=cn-hangzhou
&GatewayName=线上环境
&GatewayId=111111xxxxxx
&<公共请求参数>
```

正常返回示例

JSON 格式

``` {#codeblock_pof_8ca_ouc}
{
    "RequestId":"CDDAAA07-D806-AG67-BEE8-1E43AAE024DC"
}
```

