>? **当前页面接口为旧版 API，未来可能停止维护，目前不展示在左侧导航。黑石物理服务器1.0 API 3.0 版本接口定义更加规范，访问时延下降显著，建议使用 <a href="https://cloud.tencent.com/document/api/386/18637" target="_blank">黑石物理服务器1.0 API 3.0</a>。**
>

## 功能描述
 
GetBmCertDetail 用于获取黑石负载均衡证书详情。

接口请求域名：bmlb.api.qcloud.com


## 请求
### 请求示例

```
GET https://bmlb.api.qcloud.com/v2/index.php?Action=GetBmCertDetail
	&<公共请求参数>
	&certId=<证书ID>
```

### 请求参数

以下请求参数列表仅列出了接口请求参数，正式调用时需要加上公共请求参数，见[公共请求参数页面](/document/product/386/6718)。其中，此接口的Action字段为 GetBmCertDetail。

以下请求参数列表仅列出了接口请求参数，其它参数见[公共请求参数](/document/product/386/6718)页面。

| 参数名称 | 必选  | 类型 | 描述 |
|---------|---------|---------|---------|
| certId | 是 | String | 证书ID。|




## 响应
### 响应示例

```
{
    "code": 0,
    "message": "",
    "codeDesc": "Success",
    "data": {
        "certId": "abcdefgh",
		"certName": "certName",
		"certType": "SVR",
		"certContent": "-----BEGIN CERTIFICATE-----
            MIIE0DCCA7igAwIBAgIQEgaTYAJIpw1PQxjSr1FlTDANBgkqhkiG9w0BAQsFADBP
            MQswCQYDVQQGEwJDTjEaMBgGA1UEChMRV29TaWduIENBIExpbWl0ZWQxJDAiBgNV
            BAMMG0NBIOayg+mAmuWFjei0uVNTTOivgeS5piBHMjAeFw0xNjA1MTMwODIxMjVa
            Fw0xODA2MTMwODIxMjVaMBUxEzARBgNVBAMMCmcuZi14ai5jb20wggEiMA0GCSqG
            SIb3DQEBAQUAA4IBDwAwggEKAoIBAQC4/Ei7dxUJYXgY1V1PflCMwUrkG8Ack0vw
            +C/hCzivNBw5N0WA1Tch4REOIyDPIBq2wiblw4kSsHOF5CfB9DwDhaknZwzwyynZ
            Wr2NekKjoo6x0viqFydVyiVWGzW1qr6Dn9tiDcp75W/Os+nUzKHcc0Wd5aHvjGKD
            6xEPQKLvCZ0F4208rHWcoSnYiaFJPUAfegd8JvK5al0BvSZoXICo6Taf5x4xHag1
            6ymINH1ClLcAIOpAITWddqV20xaXrvdU7J0BusmYkHc840X3cvBywjFurzN5oLg2
            vtVQhGm6qJ/Fjqdg8w40BZkTQb4PlEX8AJ27g+548giuVnLzf8CHAgMBAAGjggHg
            MIIB3DAOBgNVHQ8BAf8EBAMCBaAwHQYDVR0lBBYwFAYIKwYBBQUHAwIGCCsGAQUF
            BwMBMAkGA1UdEwQCMAAwHQYDVR0OBBYEFBvlTUGHZ/GGU4qGT+T7r/Zbcg0pMB8G
            A1UdIwQYMBaAFDDadIbzKJBWntcxMcK9Wc2TEjkdMH8GCCsGAQUFBwEBBHMwcTA1
            BggrBgEFBQcwAYYpaHR0cDovL29jc3AyLndvc2lnbi5jbi9jYTJnMi9zZXJ2ZXIx
            L2ZyZWUwOAYIKwYBBQUHMAKGLGh0dHA6Ly9haWEyLndvc2lnbi5jbi9jYTJnMi5z
            ZXJ2ZXIxLmZyZWUuY2VyMD4GA1UdHwQ3MDUwM6AxoC+GLWh0dHA6Ly9jcmxzMi53
            b3NpZ24uY24vY2EyZzItc2VydmVyMS1mcmVlLmNybDBOBgNVHREERzBFggpnLmYt
            eGouY29tghBzY2hvbGFyLmYteGouY29tggt5dC5mLXhqLmNvbYILZmIuZi14ai5j
            b22CC3R3LmYteGouY29tME8GA1UdIARIMEYwCAYGZ4EMAQIBMDoGCysGAQQBgptR
            AQECMCswKQYIKwYBBQUHAgEWHWh0dHA6Ly93d3cud29zaWduLmNvbS9wb2xpY3kv
            MA0GCSqGSIb3DQEBCwUAA4IBAQCJSd/1xmxwnT/TtKvvxTvDnkCpfsFYVmqiHB/Z
            rXiMdgobUOfF7C8kcBCTqSQAXZF3fjJ1KyhNulvKOffzGGYp+rMwoTAmfaNLUxD/
            X9gPLxZCiysDBQ1BLe16k4aKUHIOmqQNF1MD/8hOZBxjevctKaXc4Xqm2gxJLxDH
            RoY3HKZcdB6t/x7YJU640wvaFqDqIgR6Pc74YjtLrNjkXcf/IQU7c2yjZt9NIGeS
            OTku5DmFasRf04tmE7naB+wkUZOwAqGK8CESNS11BYZjO/M4G/ALS8zCpShUy89H
            hYiYAG5jdNI4vyWwaU4428nG3YvKzlTOpCaowqgbyCcqmtAT
            -----END CERTIFICATE-----",
		"certDomain": "xxx.com",
		"certSubjectDomain": ["s-xxx.com"],
		"certUploadTime": "2017-03-29 11:57:28",
		"certBeginTime": "2016-05-25 08:00:00",
		"certEndTime": "2019-07-25 07:59:59",
		"certLBList": {
			"lbId": "lb-abcdefg",
			"lbName": "lbtest",
			"vpcId": 12345,
			"regionId": 8,
		}
    }
}
```

