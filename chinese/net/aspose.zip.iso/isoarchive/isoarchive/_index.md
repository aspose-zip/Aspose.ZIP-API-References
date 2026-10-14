---
title: "IsoArchive.IsoArchive"
second_title: "Aspose.ZIP for .NET API 参考"
description: "IsoArchive 构造函数。初始化 IsoArchive 类的新实例，并创建一个空的 ISO 存档以添加新文件和目录。"
type: docs
weight: 10
url: /zh/net/aspose.zip.iso/isoarchive/isoarchive/
---
## IsoArchive() {#constructor}

初始化 [`IsoArchive`](../) 类的新实例，并创建一个空的 ISO 存档以添加新文件和目录。

```csharp
public IsoArchive()
```

## 示例

下面的示例展示了如何创建一个新的空 ISO 存档并向其中添加文件：

```csharp
// 创建一个新的空 ISO 存档
using(IsoArchive isoArchive = new IsoArchive())
{
    // 向 ISO 存档添加文件
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // 将 ISO 存档保存到文件
    isoArchive.Save("new_archive.iso");
}
```

### 另请参阅

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(Stream, IsoLoadOptions) {#constructor_1}

初始化 [`IsoArchive`](../) 类的新实例，并生成可从存档中提取的条目列表。

```csharp
public IsoArchive(Stream sourceStream, IsoLoadOptions loadOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | 流 | 存档的来源。必须支持定位。 |
| loadOptions | IsoLoadOptions | 用于加载存档的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *sourceStream* 为 null。 |
| ArgumentException | *sourceStream* 不支持定位。 |
| InvalidDataException | *sourceStream* 不是有效的 ISO 存档。 |
| ObjectDisposedException | 如果源流已被释放，则抛出此异常。 |
| EndOfStreamException | 当意外到达流的末尾时抛出此异常。 |
| IOException | 发生 I/O 错误。 |
| NotSupportedException | 该流不支持读取。 |

## 备注

此构造函数不会解压任何条目。

## 示例

下面的示例展示了如何将所有条目提取到目录中。

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### 另请参阅

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(string, IsoLoadOptions) {#constructor_2}

初始化 [`IsoArchive`](../) 类的新实例，并生成可从存档中提取的条目列表。

```csharp
public IsoArchive(string path, IsoLoadOptions loadOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 存档文件的路径。 |
| loadOptions | IsoLoadOptions | 用于加载存档的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *path* 为 null。 |
| SecurityException | 调用方没有访问所需的权限。 |
| ArgumentException | 该 *path* 为空，仅包含空白字符，或包含无效字符。 |
| UnauthorizedAccessException | 对文件 *path* 的访问被拒绝。 |
| PathTooLongException | 指定的 *path*、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 位于 *path* 的文件在字符串中间包含冒号 (:)。 |
| FileNotFoundException | 未找到该文件。 |
| DirectoryNotFoundException | 指定的路径无效，例如位于未映射的驱动器上。 |
| IOException | 该文件已打开。 |
| EndOfStreamException | 该文件太短。 |
| InvalidDataException | 当数据无效或损坏时抛出。 |

## 备注

此构造函数不会解压任何条目。

## 示例

下面的示例展示了如何将所有条目提取到目录中。

```csharp
using (var archive = new IsoArchive("archive.iso")) 
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### 另请参阅

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


