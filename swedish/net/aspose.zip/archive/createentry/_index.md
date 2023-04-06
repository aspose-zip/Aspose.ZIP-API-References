---
title: Archive.CreateEntry
second_title: Aspose.ZIP för .NET API-referens
description: Archive metod. Skapa en enskild post i arkivet.
type: docs
weight: 50
url: /sv/net/aspose.zip/archive/createentry/
---
## CreateEntry(string, string, bool, ArchiveEntrySettings) {#createentry_3}

Skapa en enskild post i arkivet.

```csharp
public ArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| path | String | Det fullständiga namnet på den nya filen, eller det relativa filnamnet som ska komprimeras. |
| openImmediately | Boolean | Sant om du öppnar filen omedelbart, annars öppnar du filen när du sparar arkivet. |
| newEntrySettings | ArchiveEntrySettings | Komprimerings- och krypteringsinställningar som används för att lägga till[`ArchiveEntry`](../../archiveentry/) Artikel. |

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
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### Se även

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namnutrymme [Aspose.Zip](../../archive/)
* hopsättning [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings) {#createentry_1}

Skapa en enskild post i arkivet.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| source | Stream | Ingångsströmmen för posten. |
| newEntrySettings | ArchiveEntrySettings | Komprimerings- och krypteringsinställningar som används för att lägga till[`ArchiveEntry`](../../archiveentry/) Artikel. |

### Returvärde

Zip-inträdesinstans.

### Exempel

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.zip");
}
```

### Se även

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namnutrymme [Aspose.Zip](../../archive/)
* hopsättning [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool, ArchiveEntrySettings) {#createentry}

Skapa en enskild post i arkivet.

```csharp
public ArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| fileInfo | FileInfo | Metadata för filen som ska komprimeras. |
| openImmediately | Boolean | Sant om du öppnar filen omedelbart, annars öppnar du filen när du sparar arkivet. |
| newEntrySettings | ArchiveEntrySettings | Komprimerings- och krypteringsinställningar som används för att lägga till[`ArchiveEntry`](../../archiveentry/) Artikel. |

### Returvärde

Zip-inträdesinstans.

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

Komponera arkiv med poster krypterade med olika krypteringsmetoder och lösenord var och en.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
        archive.CreateEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass2", EncryptionMethod.AES128)));
        archive.CreateEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass3", EncryptionMethod.AES256)));
        archive.Save(zipFile);
    }
}
```

### Se även

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namnutrymme [Aspose.Zip](../../archive/)
* hopsättning [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings, FileSystemInfo) {#createentry_2}

Skapa en enskild post i arkivet.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, ArchiveEntrySettings newEntrySettings, 
    FileSystemInfo fileInfo)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| source | Stream | Ingångsströmmen för posten. |
| newEntrySettings | ArchiveEntrySettings | Komprimerings- och krypteringsinställningar som används för att lägga till[`ArchiveEntry`](../../archiveentry/) Artikel. |
| fileInfo | FileSystemInfo | Metadata för fil eller mapp som ska komprimeras. |

### Returvärde

Zip-inträdesinstans.

### Undantag

| undantag | skick |
| --- | --- |
| InvalidOperationException | Både*source* och*fileInfo* är null eller*source*är null och*fileInfo* står för katalog. |

### Anmärkningar

Postens namn anges endast inom*name* parameter. Filnamnet som anges i*fileInfo* parametern påverkar inte postens namn.

*fileInfo* kan hänvisa tillDirectoryInfo om posten är katalog.

### Exempel

Skapa arkiv med krypterad post.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF} ), new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")), new FileInfo("data1.bin")); 
        archive.Save(zipFile);
    }
}
```

### Se även

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namnutrymme [Aspose.Zip](../../archive/)
* hopsättning [Aspose.Zip](../../../)


