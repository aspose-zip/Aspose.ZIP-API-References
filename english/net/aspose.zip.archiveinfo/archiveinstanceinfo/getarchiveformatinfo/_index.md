---
title: ArchiveInstanceInfo.GetArchiveFormatInfo
second_title: Aspose.ZIP for .NET API Reference
description: ArchiveInstanceInfo method. Gets archive format info
type: docs
weight: 50
url: /net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveformatinfo/
---
## GetArchiveFormatInfo(string) {#getarchiveformatinfo_1}

Gets archive format info.

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The filename of the archive file. |

### Return Value

Information about archive format.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *fileName* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *fileName* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *fileName* is denied. |
| PathTooLongException | The specified *fileName* exceeds the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *fileName* contains a colon (:) in the middle of the string. |
| IOException | An I/O error occurred while opening the file. |

### See Also

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* assembly [Aspose.Zip](../../../)

---

## GetArchiveFormatInfo(Stream) {#getarchiveformatinfo}

Gets archive format info.

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream of the archive file. |

### Return Value

Information about archive format.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *stream* is null. |
| ArgumentException | *stream* is not seekable. |

### See Also

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* assembly [Aspose.Zip](../../../)


