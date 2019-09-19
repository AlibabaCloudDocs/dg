# DownloadGatewayProgram {#concept_878756 .concept}

调用DownloadGatewayProgram接口获取网关程序的下载地址。阿里云用户均可下载，无需权限认证。

**返回参数**：网关程序的下载地址

请求示例

``` {#codeblock_m6s_st5_ijc}
http(s)://dg.aliyuncs.com/?Action=DownloadGatewayProgram
&RegionId=cn-hangzhou
&GatewayId=111111xxxxxx
&<公共请求参数>
```

正常返回示例

JSON 格式

``` {#codeblock_qc7_9zi_knh}
{
    "Data": "https://public-buk.oss-cn-hangzhou.aliyuncs.com/db-gateway-pkgs/gateway-daemon-pkgs/aliyun-db-gateway.tar.gz?Expires=xxx/YV56pzE%3D",
    "RequestId": "028D8614-5940-4BC4-86BB-428E115F27DC"
}
```

