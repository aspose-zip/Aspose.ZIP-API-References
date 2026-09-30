---
title: "IsoArchive.ExtractToDirectory"
second_title: "Aspose.ZIP for .NET API 参考"
description: "IsoArchive 方法。将所有条目提取到指定目录"
type: docs
weight: 60
url: /zh/net/aspose.zip.iso/isoarchive/extracttodirectory/
---
## IsoArchive.ExtractToDirectory method

将所有条目提取到指定目录。

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationDirectory | String | 用于提取条目的目录。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| InvalidOperationException | 当存档处于编辑模式时抛出。 |
| ArgumentNullException | 当 *destinationDirectory* 为 null 时抛出。 |
| OperationCanceledException | 在 .NET Framework 4.0 及以上版本：当通过提供的取消令牌取消提取时抛出。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |

## 示例

下面的示例展示了如何将所有条目提取到目录：

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### 另请参阅

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


