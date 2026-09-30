---
title: "IsoArchive.IsoArchive"
second_title: "Aspose.ZIP för .NET API-referens"
description: "IsoArchive‑konstruktor. Initierar en ny instans av klassen IsoArchive och skapar ett tomt ISO‑arkiv för att lägga till nya filer och kataloger."
type: docs
weight: 10
url: /sv/net/aspose.zip.iso/isoarchive/isoarchive/
---
## IsoArchive() {#constructor}

Initierar en ny instans av klassen [`IsoArchive`](../) och skapar ett tomt ISO‑arkiv för att lägga till nya filer och kataloger.

```csharp
public IsoArchive()
```

## Exempel

Följande exempel visar hur man skapar ett nytt tomt ISO‑arkiv och lägger till filer i det:

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

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(Stream, IsoLoadOptions) {#constructor_1}

Initierar en ny instans av klassen [`IsoArchive`](../) och skapar en postlista som kan extraheras från arkivet.

```csharp
public IsoArchive(Stream sourceStream, IsoLoadOptions loadOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | Ström | Källan till arkivet. Den måste vara sökbar. |
| loadOptions | IsoLoadOptions | Alternativen för att ladda arkivet med. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *sourceStream* är null. |
| ArgumentException | *sourceStream* är inte sökbar. |
| InvalidDataException | *sourceStream* är inte ett giltigt ISO‑arkiv. |
| ObjectDisposedException | Kastas om källströmmen har frigjorts. |
| EndOfStreamException | Kastas när slutet på strömmen nås oväntat. |
| IOException | Ett I/O‑fel inträffar. |
| NotSupportedException | Strömmen stöder inte läsning. |

## Anmärkningar

Denna konstruktor packar inte upp någon post.

## Exempel

Följande exempel visar hur man extraherar alla poster till en katalog.

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Se även

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(string, IsoLoadOptions) {#constructor_2}

Initierar en ny instans av klassen [`IsoArchive`](../) och skapar en postlista som kan extraheras från arkivet.

```csharp
public IsoArchive(string path, IsoLoadOptions loadOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Sökvägen till arkivfilen. |
| loadOptions | IsoLoadOptions | Alternativen för att ladda arkivet med. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *path* är null. |
| SecurityException | Anroparen har inte den erforderliga behörigheten för åtkomst. |
| ArgumentException | *path* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Åtkomst till filen *path* nekas. |
| PathTooLongException | Den angivna *path*, filnamnet eller båda överskrider systemdefinierad maximal längd. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken och filnamn kortare än 260 tecken. |
| NotSupportedException | Filen på *path* innehåller ett kolon (:) i mitten av strängen. |
| FileNotFoundException | Filen hittades inte. |
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig, till exempel om den ligger på en ej mappad enhet. |
| IOException | Filen är redan öppen. |
| EndOfStreamException | Filen är för kort. |
| InvalidDataException | Kastas när data är ogiltig eller korrupt. |

## Anmärkningar

Denna konstruktor packar inte upp någon post.

## Exempel

Följande exempel visar hur man extraherar alla poster till en katalog.

```csharp
using (var archive = new IsoArchive("archive.iso")) 
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Se även

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


