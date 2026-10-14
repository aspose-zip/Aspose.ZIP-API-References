---
title: "XarBzip2CompressionSettings.XarBzip2CompressionSettings"
second_title: "Aspose.ZIP for .NET API 参考"
description: "XarBzip2CompressionSettings 构造函数。初始化 XarBzip2CompressionSettings 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.zip.xar/xarbzip2compressionsettings/xarbzip2compressionsettings/
---
## XarBzip2CompressionSettings(int) {#constructor_1}

初始化 [`XarBzip2CompressionSettings`](../) 类的新实例。

```csharp
public XarBzip2CompressionSettings(int blockSize)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| blockSize | Int32 | 块大小（以百千字节为单位）。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentOutOfRangeException | 块大小不在 1 到 9 之间。 |

## 示例

```csharp
using (XarArchive archive = new XarArchive())
{
    archive.CreateEntry("data.bin", "data.bin", new XarBzip2CompressionSettings(1));
    archive.Save("archive.xar");
}
```

### 另请参阅

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## XarBzip2CompressionSettings() {#constructor}

使用默认块大小（等于 9 百千字节）初始化 [`XarBzip2CompressionSettings`](../) 类的新实例。

```csharp
public XarBzip2CompressionSettings()
```

### 另请参阅

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


