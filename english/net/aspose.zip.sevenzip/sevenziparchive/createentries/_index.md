---
title: SevenZipArchive.CreateEntries
second_title: Aspose.ZIP for .NET API Reference
description: SevenZipArchive method. Adds to the archive all files and directories recursively in the directory given
type: docs
weight: 40
url: /net/aspose.zip.sevenzip/sevenziparchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Adds to the archive all files and directories recursively in the directory given.

```csharp
public SevenZipArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Type | Description |
| --- | --- | --- |
| directory | DirectoryInfo | Directory to compress. |
| includeRootDirectory | Boolean | Indicates whether to include the root directory itself or not. |

### Return Value

The archive with entries composed.

### Exceptions

| exception | condition |
| --- | --- |
| DirectoryNotFoundException | The path to *directory* is invalid, such as being on an unmapped drive. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |
| SecurityException | The caller does not have the required permission to access *directory*. |

## Examples

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.7z");
}
```

### See Also

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Adds to the archive all files and directories recursively in the directory given.

```csharp
public SevenZipArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | String | Directory to compress. |
| includeRootDirectory | Boolean | Indicates whether to include the root directory itself or not. |

### Return Value

The archive with entries composed.

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

## Examples

Compose 7z archive with LZMA2 compression.

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.7z");
}
```

### See Also

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


