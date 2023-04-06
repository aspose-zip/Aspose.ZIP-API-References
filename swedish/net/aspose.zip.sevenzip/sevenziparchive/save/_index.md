---
title: SevenZipArchive.Save
second_title: Aspose.ZIP för .NET API-referens
description: SevenZipArchive metod. Sparar 7zarkiv till den tillhandahållna strömmen.
type: docs
weight: 80
url: /sv/net/aspose.zip.sevenzip/sevenziparchive/save/
---
## Save(Stream) {#save}

Sparar 7z-arkiv till den tillhandahållna strömmen.

```csharp
public void Save(Stream output)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| output | Stream | Destinationsström. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentException | *output* stöder inte sökning. |
| ArgumentNullException | *output* är inget. |
| InvalidOperationException | Encoder misslyckades med att komprimera data. |

### Anmärkningar

*output* måste vara sökbar.

### Exempel

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
  using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
  {
    using (var archive = new SevenZipArchive())
    {
      archive.CreateEntry("data", source);
      archive.Save(sevenZipFile);
    }
  }
}
```

### Se även

* class [SevenZipArchive](../)
* namnutrymme [Aspose.Zip.SevenZip](../../sevenziparchive/)
* hopsättning [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Sparar arkiv till destinationsfil som tillhandahålls.

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

### Anmärkningar

Det är möjligt att spara ett arkiv på samma sökväg som det laddades från. Detta rekommenderas dock inte eftersom detta tillvägagångssätt använder kopiering till temporär fil.

### Exempel

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
   using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
   {
      archive.CreateEntry("data", source);
      archive.Save("archive.7z");
   }
}
```

### Se även

* class [SevenZipArchive](../)
* namnutrymme [Aspose.Zip.SevenZip](../../sevenziparchive/)
* hopsättning [Aspose.Zip](../../../)


