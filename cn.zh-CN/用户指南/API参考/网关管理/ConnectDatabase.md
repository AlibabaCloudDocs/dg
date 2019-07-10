# ConnectDatabase {#concept_878811 .concept}

调用ConnectDatabase接口通过网关进行数据库连通性测试。

|名称|类型|是否必选|示例|描述|
|--|--|----|--|--|
|Host|String|是|11.163.23.109|通过网关所在宿主机去访问数据库的地址。|
|Port|String|是|3440|通过网关所在宿主机去访问数据库的端口。|
|DbType|String \(enumeration\)|否|MySQL|数据库类型 **说明：** 目前数据库类型仅支持MySQL。

 |
|DbUserName|String|是|dg\_test|访问数据库所用的用户名。|
|DbPassword|String|是|password|访问数据库所用的密码。|

**返回参数**：SUCCESS或登录异常信息

**示例**

请求示例

``` {#codeblock_kju_skn_yyo}
http(s)://dg.aliyuncs.com/?Action=ConnectDatabase
&RegionId=cn-hangzhou
&GatewayId=111111xxxxxx
&Host=11.163.23.109
&Port=3440
&DbType=MySQL
&DbUserName=dg_test
&DbPassword=password
&<公共请求参数>
```

正常返回示例

JSON 格式

``` {#codeblock_wzw_4n0_yra}
{
    "RequestId":"EAF2AA07-860D-43DA-BEE8-1E43AAE024DG"
}
```

