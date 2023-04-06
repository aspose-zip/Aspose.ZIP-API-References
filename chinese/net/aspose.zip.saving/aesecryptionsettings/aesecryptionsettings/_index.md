---
title: AesEcryptionSettings.AesEcryptionSettings
second_title: Aspose.ZIP for .NET API 参考
description: AesEcryptionSettings 构造函数. 初始化一个新的实例AesEcryptionSettings类.
type: docs
weight: 10
url: /zh/net/aspose.zip.saving/aesecryptionsettings/aesecryptionsettings/
---
## AesEcryptionSettings(string, EncryptionMethod) {#constructor_1}

初始化一个新的实例[`AesEcryptionSettings`](../)类.

```csharp
public AesEcryptionSettings(string password, EncryptionMethod method)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| password | String | 用于加密或解密的密码。 |
| method | EncryptionMethod | 指示密码块大小的算法选项。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| NotSupportedException | *method*不是其中之一AES128,AES192 ， 或者AES256. |

### 例子

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.zip");
}
```

### 也可以看看

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* 命名空间 [Aspose.Zip.Saving](../../aesecryptionsettings/)
* 部件 [Aspose.Zip](../../../)

---

## AesEcryptionSettings(EncryptionMethod) {#constructor}

初始化一个新的实例[`AesEcryptionSettings`](../)没有密码的类.

```csharp
public AesEcryptionSettings(EncryptionMethod method)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| method | EncryptionMethod | 指示密码块大小的算法选项。 |

### 也可以看看

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* 命名空间 [Aspose.Zip.Saving](../../aesecryptionsettings/)
* 部件 [Aspose.Zip](../../../)


