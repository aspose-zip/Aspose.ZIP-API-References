---
title: Class MeteredLicense
second_title: Aspose.ZIP for .NET API 参考
description: Aspose.Zip.MeteredLicense 班级. 提供设置计量密钥的方法
type: docs
weight: 290
url: /zh/net/aspose.zip/meteredlicense/
---
## MeteredLicense class

提供设置计量密钥的方法。

```csharp
public class MeteredLicense
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [MeteredLicense](meteredlicense/)() | 初始化此类的新实例。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [SetMeteredKey](../../aspose.zip/meteredlicense/setmeteredkey/)(string, string) | 设置计量公钥和私钥。 |
| static [GetConsumptionCredit](../../aspose.zip/meteredlicense/getconsumptioncredit/)() | 获得消费信用。 |

### 评论

重要提示：使用计量许可证，您无法编写自解压 zip 存档。

### 例子

在此示例中，将尝试设置计量公钥和私钥。

```csharp
MeteredLicense matered = new MeteredLicense();
matered.SetMeteredKey("PublicKey", "PrivateKey");
```

### 也可以看看

* 命名空间 [Aspose.Zip](../../aspose.zip/)
* 部件 [Aspose.Zip](../../)