### 响应参数

| 参数名称 | 类型 | 描述 |
|---------|---------|---------|
| code | Int | 错误码。0表示成功，其他值表示失败。详见错误码页面的[公共错误码](/document/product/386/6725)。|
| message | String | 错误信息描述，与接口相关。|
| codeDesc | String | 返回码信息描述。|
| data | Obj | 返回对象。|

data包含字段如下

| 参数名称 | 类型 | 描述 |
|---------|---------|---------|
| certId | String | 证书ID。|
| certName | String | 证书名称。|
| certType | String | 证书类型（SVR=服务器证书，CA=客户端证书）。|
| certContent | String | 证书内容。|
| certDomain | String | 证书主域名。|
| certSubjectDomain | Array | 证书子域名列表。|
| certUploadTime | String | 证书上传时间。|
| certBeginTime | String | 证书生效时间。|
| certEndTime | String | 证书失效时间。|
| certLBList | Array | 该证书关联的黑石负载均衡对象列表。|

certLBList每一个子项目包含字段如下

| 参数名称 | 类型 | 描述 |
|---------|---------|---------|
| lbId | String | 黑石负载均衡实例ID。|
| lbName | String | 黑石负载均衡实例名称。|
| vpcId | Int | 该黑石负载均衡所在的vpcId。|
| regionId | Int | 该黑石负载均衡所在的regionId。|

## 错误码

| 错误代码 | 英文提示 | 错误描述 |
|------|------|------|
| 9003 | InvalidParameter | 参数错误 |
| 9006 | InternalError.CCDBAbnormal | CCDB 服务异常 |
| -20000 | InvalidResource.CertPlatformErr | 访问证书平台异常 |

## 实际案例
 
### 输入

```
GET https://bmlb.api.qcloud.com/v2/index.php?Action=GetBmCertDetail
	&SecretId=AKIDlfdHxN0ntSVt4KPH0xXWnGl21UUFNoO5
	&Nonce=24763
	&Timestamp=1507714922
	&Region=bj
	&certId=abcdefgh
	&Signature=AySJsE6Zq3knXwPSzxlYUl%2FrM90%3D
```

### 输出

