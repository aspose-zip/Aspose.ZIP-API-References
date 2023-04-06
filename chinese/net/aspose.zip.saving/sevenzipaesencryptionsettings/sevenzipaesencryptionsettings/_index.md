---
title: SevenZipAESEncryptionSettings.SevenZipAESEncryptionSettings
second_title: Aspose.ZIP for .NET API 参考
description: SevenZipAESEncryptionSettings 构造函数. 初始化一个新的实例SevenZipAESEncryptionSettings类.
type: docs
weight: 10
url: /zh/net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings(string) {#constructor_1}

初始化一个新的实例[`SevenZipAESEncryptionSettings`](../)类.

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| password | String | 用于加密或解密的密码。 |

### 例子

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### 也可以看看

* class [SevenZipAESEncryptionSettings](../)
* 命名空间 [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* 部件 [Aspose.Zip](../../../)

---

## SevenZipAESEncryptionSettings(SevenZipCipher) {#constructor}

初始化一个新的实例[`SevenZipAESEncryptionSettings`](../)带有外部密码的类.

```csharp
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| cipher | SevenZipCipher | 自定义 AES 实现。 |

### 例子

```csharp
SevenZipCipher cipher = ComposeMyCipher();
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings(cipher))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### 也可以看看

* class [SevenZipCipher](../../../aspose.zip.crypto/sevenzipcipher/)
* class [SevenZipAESEncryptionSettings](../)
* 命名空间 [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* 部件 [Aspose.Zip](../../../)


