# GetUserDatabases {#concept_895452 .concept}

调用GetUserDatabases接口返回用户数据库列表信息。

|名称|类型|是否必选|示例|描述|
|--|--|----|--|--|
|PageSize|String|是|1|页面大小|
|PageNumber|String|是|10|页码|
|GatewayId|String|否|111111|网关ID|
|SearchKey|String|否|网关|搜索关键字|

**示例**

请求示例

``` {#codeblock_j0l_bup_35z}
http(s)://dg.aliyuncs.com/?Action=GetUserDatabases
&RegionId=cn-hangzhou
&PageSize=1
&PageNumber=1
&<公共请求参数>
```

正常返回示例

JSON 格式

``` {#codeblock_3ls_6kk_idy}
{
    "Data": "[{\"dbDescription\":\"开发环境数据库\",\"dbType\":\"MySQL\",\"dbUserName\":\"dbatool\",\"gatewayId\":\"test_gateway\",\"gatewayName\":\"Gateway—1\",\"gmtCreate\":1560736969000,\"gmtCreateString\":\"2019-06-17 10:02\",\"host\":\"11.163.23.109\",\"instanceId\":\"instance_1\",\"parentId\":\"1344371\",\"port\":3440,\"userId\":\"1344371\"}]",
    "Count": 1,
    "RequestId": "951AE6AA-BFC5-4DD8-8CD6-DFD3D51E4170"
}
```

