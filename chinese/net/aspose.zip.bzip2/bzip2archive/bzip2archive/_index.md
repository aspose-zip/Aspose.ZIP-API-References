---
title: Bzip2Archive
second_title: Aspose.ZIP for .NET API 参考
description: 初始化准备压缩的Bzip2Archiveaspose.zip.bzip2/bzip2archive类的新实例
type: docs
weight: 10
url: /zh/net/aspose.zip.bzip2/bzip2archive/bzip2archive/
---
## Bzip2Archive() {#constructor}

初始化准备压缩的[`Bzip2Archive`](../../bzip2archive)类的新实例。

```csharp
public Bzip2Archive()
```

### 例子

以下示例显示如何压缩文件。

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### 也可以看看

* class [Bzip2Archive](../../bzip2archive)
* 命名空间 [Aspose.Zip.Bzip2](../../bzip2archive)
* 部件 [Aspose.Zip](../../../)

---

## Bzip2Archive(Stream) {#constructor_1}

初始化准备解压缩的[`Bzip2Archive`](../../bzip2archive)类的新实例。

```csharp
public Bzip2Archive(Stream sourceStream)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | Stream | 存档的来源。 |

### 评论

此构造函数不解压缩。参见[`Open`](../open)方法解压。

### 例子

从流中打开存档并将其解压缩到` MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive(File.OpenRead("archive.bz2")))
  archive.Open().CopyTo(ms);
```

### 也可以看看

* class [Bzip2Archive](../../bzip2archive)
* 命名空间 [Aspose.Zip.Bzip2](../../bzip2archive)
* 部件 [Aspose.Zip](../../../)

---

## Bzip2Archive(string) {#constructor_2}

初始化准备解压缩的[`Bzip2Archive`](../../bzip2archive)类的新实例。

```csharp
public Bzip2Archive(string path)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| path | String | 存档文件的路径。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *path*为空。 |
| SecurityException | 调用者没有访问所需的权限 |
| ArgumentException | *path*为空，仅包含空格，或包含无效字符。 |
| UnauthorizedAccessException | 对文件*path*的访问被拒绝。 |
| PathTooLongException | 指定的*path*、文件名或两者都超过了系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | *path*的文件在字符串中间包含一个冒号 (:)。 |

### 评论

此构造函数不解压缩。参见[`Open`](../open)方法解压。

### 例子

按路径从文件中打开存档并将其解压缩到` MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
  archive.Open().CopyTo(ms);
```

### 也可以看看

* class [Bzip2Archive](../../bzip2archive)
* 命名空间 [Aspose.Zip.Bzip2](../../bzip2archive)
* 部件 [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
