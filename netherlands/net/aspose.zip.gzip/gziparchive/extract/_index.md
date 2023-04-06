---
title: GzipArchive.Extract
second_title: Aspose.ZIP voor .NET API-referentie
description: GzipArchive methode. Pakt het archief uit naar de geleverde stream.
type: docs
weight: 40
url: /nl/net/aspose.zip.gzip/gziparchive/extract/
---
## GzipArchive.Extract method

Pakt het archief uit naar de geleverde stream.

```csharp
public void Extract(Stream destination)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destination | Stream | Bestemmingsstroom. Moet beschrijfbaar zijn. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentException | *destination* ondersteunt schrijven niet. |

### Voorbeelden

```csharp
using (var archive = new GzipArchive("archive.gz"))
{
     archive.Extract(httpResponseStream);
}
```

### Zie ook

* class [GzipArchive](../)
* naamruimte [Aspose.Zip.Gzip](../../gziparchive/)
* montage [Aspose.Zip](../../../)


