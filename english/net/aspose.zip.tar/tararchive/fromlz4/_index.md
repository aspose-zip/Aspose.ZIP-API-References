---
title: TarArchive.FromLZ4
second_title: Aspose.ZIP for .NET API Reference
description: TarArchive method. Extracts supplied LZ4 archive and composes TarArchive from extracted data
type: docs
weight: 30
url: /net/aspose.zip.tar/tararchive/fromlz4/
---
## FromLZ4(string) {#fromlz4_1}

Extracts supplied LZ4 archive and composes [`TarArchive`](../) from extracted data.

Important: LZ4 archive is fully extracted within this method, its content is kept internally. Beware of memory consumption.

```csharp
public static TarArchive FromLZ4(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to the archive file. |

### Return Value

An instance of [`TarArchive`](../)

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* is null. |
| SecurityException | The caller does not have the required permission to access |
| ArgumentException | The *path* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *path* is denied. |
| PathTooLongException | The specified *path*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *path* is in an invalid format. |
| DirectoryNotFoundException | The specified path is invalid, such as being on an unmapped drive. |
| FileNotFoundException | The file is not found. |
| EndOfStreamException | The file is too short. |
| InvalidDataException | The file has the wrong signature. |

## Remarks

LZ4 extraction stream is not seekable by the nature of compression algorithm. Tar archive provides facility to extract arbitrary record, so it has to operate seekable stream under the hood.

### See Also

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZ4(Stream) {#fromlz4}

Extracts supplied LZ4 archive and composes [`TarArchive`](../) from extracted data.

Important: LZ4 archive is fully extracted within this method, its content is kept internally. Beware of memory consumption.

```csharp
public static TarArchive FromLZ4(Stream source)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Stream | The source of the archive. |

### Return Value

An instance of [`TarArchive`](../)

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Cannot read from *source* |
| ArgumentNullException | *source* is null. |
| EndOfStreamException | *source* is too short. |
| InvalidDataException | The *source* has the wrong signature. |

## Remarks

LZ4 extraction stream is not seekable by the nature of compression algorithm. Tar archive provides facility to extract arbitrary record, so it has to operate seekable stream under the hood.

### See Also

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


