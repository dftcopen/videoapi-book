# Http Headers

在阿里云 APP 认证模式下,http headers 除了需要携带签名和 appkey 需要的字段外,在获取到企业区 域代码后,  

需要在 header 中携带 region 字段,以验证对应用户是否有获取该区域企业信息权限。

* 阿里云 APP 认证模式下,接口至少需要包含如下 headers:

```
Content-Type: application/json
Accept: application/json
X-Ca-Key: AppKey
X-Ca-Signature:签名字符串
Region: 区域代码 /* 获取到 region 后加入 header */
```



