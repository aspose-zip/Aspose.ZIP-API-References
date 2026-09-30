---
title: "AppleArchive.CreateEntry"
second_title: "Aspose.ZIP for .NET API 参考"
description: "AppleArchive 方法。创建存档中的单个条目"
type: docs
weight: 60
url: /zh/net/aspose.zip.apple/applearchive/createentry/
---
## CreateEntry(string, string, bool) {#createentry_2}

在存档中创建单个条目。

```csharp
public AppleArchiveEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| 路径 | String | 要压缩的文件路径。 |
| openImmediately | Boolean | 如果立即打开文件则为 True，否则在存档保存时打开文件。 |

### Return Value

Apple Archive 条目实例。

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放。 |
| ArgumentException | *name* 为空。 |
| ArgumentNullException | *path* 为 `null`。 |

### 另请参阅

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

在存档中创建单个条目。

```csharp
public AppleArchiveEntry CreateEntry(string name, Stream source)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| source | 流 | 条目的输入流。 |

### Return Value

Apple Archive 条目实例。

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放。 |
| ArgumentException | *name* 为空。 |
| ArgumentNullException | *source* 为 `null`。 |

### 另请参阅

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

在存档中创建单个条目。

```csharp
public AppleArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| fileInfo | FileInfo | 待压缩文件的元数据。 |
| openImmediately | Boolean | 如果立即打开文件则为 True，否则在存档保存时打开文件。 |

### Return Value

Apple Archive 条目实例。

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放。 |
| ArgumentException | *name* 为空。 |
| ArgumentNullException | *fileInfo* 为 `null`。 |

### 另请参阅

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


