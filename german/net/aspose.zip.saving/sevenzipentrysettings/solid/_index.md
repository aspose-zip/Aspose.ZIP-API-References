---
title: "SevenZipEntrySettings.Solid"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "SevenZipEntrySettings-Eigenschaft. Liest oder setzt einen Wert, der angibt, ob Einträge zusammengeführt und als ein einziger Datenblock behandelt werden sollen"
type: docs
weight: 50
url: /de/net/aspose.zip.saving/sevenzipentrysettings/solid/
---
## SevenZipEntrySettings.Solid property

Liest oder setzt den Wert, der angibt, ob Einträge zusammengeführt und als ein einzelner Datenblock behandelt werden sollen.

```csharp
public bool Solid { get; set; }
```

## Hinweise

Stellt `SevenZipEntrySettings` für ein festes 7z-Archiv bei der Instanziierung des Archivs bereit.

## Beispiele

Das folgende Beispiel zeigt, wie ein Verzeichnis zu einem festen 7z-Archiv mit LZMA2-Kompression ohne Verschlüsselung komprimiert wird.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings()){ Solid = true }))
    {
        archive.CreateEntries("C:\\Documents");
        archive.Save(sevenZipFile);
    }
}
```

### Siehe auch

* class [SevenZipEntrySettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipentrysettings/)
* assembly [Aspose.Zip](../../../)


