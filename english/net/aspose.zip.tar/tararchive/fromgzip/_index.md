---
title: TarArchive.FromGZip
second_title: Aspose.ZIP for .NET API Reference
description: TarArchive method. Extracts supplied gzip archive and composes TarArchive from extracted data
type: docs
weight: 20
url: /net/aspose.zip.tar/tararchive/fromgzip/
---
## FromGZip(Stream) {#fromgzip}

Extracts supplied gzip archive and composes [`TarArchive`](../) from extracted data.

Important: gzip archive is fully extracted within this method, its content is kept internally. Beware of memory consumption.

```csharp
public static TarArchive FromGZip(Stream source)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Stream | The source of the archive. |

### Return Value

An instance of [`TarArchive`](../)

### Exceptions

| exception | condition |
| --- | --- |
| InvalidDataException | Archive is corrupted. |

## Remarks

GZip extraction stream is not seekable by the nature of compression algorithm. Tar archive provides facility to extract arbitrary record, so it has to operate seekable stream under the hood.

### See Also

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromGZip(string) {#fromgzip_1}

Extracts supplied gzip archive and composes [`TarArchive`](../) from extracted data.

Important: gzip archive is fully extracted within this method, its content is kept internally. Beware of memory consumption.

```csharp
public static TarArchive FromGZip(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to the archive file. |

### Return Value

An instance of [`TarArchive`](../)

### Exceptions

| exception | condition |
| --- | --- |
| InvalidDataException | Archive is corrupted. |

## Remarks

GZip extraction stream is not seekable by the nature of compression algorithm. Tar archive provides facility to extract arbitrary record, so it has to operate seekable stream under the hood.

### See Also

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


