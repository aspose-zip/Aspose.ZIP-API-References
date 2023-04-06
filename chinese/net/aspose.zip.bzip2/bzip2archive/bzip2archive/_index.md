---
title: Bzip2Archive.Bzip2Archive
second_title: Aspose.ZIP for .NET API 参考
description: Bzip2Archive 构造函数. 初始化一个新的实例Bzip2Archive准备压缩的类.
type: docs
weight: 10
url: /zh/net/aspose.zip.bzip2/bzip2archive/bzip2archive/
---
## Bzip2Archive() {#constructor}

初始化一个新的实例[`Bzip2Archive`](../)准备压缩的类.

```csharp
public Bzip2Archive()
```

### 例子

以下示例显示了如何压缩文件。

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### 也可以看看

* class [Bzip2Archive](../)
* 命名空间 [Aspose.Zip.Bzip2](../../bzip2archive/)
* 部件 [Aspose.Zip](../../../)

---

## Bzip2Archive(Stream) {#constructor_1}

初始化一个新的实例[`Bzip2Archive`](../)准备解压的类.

```csharp
public Bzip2Archive(Stream sourceStream)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | Stream | 存档的来源。 |

### 评论

此构造函数不解压缩。看[`Open`](../open/)解压方法.

### 例子

从流中打开存档并将其提取到`内存流`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive(File.OpenRead("archive.bz2")))
  archive.Open().CopyTo(ms);
```

### 也可以看看

* class [Bzip2Archive](../)
* 命名空间 [Aspose.Zip.Bzip2](../../bzip2archive/)
* 部件 [Aspose.Zip](../../../)

---

## Bzip2Archive(string) {#constructor_2}

初始化一个新的实例[`Bzip2Archive`](../)准备解压的类.

```csharp
public Bzip2Archive(string path)
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

此构造函数不解压缩。看[`Open`](../open/)解压方法.

### 例子

按路径从文件中打开存档并将其解压缩到`内存流`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
  archive.Open().CopyTo(ms);
```

### 也可以看看

* class [Bzip2Archive](../)
* 命名空间 [Aspose.Zip.Bzip2](../../bzip2archive/)
* 部件 [Aspose.Zip](../../../)


