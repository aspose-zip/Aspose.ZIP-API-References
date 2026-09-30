---
title: "AppleArchive.AppleArchive"
second_title: "Aspose.ZIP for .NET API 参考"
description: "AppleArchive 构造函数。初始化一个使用用于已组成条目的设置的 AppleArchive 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.zip.apple/applearchive/applearchive/
---
## AppleArchive(AppleArchiveEntrySettings) {#constructor}

初始化一个使用用于已组成条目的设置的 [`AppleArchive`](../) 类的新实例。

```csharp
public AppleArchive(AppleArchiveEntrySettings newEntrySettings = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| newEntrySettings | AppleArchiveEntrySettings | 在组成新的 Apple Archive 时使用的设置。 |

### 另请参阅

* class [AppleArchiveEntrySettings](../../applearchiveentrysettings/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(Stream, AppleArchiveLoadOptions) {#constructor_1}

初始化一个 [`AppleArchive`](../) 类的新实例，并组成可以从存档中提取的条目列表。

```csharp
public AppleArchive(Stream sourceStream, AppleArchiveLoadOptions loadOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | 流 | 存档的来源。 |
| loadOptions | AppleArchiveLoadOptions | 用于加载现有存档的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *sourceStream* 为 null。 |
| ArgumentException | *sourceStream* 不支持定位。 |
| InvalidDataException | *sourceStream* 不是有效的 Apple Archive。 |
| EndOfStreamException | 在解析存档条目期间，流意外结束。 |

## 备注

此构造函数不会解压任何条目。请参阅用于解压的 [`ExtractToDirectory`](../extracttodirectory/) 和 [`Open`](../../applearchiveentry/open/) 方法。

### 另请参阅

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(string, AppleArchiveLoadOptions) {#constructor_2}

初始化一个 [`AppleArchive`](../) 类的新实例，并组成可以从存档中提取的条目列表。

```csharp
public AppleArchive(string path, AppleArchiveLoadOptions loadOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 归档文件的完全限定路径或相对路径。 |
| loadOptions | AppleArchiveLoadOptions | 用于加载现有存档的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *path* 为 null。 |
| FileNotFoundException | 未找到该文件。 |
| InvalidDataException | *path* 不是有效的 Apple Archive。 |
| EndOfStreamException | 在解析存档条目期间，流意外结束。 |

## 备注

此构造函数不会解压任何条目。请参阅用于解压的 [`ExtractToDirectory`](../extracttodirectory/) 和 [`Open`](../../applearchiveentry/open/) 方法。

### 另请参阅

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


