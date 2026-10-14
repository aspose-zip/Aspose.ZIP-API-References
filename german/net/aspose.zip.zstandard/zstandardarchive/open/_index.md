---
title: "ZstandardArchive.Open"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "ZstandardArchive-Methode. Öffnet das Archiv zur Extraktion und stellt einen Stream mit dem Archivinhalt bereit."
type: docs
weight: 50
url: /de/net/aspose.zip.zstandard/zstandardarchive/open/
---
## ZstandardArchive.Open method

Öffnet das Archiv zum Extrahieren und stellt einen Stream mit dem Archivinhalt bereit.

```csharp
public Stream Open()
```

### Rückgabewert

Der Stream, der den Inhalt des Archivs darstellt.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

## Hinweise

Lesen Sie aus dem Stream, um den ursprünglichen Inhalt einer Datei zu erhalten. Siehe den Abschnitt Beispiele.

## Beispiele

Extrahiert das Archiv und kopiert den extrahierten Inhalt in den Dateistream.

```csharp
using (var archive = new ZstandardArchive("archive.zst"))
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

Sie können die Stream.CopyTo-Methode für .NET 4.0 und höher verwenden:

```csharp
unpacked.CopyTo(extracted);
```

### Siehe auch

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


