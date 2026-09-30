---
title: "Lz4Archive.SetSource"
second_title: "Aspose.ZIP for .NET API 参考"
description: "Lz4Archive 方法。设置要在归档中压缩的内容"
type: docs
weight: 70
url: /zh/net/aspose.zip.lz4/lz4archive/setsource/
---
## SetSource(Stream) {#setsource_2}

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
| InvalidOperationException | 已准备好进行提取的归档。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |

## 示例

```csharp
using (var archive = new Lz4Archive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.lz4");
}
```

### 另请参阅

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

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
| InvalidOperationException | 已准备好进行提取的归档。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |

## 示例

从流中打开存档并将其提取到 `MemoryStream`

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.lz4");
}
```

### 另请参阅

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(TarArchive, TarFormat) {#setsource}

设置要在存档中压缩的内容。

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| tarArchive | TarArchive | 要压缩的 Tar 归档。 |
| 格式 | TarFormat | 定义 tar 头部格式。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| InvalidOperationException | 此归档已准备好进行提取。 |

## 备注

使用此方法组合联合 tar.lz4 归档。

## 示例

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var lz4Archive = new Lz4Archive())
    {
        lz4Archive.SetSource(tarArchive);
        lz4Archive.Save("archive.tar.lz4");
    }
}
```

### 另请参阅

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* enum [TarFormat](../../../aspose.zip.tar/tarformat/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

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
| ArgumentNullException | *path* 为 null。 |
| SecurityException | 调用者没有访问所需的权限 |
| ArgumentException | 该 *path* 为空，仅包含空白字符，或包含无效字符。 |
| UnauthorizedAccessException | 对文件 *path* 的访问被拒绝。 |
| PathTooLongException | 指定的 *path*、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 位于 *path* 的文件在字符串中间包含冒号 (:)。 |
| InvalidOperationException | 此归档已准备好进行提取。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |

## 示例

通过路径从文件打开存档并将其提取到 `MemoryStream`

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### 另请参阅

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


