---
title: "GzipArchive.UncompressedSize"
second_title: "Aspose.ZIP för .NET API-referens"
description: "GzipArchive‑egenskap. Hämtar storleken på den ursprungliga filen."
type: docs
weight: 30
url: /sv/net/aspose.zip.gzip/gziparchive/uncompressedsize/
---
## GzipArchive.UncompressedSize property

Hämtar storleken på en originalfil.

```csharp
public ulong UncompressedSize { get; }
```

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Anmärkningar

Under dekomprimering kan denna egenskap innehålla felaktig storlek. Om den okomprimerade filstorleken överstiger 4 GB kommer egenskapen att ge ett felaktigt värde på grund av 32‑bitsgränsen i huvudet.

### Se även

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


