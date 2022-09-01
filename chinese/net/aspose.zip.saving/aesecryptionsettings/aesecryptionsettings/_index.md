---
title: AesEcryptionSettings
second_title: Aspose.ZIP for .NET API 参考
description: 初始化AesEcryptionSettingsaspose.zip.saving/aesecryptionsettings类的新实例
type: docs
weight: 10
url: /zh/net/aspose.zip.saving/aesecryptionsettings/aesecryptionsettings/
---
## AesEcryptionSettings(string, EncryptionMethod) {#constructor_1}

初始化[`AesEcryptionSettings`](../../aesecryptionsettings)类的新实例。

```csharp
public AesEcryptionSettings(string password, EncryptionMethod method)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| password | String | 加密或解密密码。 |
| method | EncryptionMethod | 指示密码块大小的算法选项。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| NotSupportedException | *method*不是AES128,AES192或AES256。 |

### 例子

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.zip");
}
```

### 也可以看看

* enum [EncryptionMethod](../../encryptionmethod)
* class [AesEcryptionSettings](../../aesecryptionsettings)
* 命名空间 [Aspose.Zip.Saving](../../aesecryptionsettings)
* 部件 [Aspose.Zip](../../../)

---

## AesEcryptionSettings(EncryptionMethod) {#constructor}

在没有密码的情况下初始化[`AesEcryptionSettings`](../../aesecryptionsettings)类的新实例。

```csharp
public AesEcryptionSettings(EncryptionMethod method)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| method | EncryptionMethod | 指示密码块大小的算法选项。 |

### 也可以看看

* enum [EncryptionMethod](../../encryptionmethod)
* class [AesEcryptionSettings](../../aesecryptionsettings)
* 命名空间 [Aspose.Zip.Saving](../../aesecryptionsettings)
* 部件 [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->