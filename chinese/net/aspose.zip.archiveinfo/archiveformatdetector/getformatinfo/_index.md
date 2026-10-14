---
title: "GetFormatInfo"
second_title: "Aspose.ZIP for .NET API 参考"
description: 
type: docs
weight: 20
url: /zh/net/aspose.zip.archiveinfo/archiveformatdetector/getformatinfo/
---
## ArchiveFormatDetector.GetFormatInfo method (1 of 2)

获取格式信息。

```csharp
public ArchiveFormatInfo GetFormatInfo(string fileName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | String | 存档文件的文件名。 |

### Return Value

关于存档格式的信息，如果未检测到格式则为 null。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *fileName* 为 null。 |
| SecurityException | 调用方没有访问所需的权限。 |
| ArgumentException | *fileName* 为空，仅包含空白字符，或包含无效字符。 |
| UnauthorizedAccessException | 对文件 *fileName* 的访问被拒绝。 |
| PathTooLongException | 指定的 *fileName* 超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | *fileName* 处的文件在字符串中间包含冒号 (:)。 |
| IOException | 打开文件时发生 I/O 错误。 |

### 另请参阅

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

---

## ArchiveFormatDetector.GetFormatInfo method (2 of 2)

获取格式信息。

```csharp
public ArchiveFormatInfo GetFormatInfo(Stream stream)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 存档文件的流。 |

### Return Value

关于存档格式的信息，如果未检测到格式则为 null。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *stream* 为 null。 |
| ArgumentException | *stream* 不可定位。 |

### 另请参阅

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

<!-- 请勿编辑：由 xmldocmd 为 Aspose.Zip.dll 生成 -->
