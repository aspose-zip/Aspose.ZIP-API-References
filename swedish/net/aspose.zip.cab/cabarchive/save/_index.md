---
title: "CabArchive.Save"
second_title: "Aspose.ZIP för .NET API-referens"
description: "CabArchive-metod. Sparar arkivet till den angivna strömmen."
type: docs
weight: 70
url: /sv/net/aspose.zip.cab/cabarchive/save/
---
## Save(Stream, CabSaveOptions) {#save}

Sparar arkivet till den angivna strömmen.

```csharp
public void Save(Stream outputStream, CabSaveOptions saveOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| outputStream | Ström | Målsström. |
| saveOptions | CabSaveOptions | Alternativ för att spara arkivet. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentException | *outputStream* är inte skrivbar och sökbar. |
| ObjectDisposedException | Arkivet har frigjorts. |
| InvalidOperationException | Arkivet är förberett för extrahering och kan inte sparas. |

## Anmärkningar

*outputStream* must be writable.

## Exempel

```csharp
using (FileStream cabFile = File.Open("archive.cab", FileMode.Create))
{
    using (var archive = new CabArchive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(cabFile);
    }
}
```

### Se även

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, CabSaveOptions) {#save_1}

Sparar arkivet till den angivna destinationsfilen.

```csharp
public void Save(string destinationFileName, CabSaveOptions saveOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationFileName | String | Sökvägen för arkivet som ska skapas. Om det angivna filnamnet pekar på en befintlig fil kommer den att skrivas över. |
| saveOptions | CabSaveOptions | Alternativ för att spara arkivet. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *destinationFileName* är null. |
| SecurityException | Anroparen har inte den erforderliga behörigheten för åtkomst. |
| ArgumentException | Den *destinationFileName* är tom, innehåller endast blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Åtkomst till filen *destinationFileName* nekas. |
| PathTooLongException | Den angivna *destinationFileName*, filnamnet eller båda överskrider den systemdefinierade maximala längden. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken och filnamn kortare än 260 tecken. |
| NotSupportedException | Filen på *destinationFileName* innehåller ett kolon (:) i mitten av strängen. |
| FileNotFoundException | Filen hittades inte. |
| InvalidOperationException | Arkivet är öppnat för extraktion. |
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig, till exempel om den ligger på en ej mappad enhet. |
| IOException | Filen är redan öppen. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Anmärkningar

Det är möjligt att spara ett arkiv till samma sökväg som det laddades från. Detta rekommenderas dock inte eftersom detta tillvägagångssätt använder kopiering till en temporär fil.

## Exempel

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### Se även

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


