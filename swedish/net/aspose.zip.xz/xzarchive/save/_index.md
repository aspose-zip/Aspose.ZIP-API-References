---
title: XzArchive.Save
second_title: Aspose.ZIP för .NET API-referens
description: XzArchive metod. Sparar xzarkiv till den tillhandahållna strömmen.
type: docs
weight: 40
url: /sv/net/aspose.zip.xz/xzarchive/save/
---
## Save(Stream) {#save}

Sparar xz-arkiv till den tillhandahållna strömmen.

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

### Anmärkningar

*output* måste vara sökbar.

### Exempel

```csharp
using (FileStream xzFile = File.Open("archive.xz", FileMode.Create))
{
    using (var archive = new XzArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(xzFile);
     }
}
```

### Se även

* class [XzArchive](../)
* namnutrymme [Aspose.Zip.Xz](../../xzarchive/)
* hopsättning [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Sparar xz-arkiv till destinationsfilen som tillhandahålls.

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
using (var archive = new XzArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.xz");
}
```

### Se även

* class [XzArchive](../)
* namnutrymme [Aspose.Zip.Xz](../../xzarchive/)
* hopsättning [Aspose.Zip](../../../)


