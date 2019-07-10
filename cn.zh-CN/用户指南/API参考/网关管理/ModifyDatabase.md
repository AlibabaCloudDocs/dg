# ModifyDatabase {#concept_878851 .concept}

调用ModifyDatabase接口修改数据库信息。

|名称|类型|是否必选|示例|描述|
|--|--|----|--|--|
|GatewayId|String|是|111111|网关ID|
|InstanceId|String|是|db|实例ID|
|Host|String|是|11.163.23.109|通过网关所在宿主机去访问数据库的地址。|
|Port|String|是|3440|通过网关所在宿主机去访问数据库的端口。|
|DbType|String \(enumeration\)|否|MySQL|数据库类型 **说明：** 目前数据库类型仅支持MySQL。

 |
|DbUserName|String|是|dg\_test|访问数据库所用的用户名。|
|DbPassword|String|是|password|访问数据库所用的密码。 **说明：** 仅用于验证数据库是否可以连接成功，不做任何其他工作。

 |

**返回参数**：SUCCESS或登录异常信息

**示例**

请求示例

``` {#codeblock_8ub_kgn_ty3}
http(s)://dg.aliyuncs.com/?Action=ModifyDatabase
&RegionId=cn-hangzhou
&GatewayId=111111xxxxxx
&InstanceId=z8gw7qdjm361b4i
&Host=11.163.23.109
&Port=3440
&DbType=MySQL
&DbUserName=dg_test
&DbPassword=password
&<公共请求参数>
```

正常返回示例

JSON 格式

``` {#codeblock_9g8_2zk_dxu}
{
    "RequestId":"EAF2AA07-860D-43DA-BEE8-1E43AAE024ED"
}
```

