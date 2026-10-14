---
title: "ZstandardArchive.Save"
second_title: "Aspose.ZIP för .NET API-referens"
description: "ZstandardArchive‑metod. Sparar arkivet till den angivna strömmen"
type: docs
weight: 60
url: /sv/net/aspose.zip.zstandard/zstandardarchive/save/
---
## Save(Stream, ZstandardSaveOptions) {#save_1}

Sparar arkivet till den angivna strömmen.

```csharp
public void Save(Stream outputStream, ZstandardSaveOptions settings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| outputStream | Ström | Målsström. |
| inställningar | ZstandardSaveOptions | Valfria inställningar för arkivkomposition. |

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| ArgumentException | *outputStream* är inte skrivbar. |
| InvalidOperationException | Källan har inte tillhandahållits. |

## Anmärkningar

*outputStream* must be writable.

## Exempel

Skriv komprimerad data till http-svarsström.

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Se även

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, ZstandardSaveOptions) {#save_2}

Sparar arkivet till den angivna destinationsfilen.

```csharp
public void Save(string destinationFileName, ZstandardSaveOptions settings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationFileName | String | Sökvägen för arkivet som ska skapas. Om det angivna filnamnet pekar på en befintlig fil kommer den att skrivas över. |
| inställningar | ZstandardSaveOptions | Valfria inställningar för arkivkomposition. |

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| ArgumentNullException | *destinationFileName* är null. |
| SecurityException | Anroparen har inte den erforderliga behörigheten för åtkomst. |
| ArgumentException | Den *destinationFileName* är tom, innehåller endast blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Åtkomst till filen *destinationFileName* nekas. |
| PathTooLongException | Den angivna *destinationFileName*, filnamnet eller båda överskrider den systemdefinierade maximala längden. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken och filnamn kortare än 260 tecken. |
| NotSupportedException | Filen på *destinationFileName* innehåller ett kolon (:) i mitten av strängen. |
| Undantag | Kastas när ett körningsfel inträffar. |
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig (till exempel om den ligger på en ej mappad enhet). |
| IOException | Ett I/O‑fel inträffade när filen öppnades. |
| InvalidOperationException | Källan har inte tillhandahållits. |

## Exempel

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.zst");
}
```

### Se även

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo, ZstandardSaveOptions) {#save}

Sparar arkivet till den angivna destinationsfilen.

```csharp
public void Save(FileInfo destination, ZstandardSaveOptions settings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | FileInfo | FileInfo, som kommer att öppnas som destinationsström. |
| inställningar | ZstandardSaveOptions | Valfria inställningar för arkivkomposition. |

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| SecurityException | Anroparen har inte den nödvändiga behörigheten för att öppna *destination*. |
| ArgumentException | Filsökvägen är tom eller innehåller endast blanksteg. |
| FileNotFoundException | Filen hittades inte. |
| UnauthorizedAccessException | Sökvägen till filen är skrivskyddad eller är en katalog. |
| ArgumentNullException | *destination* är null. |
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig, till exempel om den ligger på en ej mappad enhet. |
| IOException | Filen är redan öppen. |
| InvalidOperationException | Källan har inte tillhandahållits. |

## Exempel

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.zst"));
}
```

### Se även

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


