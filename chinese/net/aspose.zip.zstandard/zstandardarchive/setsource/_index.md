---
title: "ZstandardArchive.SetSource"
second_title: "Aspose.ZIP for .NET API 参考"
description: "ZstandardArchive 方法。设置要在存档中压缩的内容"
type: docs
weight: 70
url: /zh/net/aspose.zip.zstandard/zstandardarchive/setsource/
---
## SetSource(Stream) {#setsource_1}

设置要在存档中压缩的内容。

```csharp
public void SetSource(Stream source)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | 流 | 存档的输入流。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放，无法使用。 |

## 示例

```csharp
using (var archive = new ZstandardArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.zst");
}
```

### 另请参阅

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

设置要在存档中压缩的内容。

```csharp
public void SetSource(FileInfo fileInfo)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileInfo | FileInfo | 要压缩的文件的引用。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放，无法使用。 |

## 示例

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.zst");
}
```

### 另请参阅

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

设置要在存档中压缩的内容。

```csharp
public void SetSource(string path)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 要压缩的文件路径。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| ArgumentNullException | *path* 为 null。 |
| SecurityException | 调用方没有访问所需的权限。 |
| ArgumentException | 该 *path* 为空，仅包含空白字符，或包含无效字符。 |
| UnauthorizedAccessException | 对文件 *path* 的访问被拒绝。 |
| PathTooLongException | 指定的 *path*、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 位于 *path* 的文件在字符串中间包含冒号 (:)。 |

## 示例

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.zst");
}
```

### 另请参阅

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


