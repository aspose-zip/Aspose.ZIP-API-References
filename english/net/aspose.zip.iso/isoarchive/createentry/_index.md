---
title: IsoArchive.CreateEntry
second_title: Aspose.ZIP for .NET API Reference
description: IsoArchive method. Adds a file to the ISO image
type: docs
weight: 40
url: /net/aspose.zip.iso/isoarchive/createentry/
---
## CreateEntry(string, string) {#createentry_2}

Adds a file to the ISO image.

```csharp
public IsoEntry CreateEntry(string name, string filePath)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | Path of the file in the ISO. |
| filePath | String | Path of the file. |

### Return Value

The ISO entry composed.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | The *filePath* is null. |
| ArgumentException | The *filePath* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *filePath* is denied. |
| PathTooLongException | The specified *filePath* exceeds the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *filePath* contains a colon (:) in the middle of the string. |
| IOException | An I/O error occurred while opening the file. |

### See Also

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Adds a file to the ISO image.

```csharp
public IsoEntry CreateEntry(string name, Stream source)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | Path of the file in the ISO. |
| source | Stream | Stream containing the file data. |

### Return Value

The ISO entry composed.

### See Also

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string) {#createentry}

Adds a file to the ISO image.

```csharp
public IsoEntry CreateEntry(string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | Path of the directory in the ISO. |

### Return Value

The ISO entry composed.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | `name` is null or empty. |
| InvalidOperationException | The archive is opened for extraction. |

### See Also

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