```
{
    "code": 0,
    "message": "",
    "codeDesc": "Success",
    "data": {
        "certId": "abcdefgh",
		"certName": "certName",
		"certType": "SVR",
		"certContent": "-----BEGIN CERTIFICATE-----
            MIIE0DCCA7igAwIBAgIQEgaTYAJIpw1PQxjSr1FlTDANBgkqhkiG9w0BAQsFADBP
            MQswCQYDVQQGEwJDTjEaMBgGA1UEChMRV29TaWduIENBIExpbWl0ZWQxJDAiBgNV
            BAMMG0NBIOayg+mAmuWFjei0uVNTTOivgeS5piBHMjAeFw0xNjA1MTMwODIxMjVa
            Fw0xODA2MTMwODIxMjVaMBUxEzARBgNVBAMMCmcuZi14ai5jb20wggEiMA0GCSqG
            SIb3DQEBAQUAA4IBDwAwggEKAoIBAQC4/Ei7dxUJYXgY1V1PflCMwUrkG8Ack0vw
            +C/hCzivNBw5N0WA1Tch4REOIyDPIBq2wiblw4kSsHOF5CfB9DwDhaknZwzwyynZ
            Wr2NekKjoo6x0viqFydVyiVWGzW1qr6Dn9tiDcp75W/Os+nUzKHcc0Wd5aHvjGKD
            6xEPQKLvCZ0F4208rHWcoSnYiaFJPUAfegd8JvK5al0BvSZoXICo6Taf5x4xHag1
            6ymINH1ClLcAIOpAITWddqV20xaXrvdU7J0BusmYkHc840X3cvBywjFurzN5oLg2
            vtVQhGm6qJ/Fjqdg8w40BZkTQb4PlEX8AJ27g+548giuVnLzf8CHAgMBAAGjggHg
            MIIB3DAOBgNVHQ8BAf8EBAMCBaAwHQYDVR0lBBYwFAYIKwYBBQUHAwIGCCsGAQUF
            BwMBMAkGA1UdEwQCMAAwHQYDVR0OBBYEFBvlTUGHZ/GGU4qGT+T7r/Zbcg0pMB8G
            A1UdIwQYMBaAFDDadIbzKJBWntcxMcK9Wc2TEjkdMH8GCCsGAQUFBwEBBHMwcTA1
            BggrBgEFBQcwAYYpaHR0cDovL29jc3AyLndvc2lnbi5jbi9jYTJnMi9zZXJ2ZXIx
            L2ZyZWUwOAYIKwYBBQUHMAKGLGh0dHA6Ly9haWEyLndvc2lnbi5jbi9jYTJnMi5z
            ZXJ2ZXIxLmZyZWUuY2VyMD4GA1UdHwQ3MDUwM6AxoC+GLWh0dHA6Ly9jcmxzMi53
            b3NpZ24uY24vY2EyZzItc2VydmVyMS1mcmVlLmNybDBOBgNVHREERzBFggpnLmYt
            eGouY29tghBzY2hvbGFyLmYteGouY29tggt5dC5mLXhqLmNvbYILZmIuZi14ai5j
            b22CC3R3LmYteGouY29tME8GA1UdIARIMEYwCAYGZ4EMAQIBMDoGCysGAQQBgptR
            AQECMCswKQYIKwYBBQUHAgEWHWh0dHA6Ly93d3cud29zaWduLmNvbS9wb2xpY3kv
            MA0GCSqGSIb3DQEBCwUAA4IBAQCJSd/1xmxwnT/TtKvvxTvDnkCpfsFYVmqiHB/Z
            rXiMdgobUOfF7C8kcBCTqSQAXZF3fjJ1KyhNulvKOffzGGYp+rMwoTAmfaNLUxD/
            X9gPLxZCiysDBQ1BLe16k4aKUHIOmqQNF1MD/8hOZBxjevctKaXc4Xqm2gxJLxDH
            RoY3HKZcdB6t/x7YJU640wvaFqDqIgR6Pc74YjtLrNjkXcf/IQU7c2yjZt9NIGeS
            OTku5DmFasRf04tmE7naB+wkUZOwAqGK8CESNS11BYZjO/M4G/ALS8zCpShUy89H
            hYiYAG5jdNI4vyWwaU4428nG3YvKzlTOpCaowqgbyCcqmtAT
            -----END CERTIFICATE-----",
		"certDomain": "xxx.com",
		"certSubjectDomain": ["s-xxx.com"],
		"certUploadTime": "2017-03-29 11:57:28",
		"certBeginTime": "2016-05-25 08:00:00",
		"certEndTime": "2019-07-25 07:59:59",
		"certLBList": {
			"lbId": "lb-abcdefg",
			"lbName": "lbtest",
			"vpcId": 12345,
			"regionId": 8,
		}
    }
}

```