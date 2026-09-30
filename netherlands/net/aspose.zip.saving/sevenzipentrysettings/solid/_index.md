---
title: "SevenZipEntrySettings.Solid"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "SevenZipEntrySettings eigenschap. Haalt op of stelt een waarde in die aangeeft of items moeten worden aaneengeschakeld en behandeld als één enkel datablock"
type: docs
weight: 50
url: /nl/net/aspose.zip.saving/sevenzipentrysettings/solid/
---
## SevenZipEntrySettings.Solid property

Haalt op of stelt de waarde in die aangeeft of items moeten worden samengevoegd en behandeld als één enkel gegevensblok.

```csharp
public bool Solid { get; set; }
```

## Opmerkingen

Voorzie `SevenZipEntrySettings` voor een solide 7z-archief bij het instantieren van het archief.

## Voorbeelden

Het volgende voorbeeld toont hoe een map te comprimeren naar een solide 7z-archief met LZMA2-compressie zonder versleuteling.

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

### Zie ook

* class [SevenZipEntrySettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipentrysettings/)
* assembly [Aspose.Zip](../../../)


