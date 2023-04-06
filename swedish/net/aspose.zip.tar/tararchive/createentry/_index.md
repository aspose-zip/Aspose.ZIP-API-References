---
title: TarArchive.CreateEntry
second_title: Aspose.ZIP för .NET API-referens
description: TarArchive metod. Skapa en enskild post i arkivet.
type: docs
weight: 80
url: /sv/net/aspose.zip.tar/tararchive/createentry/
---
## CreateEntry(string, Stream, FileSystemInfo) {#createentry_1}

Skapa en enskild post i arkivet.

```csharp
public TarEntry CreateEntry(string name, Stream source, FileSystemInfo fileInfo = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| source | Stream | Ingångsströmmen för posten. |
| fileInfo | FileSystemInfo | Metadata för fil eller mapp som ska komprimeras. |

### Returvärde

Tar inträdesinstans.

### Undantag

| undantag | skick |
| --- | --- |
| PathTooLongException | *name* är för lång för tjära enligt IEEE 1003.1-1998 standard. |
| ArgumentException | Filnamn, som en del av*name*, överstiger 100 symboler. |

### Anmärkningar

Postens namn anges endast inom*name* parameter. Filnamnet som anges i*fileInfo* parametern påverkar inte postens namn.

*fileInfo* kan hänvisa tillDirectoryInfo om posten är katalog.

### Exempel

```csharp
using (var archive = new TarArchive())
{
   archive.CreateEntry("bytes", new MemoryStream(new byte[] {0x00, 0xFF}));
   archive.Save(tarFile);
}
```

### Se även

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* namnutrymme [Aspose.Zip.Tar](../../tararchive/)
* hopsättning [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Skapa en enskild post i arkivet.

```csharp
public TarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| fileInfo | FileInfo | Metadata för fil eller mapp som ska komprimeras. |
| openImmediately | Boolean | Sant om du öppnar filen omedelbart, annars öppnar du filen när du sparar arkivet. |

### Returvärde

Tar inträdesinstans.

### Undantag

| undantag | skick |
| --- | --- |
| PathTooLongException | *name* är för lång för tjära enligt IEEE 1003.1-1998 standard. |
| ArgumentException | Filnamn, som en del av*name*, överstiger 100 symboler. |

### Anmärkningar

Postens namn anges endast inom*name* parameter. Filnamnet som anges i*fileInfo* parametern påverkar inte postens namn.

*fileInfo* kan hänvisa tillDirectoryInfo om posten är katalog.

Om filen öppnas omedelbart med*openImmediately*parametern blockeras den tills arkivet kasseras.

### Exempel

```csharp
FileInfo fi = new FileInfo("data.bin");
using (var archive = new TarArchive())
{
   archive.CreateEntry("data.bin", fi);
   archive.Save(tarFile);
}
```

### Se även

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* namnutrymme [Aspose.Zip.Tar](../../tararchive/)
* hopsättning [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Skapa en enskild post i arkivet.

```csharp
public TarEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| path | String | Sökväg till fil som ska komprimeras. |
| openImmediately | Boolean | Sant om du öppnar filen omedelbart, annars öppnar du filen när du sparar arkivet. |

### Returvärde

Tar inträdesinstans.

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *path* är inget. |
| SecurityException | Den som ringer har inte den behörighet som krävs för att få åtkomst. |
| ArgumentException | De*path* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. - eller - Filnamn, som en del av*name*, överstiger 100 symboler. |
| UnauthorizedAccessException | Tillgång till fil*path* är nekad. |
| PathTooLongException | Den angivna*path* , filnamn eller båda överskrider den systemdefinierade maximala längden. Till exempel, på Windows-baserade plattformar måste sökvägar vara mindre än 248 tecken och filnamn måste vara mindre än 260 tecken. - eller -*name* är för lång för tjära enligt IEEE 1003.1-1998 standard. |
| NotSupportedException | Arkivera kl*path* innehåller ett kolon (:) i mitten av strängen. |

### Anmärkningar

Postens namn anges endast inom*name* parameter. Filnamnet som anges i*path* parametern påverkar inte postens namn.

Om filen öppnas omedelbart med*openImmediately*parametern blockeras den tills arkivet kasseras.

### Exempel

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save(outputTarFile);
}
```

### Se även

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* namnutrymme [Aspose.Zip.Tar](../../tararchive/)
* hopsättning [Aspose.Zip](../../../)


