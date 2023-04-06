---
title: TarArchive.Save
second_title: Aspose.ZIP för .NET API-referens
description: TarArchive metod. Sparar arkivet i den tillhandahållna strömmen.
type: docs
weight: 120
url: /sv/net/aspose.zip.tar/tararchive/save/
---
## Save(Stream, TarFormat?) {#save}

Sparar arkivet i den tillhandahållna strömmen.

```csharp
public void Save(Stream output, TarFormat? format = default)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| output | Stream | Destinationsström. |
| format | Nullable`1 | Definierar tjärhuvudformat. Nullvärde kommer att behandlas som USTar när det är möjligt. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentException | *output* är inte skrivbar. - eller -*output* är samma ström som vi extraherar från. - ELLER - Det är omöjligt att spara arkiv i*format* på grund av formatbegränsningar. |

### Anmärkningar

*output*måste vara skrivbar.

### Exempel

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(tarFile);
    }
}       
```

### Se även

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namnutrymme [Aspose.Zip.Tar](../../tararchive/)
* hopsättning [Aspose.Zip](../../../)

---

## Save(string, TarFormat?) {#save_1}

Sparar arkiv till destinationsfil som tillhandahålls.

```csharp
public void Save(string destinationFileName, TarFormat? format = default)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationFileName | String | Sökvägen till arkivet som ska skapas. Om det angivna filnamnet pekar på en befintlig fil kommer den att skrivas över. |
| format | Nullable`1 | Definierar tjärhuvudformat. Nullvärde kommer att behandlas som USTar när det är möjligt. |

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
using (var archive = new TarArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("myarchive.tar");
}       
```

### Se även

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namnutrymme [Aspose.Zip.Tar](../../tararchive/)
* hopsättning [Aspose.Zip](../../../)


