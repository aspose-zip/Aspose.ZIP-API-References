---
title: "GzipArchive.UncompressedSize"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "GzipArchive property. Haalt de grootte op van een origineel bestand"
type: docs
weight: 30
url: /nl/net/aspose.zip.gzip/gziparchive/uncompressedsize/
---
## GzipArchive.UncompressedSize property

Haalt de grootte van een origineel bestand op.

```csharp
public ulong UncompressedSize { get; }
```

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |

## Opmerkingen

Tijdens decompressie kan deze eigenschap een onjuiste grootte bevatten. Als de grootte van het gedecomprimeerde bestand 4 GB overschrijdt, zal deze eigenschap een verkeerde waarde geven vanwege de 32‑bit limiet in de header.

### Zie ook

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


