---
title: "GetFormatInfo"
second_title: "Aspose.ZIP för .NET API-referens"
description: 
type: docs
weight: 20
url: /sv/net/aspose.zip.archiveinfo/archiveformatdetector/getformatinfo/
---
## ArchiveFormatDetector.GetFormatInfo method (1 of 2)

Hämtar formatinformation.

```csharp
public ArchiveFormatInfo GetFormatInfo(string fileName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | Filnamnet på arkivfilen. |

### Returvärde

Information om arkivformatet eller null om formatet inte upptäcktes.

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *fileName* är null. |
| SecurityException | Anroparen har inte den erforderliga behörigheten för åtkomst. |
| ArgumentException | Den *fileName* är tom, innehåller endast blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Åtkomst till filen *fileName* nekas. |
| PathTooLongException | Den angivna *fileName* överskrider systemdefinierad maximal längd. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken och filnamn kortare än 260 tecken. |
| NotSupportedException | Filen på *fileName* innehåller ett kolon (:) i mitten av strängen. |
| IOException | Ett I/O‑fel inträffade när filen öppnades. |

### Se även

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

---

## ArchiveFormatDetector.GetFormatInfo method (2 of 2)

Hämtar formatinformation.

```csharp
public ArchiveFormatInfo GetFormatInfo(Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | Strömmen för arkivfilen. |

### Returvärde

Information om arkivformatet eller null om formatet inte upptäcktes.

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *stream* är null. |
| ArgumentException | *stream* är inte sökbar. |

### Se även

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

<!-- FÅ INTE REDIGERA: genererad av xmldocmd för Aspose.Zip.dll -->
