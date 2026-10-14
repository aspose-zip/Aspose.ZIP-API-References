---
title: "AlzArchive.AlzArchive"
second_title: "Aspose.ZIP for .NET API 参考"
description: "AlzArchive 构造函数。根据流初始化 AlzArchive 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.zip.alz/alzarchive/alzarchive/
---
## AlzArchive(Stream, AlzArchiveLoadOptions) {#constructor}

从流初始化一个新的 [`AlzArchive`](../) 类实例。

```csharp
public AlzArchive(Stream stream, AlzArchiveLoadOptions loadOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | ALZ 存档流。该流必须支持读取和定位。 |
| loadOptions | AlzArchiveLoadOptions | 用于加载现有存档的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | 流为 null。 |

### 另请参阅

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)

---

## AlzArchive(string, AlzArchiveLoadOptions) {#constructor_1}

从文件路径初始化一个新的 [`AlzArchive`](../) 类实例。

```csharp
public AlzArchive(string filePath, AlzArchiveLoadOptions loadOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件路径 | String | ALZ 存档文件的路径。 |
| loadOptions | AlzArchiveLoadOptions | 用于加载现有存档的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | filePath 为 null。 |
| FileNotFoundException | 文件不存在。 |

### 另请参阅

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)


