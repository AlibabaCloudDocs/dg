# CreateGateway {#concept_861901 .concept}

调用CreateGateway接口创建一个新网关。

|名称|类型|是否必选|示例|描述|
|--|--|----|--|--|
|GatewayName|String|是|线上环境|网关名称|
|GatewayDesc|String|否|用于线上环境的网关|网关描述|

|名称|类型|示例|描述|
|--|--|--|--|
|GatewayId|String|dd5b7cc618e34d80a84f6c932bd9b1fe|网关ID|

**示例**

请求示例

``` {#codeblock_56v_eu8_1m8}
http(s)://dg.aliyuncs.com/?Action=CreateGateway
&RegionId=cn-hangzhou
&GatewayName=线上环境
&GatewayDesc=用于线上环境的网关
&<公共请求参数>
```

正常返回示例

JSON 格式

``` {#codeblock_jef_36l_vqj}
{
    "Data":"dd5b7cc618e34d80a84f6c932bd9b1fe",
    "RequestId":"A7D17E3E-358C-4A80-986C-F6C3B048AD17"
}
```

