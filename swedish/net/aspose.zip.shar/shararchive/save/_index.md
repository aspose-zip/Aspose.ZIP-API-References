---
title: SharArchive.Save
second_title: Aspose.ZIP för .NET API-referens
description: SharArchive metod. Sparar arkiv till destinationsfil som tillhandahålls.
type: docs
weight: 70
url: /sv/net/aspose.zip.shar/shararchive/save/
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
| ArgumentException | *destinationFileName* är en sträng av noll längd, innehåller endast blanksteg eller innehåller ett eller flera ogiltiga tecken enligt definitionen av System.IO.Path.InvalidPathChars. |
| ArgumentNullException | *destinationFileName* är inget. |
| PathTooLongException | Den angivna*destinationFileName*, filnamn eller båda överskrider den systemdefinierade maximala längden. Till exempel, på Windows-baserade plattformar måste sökvägar vara mindre än 248 tecken och filnamn måste vara mindre än 260 tecken. |
| DirectoryNotFoundException | Den angivna*destinationFileName* är ogiltigt, (det är till exempel på en omappad enhet). |
| IOException | Ett I/O-fel uppstod när filen öppnades. |
| UnauthorizedAccessException | *destinationFileName* angav en fil som är skrivskyddad och åtkomsten är inte Läs.-eller-sökväg specificerade en katalog.-eller- Uppringaren har inte den behörighet som krävs. |
| NotSupportedException | *destinationFileName* är i ett ogiltigt format. |

### Anmärkningar

Det är möjligt att spara ett arkiv på samma sökväg som det laddades från. Detta rekommenderas dock inte eftersom detta tillvägagångssätt använder kopiering till temporär fil.

### Exempel

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.shar");
}       
```

### Se även

* class [SharArchive](../)
* namnutrymme [Aspose.Zip.Shar](../../shararchive/)
* hopsättning [Aspose.Zip](../../../)

---

## Save(Stream) {#save}

Sparar arkivet i den tillhandahållna strömmen.

```csharp
public void Save(Stream output)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| output | Stream | Destinationsström. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *output* är inget. |
| ArgumentException | *output* är inte skrivbar. - eller -*output* är samma ström som vi extraherar från. |

### Anmärkningar

*output*måste vara skrivbar.

### Exempel

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(sharFile);
    }
}       
```

### Se även

* class [SharArchive](../)
* namnutrymme [Aspose.Zip.Shar](../../shararchive/)
* hopsättning [Aspose.Zip](../../../)


