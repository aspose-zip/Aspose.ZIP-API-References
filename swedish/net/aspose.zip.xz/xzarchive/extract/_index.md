---
title: XzArchive.Extract
second_title: Aspose.ZIP för .NET API-referens
description: XzArchive metod. Extraherar xzarkiv till en ström.
type: docs
weight: 30
url: /sv/net/aspose.zip.xz/xzarchive/extract/
---
## Extract(Stream) {#extract_2}

Extraherar xz-arkiv till en ström.

```csharp
public void Extract(Stream destination)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destination | Stream | Stream för lagring av dekomprimerad data. |

### Undantag

| undantag | skick |
| --- | --- |
| InvalidOperationException | Arkivhuvuden och tjänstinformation lästes inte. |

### Exempel

```csharp
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new XzArchive(xzFile))
        {
            archive.Extract(extractedFile);
        }
    }
}
```

### Se även

* class [XzArchive](../)
* namnutrymme [Aspose.Zip.Xz](../../xzarchive/)
* hopsättning [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Extraherar xz-arkiv till en fil.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo för lagring av dekomprimerad data. |

### Undantag

| undantag | skick |
| --- | --- |
| InvalidOperationException | Arkivhuvuden och tjänstinformation lästes inte. |
| SecurityException | Den som ringer har inte den behörighet som krävs för att öppna*fileInfo*. |
| ArgumentException | Filsökvägen är tom eller innehåller bara blanksteg. |
| FileNotFoundException | Filen hittades inte. |
| UnauthorizedAccessException | Sökvägen till filen är skrivskyddad eller är en katalog. |
| ArgumentNullException | *fileInfo* är inget. |
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig, till exempel på en omappad enhet. |
| IOException | Filen är redan öppen. |

### Exempel

```csharp
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new XzArchive(xzFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### Se även

* class [XzArchive](../)
* namnutrymme [Aspose.Zip.Xz](../../xzarchive/)
* hopsättning [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Extraherar xz-arkiv till en fil med sökväg.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | String | Sökväg till fil som lagrar dekomprimerad data. |

### Undantag

| undantag | skick |
| --- | --- |
| InvalidOperationException | Arkivhuvuden och tjänstinformation lästes inte. |
| ArgumentNullException | *path* är inget. |
| SecurityException | Den som ringer har inte den behörighet som krävs för att få åtkomst. |
| ArgumentException | De*path* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Tillgång till fil*path* är nekad. |
| PathTooLongException | Den angivna*path*, filnamn eller båda överskrider den systemdefinierade maximala längden. Till exempel, på Windows-baserade plattformar måste sökvägar vara mindre än 248 tecken och filnamn måste vara mindre än 260 tecken. |
| NotSupportedException | Arkivera kl*path* innehåller ett kolon (:) i mitten av strängen. |

### Exempel

```csharp
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new XzArchive(xzFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Se även

* class [XzArchive](../)
* namnutrymme [Aspose.Zip.Xz](../../xzarchive/)
* hopsättning [Aspose.Zip](../../../)


