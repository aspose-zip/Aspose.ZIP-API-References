---
title: TraditionalEncryptionSettings.TraditionalEncryptionSettings
second_title: Aspose.ZIP for .NET API 参考
description: TraditionalEncryptionSettings 构造函数. 初始化一个新的实例TraditionalEncryptionSettings类.
type: docs
weight: 10
url: /zh/net/aspose.zip.saving/traditionalencryptionsettings/traditionalencryptionsettings/
---
## TraditionalEncryptionSettings(string) {#constructor_1}

初始化一个新的实例[`TraditionalEncryptionSettings`](../)类.

```csharp
public TraditionalEncryptionSettings(string password)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| password | String | 加密密码。 |

### 例子

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 也可以看看

* class [TraditionalEncryptionSettings](../)
* 命名空间 [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* 部件 [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings(string, Encoding) {#constructor_2}

初始化一个新的实例[`TraditionalEncryptionSettings`](../)具有用户定义编码的类.

```csharp
public TraditionalEncryptionSettings(string password, Encoding encoding)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| password | String | 加密密码。 |
| encoding | Encoding | 密码字符的编码。 |

### 评论

不鼓励使用此构造函数。设置编码可能会与标准相矛盾并产生不兼容的存档。

### 例子

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", System.Text.Encoding.ASCII))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 也可以看看

* class [TraditionalEncryptionSettings](../)
* 命名空间 [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* 部件 [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings() {#constructor}

初始化一个新的实例[`TraditionalEncryptionSettings`](../)没有密码的类.

```csharp
public TraditionalEncryptionSettings()
```

### 也可以看看

* class [TraditionalEncryptionSettings](../)
* 命名空间 [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* 部件 [Aspose.Zip](../../../)


