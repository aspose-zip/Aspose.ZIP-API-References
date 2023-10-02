---
title: ArchiveInstanceInfo.GetArchiveInstanceInfo
second_title: Aspose.ZIP for .NET API Reference
description: ArchiveInstanceInfo method. Gets archive instance info
type: docs
weight: 10
url: /net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveinstanceinfo/
---
## GetArchiveInstanceInfo(string) {#getarchiveinstanceinfo_1}

Gets archive instance info.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The filename of the archive file. |

### Return Value

Information about archive instance or null if format was not detected.

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

* class [ArchiveInstanceInfo](../)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* assembly [Aspose.Zip](../../../)

---

## GetArchiveInstanceInfo(Stream) {#getarchiveinstanceinfo}

Gets archive instance info.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream of the archive file. |

### Return Value

Information about archive instance or null if format was not detected.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *stream* is null. |
| ArgumentException | *stream* is not seekable. |

### See Also

* class [ArchiveInstanceInfo](../)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* assembly [Aspose.Zip](../../../)


