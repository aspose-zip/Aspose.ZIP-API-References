---
title: LzxArchiveEntry.Extract
second_title: Aspose.ZIP for .NET API Reference
description: LzxArchiveEntry method. Extracts Lzx archive entry to a filesystem by path
type: docs
weight: 80
url: /net/aspose.zip.lzx/lzxarchiveentry/extract/
---
## Extract(string) {#extract}

Extracts Lzx archive entry to a filesystem by path.

```csharp
public FileSystemInfo Extract(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | Path to file which will store decompressed data. |

### Return Value

FileSystemInfoInstance containing extracted data.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Archive headers and service information were not read. |
| ArgumentNullException | *path* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *path* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *path* is denied. |
| PathTooLongException | The specified *path*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *path* contains a colon (:) in the middle of the string. |
| InvalidDataException | Checksum mismatch for headers or data. - or - Archive is corrupted. |
| OperationCanceledException | In .NET Framework 4.0 and above: Thrown when the extraction is canceled via the provided cancellation token. |
| NotSupportedException | Invalid compression method. |

## Examples

```csharp
using (FileStream lzxFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzxArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### See Also

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extracts the entry to the stream provided.

```csharp
public void Extract(Stream destination)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destination | Stream | Destination stream. Must be writable. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *destination* does not support writing. |
| InvalidDataException | Checksum mismatch for headers or data. - or - Archive is corrupted. |
| ArgumentNullException | Destination stream is null. |
| NotSupportedException | Invalid compression method. |
| OperationCanceledException | In .NET Framework 4.0 and above: Thrown when the extraction is canceled via the provided cancellation token. |

### See Also

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)


