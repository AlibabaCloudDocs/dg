# DeleteDatabase {#concept_878841 .concept}

调用DeleteDatabase接口删除数据库。

|名称|类型|是否必选|示例|描述|
|--|--|----|--|--|
|InstanceId|String|是|db|实例ID|

**返回参数**：SUCCESS或登录异常信息

**示例**

请求示例

``` {#codeblock_5iy_b4b_9mv}
http(s)://dg.aliyuncs.com/?Action=DeleteDatabase
&RegionId=cn-hangzhou
&InstanceId=z8gw7qdjm361b4i
&<公共请求参数>
```

正常返回示例

JSON 格式

``` {#codeblock_sdb_td6_ovm}
{
    "RequestId":"CDDAAA07-D806-AG67-BEE8-1E43AAE024DC"
}
```

