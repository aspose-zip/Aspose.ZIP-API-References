---
title: LzipArchive.Save
second_title: Aspose.ZIP för .NET API-referens
description: LzipArchive metod. Sparar lziparkivet i den tillhandahållna strömmen.
type: docs
weight: 50
url: /sv/net/aspose.zip.lzip/lziparchive/save/
---
## Save(Stream) {#save_1}

Sparar lzip-arkivet i den tillhandahållna strömmen.

```csharp
public void Save(Stream outputStream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| outputStream | Stream | Destinationsström. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentException | *outputStream* stöder inte sökning. |
| ArgumentNullException | *outputStream* är inget. |

### Anmärkningar

*outputStream* måste vara sökbar.

### Exempel

```csharp
using (FileStream lzFile = File.Open("archive.lz", FileMode.Create))
{
    using (var archive = new LzipArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(lzFile);
     }
}
```

### Se även

* class [LzipArchive](../)
* namnutrymme [Aspose.Zip.Lzip](../../lziparchive/)
* hopsättning [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

Sparar lzip-arkivet till destinationsfilen som tillhandahålls.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationFileName | String | Sökvägen till arkivet som ska skapas. Om det angivna filnamnet pekar på en befintlig fil kommer den att skrivas över. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *destinationFileName* är inget. |
| SecurityException | Den som ringer har inte den behörighet som krävs för att få åtkomst. |
| ArgumentException | De*destinationFileName* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Tillgång till fil*destinationFileName* är nekad. |
| PathTooLongException | Den angivna*destinationFileName*, filnamn eller båda överskrider den systemdefinierade maximala längden. Till exempel, på Windows-baserade plattformar måste sökvägar vara mindre än 248 tecken och filnamn måste vara mindre än 260 tecken. |
| NotSupportedException | Arkivera kl*destinationFileName* innehåller ett kolon (:) i mitten av strängen. |

### Exempel

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.lz");
}
```

### Se även

* class [LzipArchive](../)
* namnutrymme [Aspose.Zip.Lzip](../../lziparchive/)
* hopsättning [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Sparar lzip-arkivet till destinationsfilen som tillhandahålls.

```csharp
public void Save(FileInfo destination)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destination | FileInfo | FileInfo som kommer att öppnas som målström. |

### Undantag

| undantag | skick |
| --- | --- |
| SecurityException | Den som ringer har inte den behörighet som krävs för att öppna*destination*. |
| ArgumentException | Filsökvägen är tom eller innehåller bara blanksteg. |
| FileNotFoundException | Filen hittades inte. |
| UnauthorizedAccessException | Sökvägen till filen är skrivskyddad eller är en katalog. |
| ArgumentNullException | *destination* är inget. |
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig, till exempel på en omappad enhet. |
| IOException | Filen är redan öppen. |

### Exempel

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz"));
}
```

### Se även

* class [LzipArchive](../)
* namnutrymme [Aspose.Zip.Lzip](../../lziparchive/)
* hopsättning [Aspose.Zip](../../../)


