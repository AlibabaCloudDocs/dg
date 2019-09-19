# DeleteGateway {#concept_878734 .concept}

调用DeleteGateway接口删除网关信息。

**说明：** 调用该接口时，若网关配置下存在正在运行的实例，需要将实例停止后才能删除。

|名称|类型|是否必选|示例|描述|
|--|--|----|--|--|
|GatewayId|String|是|111111|网关ID|

**返回参数**：SUCCESS或异常信息

**示例**

请求示例

``` {#codeblock_9z0_xlg_i58}
http(s)://dg.aliyuncs.com/?Action=DeleteGateway
&RegionId=cn-hangzhou
&GatewayId=111111xxxxxx
&<公共请求参数>
```

正常返回示例

JSON 格式

``` {#codeblock_ysx_3sc_izg}
{
    "RequestId":"CDDAAA07-D806-AG67-BEE8-1E43AAE024DD"
}
```

