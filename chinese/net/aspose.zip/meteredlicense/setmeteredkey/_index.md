---
title: MeteredLicense.SetMeteredKey
second_title: Aspose.ZIP for .NET API 参考
description: MeteredLicense 方法. 设置计量公钥和私钥
type: docs
weight: 20
url: /zh/net/aspose.zip/meteredlicense/setmeteredkey/
---
## MeteredLicense.SetMeteredKey method

设置计量公钥和私钥。

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| publicKey | String | 公钥。 |
| privateKey | String | 私钥。 |

### 评论

如果你购买了metered license，当启动应用程序时，应该调用这个API，通常，这就足够了。 但是，如果总是上传消费数据失败，超过24小时，license会被设置为评估状态， 为避免这种情况，您应该定期检查license状态，如果是评估状态，请重新调用此API。

### 也可以看看

* class [MeteredLicense](../)
* 命名空间 [Aspose.Zip](../../meteredlicense/)
* 部件 [Aspose.Zip](../../../)


