---
title: TarArchive.FromXz
second_title: Aspose.ZIP for .NET API Reference
description: TarArchive method. Extracts supplied xz format archive and composes TarArchive from extracted data
type: docs
weight: 60
url: /net/aspose.zip.tar/tararchive/fromxz/
---
## FromXz(Stream) {#fromxz}

Extracts supplied xz format archive and composes [`TarArchive`](../) from extracted data.

Important: xz archive is fully extracted within this method, its content is kept internally. Beware of memory consumption.

```csharp
public static TarArchive FromXz(Stream source)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Stream | The source of the archive. |

### Return Value

An instance of [`TarArchive`](../)

## Remarks

Tar archive provides facility to extract arbitrary record, so it has to operate seekable stream under the hood.

### See Also

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromXz(string) {#fromxz_1}

Extracts supplied xz format archive and composes [`TarArchive`](../) from extracted data.

Important: xz archive is fully extracted within this method, its content is kept internally. Beware of memory consumption.

```csharp
public static TarArchive FromXz(string path)
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
| ArgumentException | The *path* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *path* is denied. |
| PathTooLongException | The specified *path*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *path* is in an invalid format. |
| DirectoryNotFoundException | The specified path is invalid, such as being on an unmapped drive. |
| FileNotFoundException | The file is not found. |

## Remarks

Tar archive provides facility to extract arbitrary record, so it has to operate seekable stream under the hood.

### See Also

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


