---
title: TarArchive.FromLZMA
second_title: Aspose.ZIP for .NET API Reference
description: TarArchive method. Extracts supplied LZMA archive and composes TarArchive from extracted data
type: docs
weight: 40
url: /net/aspose.zip.tar/tararchive/fromlzma/
---
## FromLZMA(Stream) {#fromlzma}

Extracts supplied LZMA archive and composes [`TarArchive`](../) from extracted data.

Important: LZMA archive is fully extracted within this method, its content is kept internally. Beware of memory consumption.

```csharp
public static TarArchive FromLZMA(Stream source)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Stream | The source of the archive. |

### Return Value

An instance of [`TarArchive`](../)

## Remarks

LZMA extraction stream is not seekable by the nature of compression algorithm. Tar archive provides facility to extract arbitrary record, so it has to operate seekable stream under the hood.

### See Also

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZMA(string) {#fromlzma_1}

Extracts supplied LZMA archive and composes [`TarArchive`](../) from extracted data.

Important: LZMA archive is fully extracted within this method, its content is kept internally. Beware of memory consumption.

```csharp
public static TarArchive FromLZMA(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to the archive file. |

### Return Value

An instance of [`TarArchive`](../)

## Remarks

LZMA extraction stream is not seekable by the nature of compression algorithm. Tar archive provides facility to extract arbitrary record, so it has to operate seekable stream under the hood.

### See Also

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


