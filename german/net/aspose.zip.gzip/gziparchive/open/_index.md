---
title: GzipArchive.Open
second_title: Aspose.ZIP für .NET-API-Referenz
description: GzipArchive methode. Öffnet das Archiv zum Extrahieren und stellt einen Stream mit Archivinhalten bereit.
type: docs
weight: 50
url: /de/net/aspose.zip.gzip/gziparchive/open/
---
## GzipArchive.Open method

Öffnet das Archiv zum Extrahieren und stellt einen Stream mit Archivinhalten bereit.

```csharp
public Stream Open()
```

### Rückgabewert

Der Stream, der den Inhalt des Archivs darstellt.

### Bemerkungen

Aus dem Stream lesen, um den ursprünglichen Inhalt der Datei zu erhalten. Siehe Beispielabschnitt.

### Beispiele

Extrahiert das Archiv und kopiert den extrahierten Inhalt in den Dateistream.

Sie können die Stream.CopyTo-Methode für .NET 4.0 und höher verwenden:

```csharp
unpacked.CopyTo(extracted);
```

```csharp
using (var archive = new GzipArchive("archive.gz"))
{
    using (var extracted = File.Create("data.bin"))
    {
        var unpacked = archive.Open();
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = unpacked.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }            
}
```

### Siehe auch

* class [GzipArchive](../)
* namensraum [Aspose.Zip.Gzip](../../gziparchive/)
* Montage [Aspose.Zip](../../../)


