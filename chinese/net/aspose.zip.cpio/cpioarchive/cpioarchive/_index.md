---
title: CpioArchive.CpioArchive
second_title: Aspose.ZIP for .NET API 参考
description: CpioArchive 构造函数. 初始化一个新的实例CpioArchive类.
type: docs
weight: 10
url: /zh/net/aspose.zip.cpio/cpioarchive/cpioarchive/
---
## CpioArchive() {#constructor}

初始化一个新的实例[`CpioArchive`](../)类.

```csharp
public CpioArchive()
```

### 例子

以下示例显示了如何压缩文件。

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### 也可以看看

* class [CpioArchive](../)
* 命名空间 [Aspose.Zip.Cpio](../../cpioarchive/)
* 部件 [Aspose.Zip](../../../)

---

## CpioArchive(Stream) {#constructor_1}

初始化一个新的实例[`CpioArchive`](../)可以从存档中提取类和组合条目列表。

```csharp
public CpioArchive(Stream sourceStream)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | Stream | 存档的来源。它必须是可寻的。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *sourceStream*一片空白。 |
| ArgumentException | *sourceStream*不可搜索。 |
| InvalidDataException | *sourceStream*不是有效的 cpio 存档。 |

### 评论

此构造函数不解压任何条目。看[`Open`](../../cpioentry/open/)解包方法.

### 例子

以下示例显示如何将所有条目提取到目录中。

```csharp
using (var archive = new CpioArchive(File.OpenRead("archive.cpio")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### 也可以看看

* class [CpioArchive](../)
* 命名空间 [Aspose.Zip.Cpio](../../cpioarchive/)
* 部件 [Aspose.Zip](../../../)

---

## CpioArchive(string) {#constructor_2}

初始化一个新的实例[`CpioArchive`](../)可以从存档中提取类和组合条目列表。

```csharp
public CpioArchive(string path)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| path | String | 存档文件的路径。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *path*一片空白。 |
| SecurityException | 调用者没有所需的访问权限。 |
| ArgumentException | 这*path*为空、仅包含空格或包含无效字符。 |
| UnauthorizedAccessException | 访问文件*path*被拒绝。 |
| PathTooLongException | 指定的*path*、文件名或两者都超过了系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 归档于*path*在字符串中间包含一个冒号 (:)。 |

### 评论

此构造函数不解压任何条目。看[`Open`](../../cpioentry/open/)解包方法.

### 例子

以下示例显示如何将所有条目提取到目录中。

```csharp
using (var archive = new CpioArchive("archive.cpio")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### 也可以看看

* class [CpioArchive](../)
* 命名空间 [Aspose.Zip.Cpio](../../cpioarchive/)
* 部件 [Aspose.Zip](../../../)


