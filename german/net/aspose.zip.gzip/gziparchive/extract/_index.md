---
title: GzipArchive.Extract
second_title: Aspose.ZIP für .NET-API-Referenz
description: GzipArchive methode. Extrahiert das Archiv in den bereitgestellten Stream.
type: docs
weight: 40
url: /de/net/aspose.zip.gzip/gziparchive/extract/
---
## GzipArchive.Extract method

Extrahiert das Archiv in den bereitgestellten Stream.

```csharp
public void Extract(Stream destination)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destination | Stream | Zielstrom. Muss beschreibbar sein. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | *destination* unterstützt das Schreiben nicht. |

### Beispiele

```csharp
using (var archive = new GzipArchive("archive.gz"))
{
     archive.Extract(httpResponseStream);
}
```

### Siehe auch

* class [GzipArchive](../)
* namensraum [Aspose.Zip.Gzip](../../gziparchive/)
* Montage [Aspose.Zip](../../../)


