---
title: TarArchive.FromLZip
second_title: Aspose.ZIP for .NET API Reference
description: TarArchive method. Extracts supplied lzip archive and composes TarArchive from extracted data
type: docs
weight: 30
url: /net/aspose.zip.tar/tararchive/fromlzip/
---
## FromLZip(Stream) {#fromlzip}

Extracts supplied lzip archive and composes [`TarArchive`](../) from extracted data.

Important: lzip archive is fully extracted within this method, its content is kept internally. Beware of memory consumption.

```csharp
public static TarArchive FromLZip(Stream source)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Stream | The source of the archive. |

### Return Value

An instance of [`TarArchive`](../)

## Remarks

Lzip extraction stream is not seekable by the nature of compression algorithm. Tar archive provides facility to extract arbitrary record, so it has to operate seekable stream under the hood.

### See Also

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZip(string) {#fromlzip_1}

Extracts supplied lzip archive and composes [`TarArchive`](../) from extracted data.

Important: lzip archive is fully extracted within this method, its content is kept internally. Beware of memory consumption.

```csharp
public static TarArchive FromLZip(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to the archive file. |

### Return Value

An instance of [`TarArchive`](../)

## Remarks

Lzip extraction stream is not seekable by the nature of compression algorithm. Tar archive provides facility to extract arbitrary record, so it has to operate seekable stream under the hood.

### See Also

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


