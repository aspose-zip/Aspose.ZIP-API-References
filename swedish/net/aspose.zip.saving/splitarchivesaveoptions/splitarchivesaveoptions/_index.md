---
title: SplitArchiveSaveOptions.SplitArchiveSaveOptions
second_title: Aspose.ZIP för .NET API-referens
description: SplitArchiveSaveOptions byggare. Instantierar inställningar för att spara ett ziparkiv med flera volymer.
type: docs
weight: 10
url: /sv/net/aspose.zip.saving/splitarchivesaveoptions/splitarchivesaveoptions/
---
## SplitArchiveSaveOptions constructor

Instantierar inställningar för att spara ett zip-arkiv med flera volymer.

```csharp
public SplitArchiveSaveOptions(string fileName, uint segmentSize)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | Namn på volymer. Kan vara med eller utan .zip-tillägg. |
| segmentSize | UInt32 | Storlek på volym. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentOutOfRangeException | Segmentstorleken är mindre än 65536 byte. |

### Anmärkningar

Vissa volymer kan vara mindre än*segmentSize*. I de flesta fall kommer det sista segmentet att vara mindre men sällan kan vanliga segment också vara det.

Namnen på filerna kommer att vara följande:*fileName* .z01,*fileName* .z02, ...,*fileName* .z(n-1),*fileName*.blixtlås.

### Se även

* class [SplitArchiveSaveOptions](../)
* namnutrymme [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* hopsättning [Aspose.Zip](../../../)


