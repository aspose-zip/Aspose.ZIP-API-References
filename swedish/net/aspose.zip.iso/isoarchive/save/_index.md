---
title: "IsoArchive.Save"
second_title: "Aspose.ZIP för .NET API-referens"
description: "IsoArchive-metod. Sparar ISO-avbilden till den angivna sökvägen."
type: docs
weight: 70
url: /sv/net/aspose.zip.iso/isoarchive/save/
---
## Save(string, IsoSaveOptions) {#save_1}

Sparar ISO-avbilden till den angivna sökvägen.

```csharp
public void Save(string path, IsoSaveOptions saveOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Sökvägen där ISO-avbilden kommer att sparas. |
| saveOptions | IsoSaveOptions | Alternativ för att spara ISO-arkivet med. |

### Undantag

| undantag | villkor |
| --- | --- |
| InvalidOperationException | Kastas när arkivet inte är i redigeringsläge. |
| ArgumentNullException | Kastas när *path* är null. |
| DirectoryNotFoundException | Kastas när den angivna sökvägen är ogiltig, till exempel om den ligger på en ej mappad enhet. |
| IOException | Kastas när filen redan är öppen. |
| UnauthorizedAccessException | Kastas när åtkomst till filen *path* nekas. |
| PathTooLongException | Kastas när den angivna *path* överskrider systemdefinierad maximal längd. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Exempel

Följande exempel visar hur man sparar ett ISO-arkiv till en fil:

```csharp
// Skapa ett nytt tomt ISO‑arkiv
using(IsoArchive isoArchive = new IsoArchive())
{
    // Lägg till filer i ISO‑arkivet
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // Spara ISO‑arkivet till en fil
    isoArchive.Save("new_archive.iso");
}
```

### Se även

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, IsoSaveOptions) {#save}

Sparar ISO-avbilden till den angivna strömmen.

```csharp
public void Save(Stream stream, IsoSaveOptions saveOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | Strömmen där ISO-avbilden kommer att sparas. |
| saveOptions | IsoSaveOptions | Alternativ för att spara ISO-arkivet med. |

### Undantag

| undantag | villkor |
| --- | --- |
| InvalidOperationException | Kastas när arkivet inte är i redigeringsläge. |
| ArgumentNullException | Kastas när *stream* är null. |
| ArgumentException | Kastas när *stream* inte är skrivbar. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| IOException | Ett I/O‑fel inträffar. |

## Exempel

Följande exempel visar hur man sparar ett ISO-arkiv till en minnesström:

```csharp

 // Skapa ett nytt tomt ISO‑arkiv
 using(IsoArchive isoArchive = new IsoArchive())
 {
     // Lägg till filer i ISO‑arkivet
     isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

     // Spara ISO-arkivet till en minnesström
     isoArchive.Save(memoryStream);
 }
```

### Se även

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


