---
title: SplitSevenZipArchiveSaveOptions.SplitSevenZipArchiveSaveOptions
second_title: Aspose.ZIP för .NET API-referens
description: SplitSevenZipArchiveSaveOptions byggare. Instantierar inställningar för att spara ett 7zarkiv med flera volymer.
type: docs
weight: 10
url: /sv/net/aspose.zip.saving/splitsevenziparchivesaveoptions/splitsevenziparchivesaveoptions/
---
## SplitSevenZipArchiveSaveOptions constructor

Instantierar inställningar för att spara ett 7z-arkiv med flera volymer.

```csharp
public SplitSevenZipArchiveSaveOptions(string fileName, uint segmentSize)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | Namn på volymer. Kan vara med eller utan förlängning .7z. |
| segmentSize | UInt32 | Storlek på volym. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentOutOfRangeException | *segmentSize* är mindre än 100. |

### Anmärkningar

Vissa volymer kan vara mindre än*segmentSize*. I de flesta fall kommer det sista segmentet att vara mindre men sällan kan vanliga segment också vara det.

Namnen på filerna kommer att vara följande:*fileName* .7z.001,*fileName* .7z.002, ...,*fileName*.7z.(n).

### Se även

* class [SplitSevenZipArchiveSaveOptions](../)
* namnutrymme [Aspose.Zip.Saving](../../splitsevenziparchivesaveoptions/)
* hopsättning [Aspose.Zip](../../../)


