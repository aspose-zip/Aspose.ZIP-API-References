---
title: "ZstandardArchive.Open"
second_title: "Aspose.ZIP for .NET API 参考"
description: "ZstandardArchive 方法。打开存档进行提取并提供包含存档内容的流"
type: docs
weight: 50
url: /zh/net/aspose.zip.zstandard/zstandardarchive/open/
---
## ZstandardArchive.Open method

打开存档进行提取，并提供包含存档内容的流。

```csharp
public Stream Open()
```

### Return Value

表示归档内容的流。

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放，无法使用。 |

## 备注

从流中读取以获取文件的原始内容。参见示例部分。

## 示例

提取归档并将提取的内容复制到文件流。

```csharp
using (var archive = new ZstandardArchive("archive.zst"))
{
    using (var extracted = File.Create("data.bin"))
    {
        var unpacked = archive.Open();
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = unpacked.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }            
}
```

对于 .NET 4.0 及更高版本，您可以使用 Stream.CopyTo 方法：

```csharp
unpacked.CopyTo(extracted);
```

### 另请参阅

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


