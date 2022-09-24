---
title: Archive
second_title: Aspose.ZIP för .NET API-referens
description: Initierar en ny instans avArchiveaspose.zip/archiveklass med valfria inställningar för dess poster.
type: docs
weight: 10
url: /sv/net/aspose.zip/archive/archive/
---
## Archive(ArchiveEntrySettings) {#constructor}

Initierar en ny instans av[`Archive`](../../archive)klass med valfria inställningar för dess poster.

```csharp
public Archive(ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| newEntrySettings | ArchiveEntrySettings | Komprimerings- och krypteringsinställningar som används för nyligen tillagda[`ArchiveEntry`](../../archiveentry)items. Om det inte anges, skulle den vanligaste Deflate-komprimeringen utan kryptering användas. |

### Exempel

Följande exempel visar hur man komprimerar en enskild fil med standardinställningar.

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

* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* namnutrymme [Aspose.Zip](../../archive)
* hopsättning [Aspose.Zip](../../../)

---

## Archive(Stream, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_1}

Initierar en ny instans av[`Archive`](../../archive) klass och komponerar poster lista kan extraheras från arkivet.

```csharp
public Archive(Stream sourceStream, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | Stream | Källan till arkivet. |
| loadOptions | ArchiveLoadOptions | Alternativ att ladda befintligt arkiv med. |
| newEntrySettings | ArchiveEntrySettings | Komprimerings- och krypteringsinställningar som används för nyligen tillagda[`ArchiveEntry`](../../archiveentry)items. Om det inte anges, skulle den vanligaste Deflate-komprimeringen utan kryptering användas. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentException | *sourceStream* är inte sökbar. |
| InvalidDataException | Krypteringshuvudet för AES motsäger WinZip-komprimeringsmetoden. |

### Anmärkningar

Denna konstruktor dekomprimerar inte någon post. Ser[`Open`](../../archiveentry/open) metod för dekomprimering.

### Exempel

Följande exempel extraherar ett krypterat arkiv och dekomprimerar sedan första posten till en`MemoryStream`.

```csharp
var fs = File.OpenRead("encrypted.zip");
var extracted = new MemoryStream();
using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Se även

* class [ArchiveLoadOptions](../../archiveloadoptions)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* namnutrymme [Aspose.Zip](../../archive)
* hopsättning [Aspose.Zip](../../../)

---

## Archive(string, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_2}

Initierar en ny instans av[`Archive`](../../archive) klass och komponerar poster lista kan extraheras från arkivet.

```csharp
public Archive(string path, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | String | Den fullt kvalificerade eller den relativa sökvägen till arkivfilen. |
| loadOptions | ArchiveLoadOptions | Alternativ att ladda befintligt arkiv med. |
| newEntrySettings | ArchiveEntrySettings | Komprimerings- och krypteringsinställningar som används för nyligen tillagda[`ArchiveEntry`](../../archiveentry)items. Om det inte anges, skulle den vanligaste Deflate-komprimeringen utan kryptering användas. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *path* är inget. |
| SecurityException | Den som ringer har inte den behörighet som krävs för att få åtkomst |
| ArgumentException | De*path* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Tillgång till fil*path* är nekad. |
| PathTooLongException | Den angivna*path*, filnamn eller båda överskrider den systemdefinierade maximala längden. Till exempel, på Windows-baserade plattformar måste sökvägar vara mindre än 248 tecken och filnamn måste vara mindre än 260 tecken. |
| NotSupportedException | Arkivera kl*path* innehåller ett kolon (:) i mitten av strängen. |

### Anmärkningar

Denna konstruktor dekomprimerar inte någon post. Ser[`Open`](../../archiveentry/open) metod för dekomprimering.

### Exempel

Följande exempel extraherar ett krypterat arkiv och dekomprimerar sedan första posten till en`MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (Archive archive = new Archive("encrypted.zip", new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Se även

* class [ArchiveLoadOptions](../../archiveloadoptions)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* namnutrymme [Aspose.Zip](../../archive)
* hopsättning [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
