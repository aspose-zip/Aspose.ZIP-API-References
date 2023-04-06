---
title: ArchiveInstanceInfo.GetArchiveFormatInfo
second_title: Aspose.ZIP för .NET API-referens
description: ArchiveInstanceInfo metod. Får information om arkivformat.
type: docs
weight: 50
url: /sv/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveformatinfo/
---
## GetArchiveFormatInfo(string) {#getarchiveformatinfo_1}

Får information om arkivformat.

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(string fileName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | Filnamnet på arkivfilen. |

### Returvärde

Information om arkivformat eller null om format inte upptäcktes.

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *fileName* är inget. |
| SecurityException | Den som ringer har inte den behörighet som krävs för att få åtkomst. |
| ArgumentException | De*fileName* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Tillgång till fil*fileName* är nekad. |
| PathTooLongException | Den angivna*fileName* överskrider den systemdefinierade maximala längden. Till exempel, på Windows-baserade plattformar måste sökvägar vara mindre än 248 tecken och filnamn måste vara mindre än 260 tecken. |
| NotSupportedException | Arkivera kl*fileName* innehåller ett kolon (:) i mitten av strängen. |
| IOException | Ett I/O-fel uppstod när filen öppnades. |

### Se även

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* namnutrymme [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* hopsättning [Aspose.Zip](../../../)

---

## GetArchiveFormatInfo(Stream) {#getarchiveformatinfo}

Får information om arkivformat.

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | Stream | Strömmen av arkivfilen. |

### Returvärde

Information om arkivformat eller null om format inte upptäcktes.

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *stream* är inget. |
| ArgumentException | *stream* är inte sökbar. |

### Se även

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* namnutrymme [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* hopsättning [Aspose.Zip](../../../)


