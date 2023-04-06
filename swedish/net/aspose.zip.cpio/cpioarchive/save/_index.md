---
title: CpioArchive.Save
second_title: Aspose.ZIP för .NET API-referens
description: CpioArchive metod. Sparar arkiv till destinationsfil som tillhandahålls.
type: docs
weight: 80
url: /sv/net/aspose.zip.cpio/cpioarchive/save/
---
## Save(string, CpioFormat) {#save_1}

Sparar arkiv till destinationsfil som tillhandahålls.

```csharp
public void Save(string destinationFileName, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationFileName | String | Sökvägen till arkivet som ska skapas. Om det angivna filnamnet pekar på en befintlig fil kommer den att skrivas över. |
| cpioFormat | CpioFormat | Definierar cpio-huvudformat. |

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
using (var archive = new CpioArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.cpio");
}       
```

### Se även

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namnutrymme [Aspose.Zip.Cpio](../../cpioarchive/)
* hopsättning [Aspose.Zip](../../../)

---

## Save(Stream, CpioFormat) {#save}

Sparar arkivet i den tillhandahållna strömmen.

```csharp
public void Save(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| output | Stream | Destinationsström. |
| cpioFormat | CpioFormat | Definierar cpio-huvudformat. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *output* är inget. |
| ArgumentException | *output* är inte skrivbar. - eller -*output* är samma ström som vi extraherar från. - ELLER - Det är omöjligt att spara arkiv i*cpioFormat* på grund av formatbegränsningar. |

### Anmärkningar

*output*måste vara skrivbar.

### Exempel

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(cpioFile);
    }
}       
```

### Se även

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namnutrymme [Aspose.Zip.Cpio](../../cpioarchive/)
* hopsättning [Aspose.Zip](../../../)


