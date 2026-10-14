---
title: "UueArchive.UueArchive"
second_title: "Aspose.ZIP for .NET API 参考"
description: "UueArchive 构造函数。初始化一个准备进行编码的 UueArchive 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.zip.uue/uuearchive/uuearchive/
---
## UueArchive() {#constructor}

初始化一个准备进行编码的 [`UueArchive`](../) 类的新实例。

```csharp
public UueArchive()
```

## 示例

以下示例展示了如何对文件进行 uuencode。

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.uue");
}
```

### 另请参阅

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(Stream) {#constructor_1}

初始化一个准备进行解码的 [`UueArchive`](../) 类的新实例。

```csharp
public UueArchive(Stream sourceStream)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | 流 | 存档的来源。 |

## 备注

此构造函数不进行解码。请参阅 [`Open`](../open/) 方法以进行解压缩。

## 示例

从流中打开存档并将其提取到 `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive(File.OpenRead("archive.001")))
  archive.Open().CopyTo(ms);
```

### 另请参阅

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(string) {#constructor_2}

初始化一个 [`UueArchive`](../) 类的新实例。

```csharp
public UueArchive(string path)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 存档文件的路径。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *path* 为 null。 |
| SecurityException | 调用方没有访问所需的权限。 |
| ArgumentException | 该 *path* 为空，仅包含空白字符，或包含无效字符。 |
| UnauthorizedAccessException | 对文件 *path* 的访问被拒绝。 |
| PathTooLongException | 指定的 *path*、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 位于 *path* 的文件在字符串中间包含冒号 (:)。 |
| DirectoryNotFoundException | 指定的路径无效，例如位于未映射的驱动器上。 |
| FileNotFoundException | 未找到该文件。 |
| IOException | 该文件已打开。 |

## 备注

此构造函数不进行解压缩。请参阅 [`Open`](../open/) 方法以进行解压缩。

## 示例

通过路径从文件打开归档并将其解码为 `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive("archive.uue"))
  archive.Open().CopyTo(ms);
```

### 另请参阅

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


