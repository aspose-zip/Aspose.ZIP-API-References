---
title: TarArchive.FromZ
second_title: Aspose.ZIP for .NET API Reference
description: TarArchive method. Extracts supplied Z format archive and composes TarArchive from extracted data
type: docs
weight: 60
url: /net/aspose.zip.tar/tararchive/fromz/
---
## FromZ(Stream) {#fromz}

Extracts supplied Z format archive and composes [`TarArchive`](../) from extracted data.

Important: Z archive is fully extracted within this method, its content is kept internally. Beware of memory consumption.

```csharp
public static TarArchive FromZ(Stream source)
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

## FromZ(string) {#fromz_1}

Extracts supplied Z format archive and composes [`TarArchive`](../) from extracted data.

Important: Z archive is fully extracted within this method, its content is kept internally. Beware of memory consumption.

```csharp
public static TarArchive FromZ(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to the archive file. |

### Return Value

An instance of [`TarArchive`](../)

## Remarks

Tar archive provides facility to extract arbitrary record, so it has to operate seekable stream under the hood.

### See Also

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


