---
title: SevenZipArchive.CreateEntry
second_title: Aspose.ZIP för .NET API-referens
description: SevenZipArchive metod. Skapa en enskild post i arkivet.
type: docs
weight: 50
url: /sv/net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## CreateEntry(string, FileInfo, bool, SevenZipEntrySettings) {#createentry}

Skapa en enskild post i arkivet.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| fileInfo | FileInfo | Metadata för filen som ska komprimeras. |
| openImmediately | Boolean | Sant om du öppnar filen omedelbart, annars öppnar du filen när du sparar arkivet. |
| newEntrySettings | SevenZipEntrySettings | Komprimerings- och krypteringsinställningar som används för att lägga till[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) Artikel. |

### Returvärde

Seven Zip entry instans.

### Undantag

| undantag | skick |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* är skrivskyddad eller är en katalog. |
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig, till exempel på en omappad enhet. |
| IOException | Filen är redan öppen. |

### Anmärkningar

Postens namn anges endast inom*name* parameter. Filnamnet som anges i*fileInfo* parametern påverkar inte postens namn.

Om filen öppnas omedelbart med*openImmediately* parametern blockeras den tills arkivet sparas.

### Exempel

Komponera arkiv med poster krypterade med olika lösenord var och en.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
        archive.CreateEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
        archive.CreateEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
        archive.Save(sevenZipFile);
    }
}
```

### Se även

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namnutrymme [Aspose.Zip.SevenZip](../../sevenziparchive/)
* hopsättning [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings, FileSystemInfo) {#createentry_2}

Skapa en enskild post i arkivet.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| source | Stream | Ingångsströmmen för posten. |
| newEntrySettings | SevenZipEntrySettings | Komprimerings- och krypteringsinställningar som används för att lägga till[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) Artikel. |
| fileInfo | FileSystemInfo | Metadata för fil eller mapp som ska komprimeras. |

### Returvärde

SevenZip-inträdesinstans.

### Undantag

| undantag | skick |
| --- | --- |
| InvalidOperationException | Både*source* och*fileInfo* är null eller*source*är null och*fileInfo* står för katalog. |

### Anmärkningar

Postens namn anges endast inom*name* parameter. Filnamnet som anges i*fileInfo* parametern påverkar inte postens namn.

*fileInfo* kan hänvisa tillDirectoryInfo om posten är katalog.

### Exempel

Komponera arkiv med LZMA2 komprimerad krypterad post.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF}), new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1")), new FileInfo("data1.bin")); 
        archive.Save(sevenZipFile);
    }
}
```

### Se även

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namnutrymme [Aspose.Zip.SevenZip](../../sevenziparchive/)
* hopsättning [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings) {#createentry_1}

Skapa en enskild post i arkivet.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| source | Stream | Ingångsströmmen för posten. |
| newEntrySettings | SevenZipEntrySettings | Komprimerings- och krypteringsinställningar som används för att lägga till[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) Artikel. |

### Returvärde

Zip-inträdesinstans.

### Exempel

Komponera 7z-arkiv med LZMA2-komprimering och kryptering av alla poster.

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.7z");
}
```

### Se även

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namnutrymme [Aspose.Zip.SevenZip](../../sevenziparchive/)
* hopsättning [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, SevenZipEntrySettings) {#createentry_3}

Skapa en enskild post i arkivet.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| path | String | Det fullständiga namnet på den nya filen, eller det relativa filnamnet som ska komprimeras. |
| openImmediately | Boolean | Sant om du öppnar filen omedelbart, annars öppnar du filen när du sparar arkivet. |
| newEntrySettings | SevenZipEntrySettings | Komprimerings- och krypteringsinställningar som används för att lägga till[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) Artikel. |

### Returvärde

Zip-inträdesinstans.

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *path* är inget. |
| SecurityException | Den som ringer har inte den behörighet som krävs för att få åtkomst. |
| ArgumentException | De*path* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Tillgång till fil*path* är nekad. |
| PathTooLongException | Den angivna*path*, filnamn eller båda överskrider den systemdefinierade maximala längden. Till exempel, på Windows-baserade plattformar måste sökvägar vara mindre än 248 tecken och filnamn måste vara mindre än 260 tecken. |
| NotSupportedException | Arkivera kl*path* innehåller ett kolon (:) i mitten av strängen. |

### Anmärkningar

Postens namn anges endast inom*name* parameter. Filnamnet som anges i*path* parametern påverkar inte postens namn.

Om filen öppnas omedelbart med*openImmediately* parametern blockeras den tills arkivet sparas.

### Exempel

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings())))
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### Se även

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namnutrymme [Aspose.Zip.SevenZip](../../sevenziparchive/)
* hopsättning [Aspose.Zip](../../../)


