# CreateGatewayVerifyCode {#concept_878753 .concept}

调用CreateGatewayVerifyCode接口生成线下安装网关时需要的验证码。该验证码将与云上创建的网关相对应。

|名称|类型|是否必选|示例|描述|
|--|--|----|--|--|
|GatewayId|String|是|111111|网关ID|

**返回参数**：验证码信息

**示例**

请求示例

``` {#codeblock_4gj_thp_5xr}
http(s)://dg.aliyuncs.com/?Action=CreateGatewayVerifyCode
&RegionId=cn-hangzhou
&GatewayId=111111xxxxxx
&<公共请求参数>
```

正常返回示例

JSON 格式

``` {#codeblock_9n2_ivi_ast}
{
    "Data": "qvCKyMgl",    
    "RequestId":"CDDAAA07-D806-AG67-BEE8-1E43AAE024DF"
}
```

