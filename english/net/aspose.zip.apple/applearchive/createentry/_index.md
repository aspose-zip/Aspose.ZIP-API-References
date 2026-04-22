---
title: AppleArchive.CreateEntry
second_title: Aspose.ZIP for .NET API Reference
description: AppleArchive method. Creates a single entry within the archive
type: docs
weight: 50
url: /net/aspose.zip.apple/applearchive/createentry/
---
## CreateEntry(string, string, bool) {#createentry_2}

Creates a single entry within the archive.

```csharp
public AppleArchiveEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the entry. |
| path | String | The path to the file to compress. |
| openImmediately | Boolean | True, if open the file immediately, otherwise open the file on archive saving. |

### Return Value

Apple Archive entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | The archive has been disposed. |
| ArgumentException | *name* is empty. |
| ArgumentNullException | *path* is `null`. |

### See Also

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Creates a single entry within the archive.

```csharp
public AppleArchiveEntry CreateEntry(string name, Stream source)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the entry. |
| source | Stream | The input stream for the entry. |

### Return Value

Apple Archive entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | The archive has been disposed. |
| ArgumentException | *name* is empty. |
| ArgumentNullException | *source* is `null`. |

### See Also

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Creates a single entry within the archive.

```csharp
public AppleArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the entry. |
| fileInfo | FileInfo | The metadata of file to be compressed. |
| openImmediately | Boolean | True, if open the file immediately, otherwise open the file on archive saving. |

### Return Value

Apple Archive entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | The archive has been disposed. |
| ArgumentException | *name* is empty. |
| ArgumentNullException | *fileInfo* is `null`. |

### See Also

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


