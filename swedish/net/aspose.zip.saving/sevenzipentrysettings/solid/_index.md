---
title: "SevenZipEntrySettings.Solid"
second_title: "Aspose.ZIP för .NET API-referens"
description: "SevenZipEntrySettings-egenskap. Hämtar eller anger värde som indikerar om poster ska sammanfogas och behandlas som ett enda datablock"
type: docs
weight: 50
url: /sv/net/aspose.zip.saving/sevenzipentrysettings/solid/
---
## SevenZipEntrySettings.Solid property

Hämtar eller anger ett värde som indikerar om poster ska sammanfogas och behandlas som ett enda datablock.

```csharp
public bool Solid { get; set; }
```

## Anmärkningar

Tillhandahåll `SevenZipEntrySettings` för solid 7z-arkiv vid arkivinstansiering.

## Exempel

Följande exempel visar hur man komprimerar en katalog till ett solid 7z-arkiv med LZMA2-komprimering utan kryptering.

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

### Se även

* class [SevenZipEntrySettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipentrysettings/)
* assembly [Aspose.Zip](../../../)


