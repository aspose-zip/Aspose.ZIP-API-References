---
title: Archive.Archive
second_title: Aspose.ZIP voor .NET API-referentie
description: Archive constructeur. Initialiseert een nieuw exemplaar van hetArchive klasse met optionele instellingen voor zijn ingangen.
type: docs
weight: 10
url: /nl/net/aspose.zip/archive/archive/
---
## Archive(ArchiveEntrySettings) {#constructor}

Initialiseert een nieuw exemplaar van het[`Archive`](../) klasse met optionele instellingen voor zijn ingangen.

```csharp
public Archive(ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| newEntrySettings | ArchiveEntrySettings | Compressie- en coderingsinstellingen gebruikt voor nieuw toegevoegde[`ArchiveEntry`](../../archiveentry/) items. Indien niet gespecificeerd, zou de meest gebruikelijke Deflate-compressie zonder codering worden gebruikt. |

### Voorbeelden

Het volgende voorbeeld laat zien hoe een enkel bestand met standaardinstellingen kan worden gecomprimeerd.

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

### Zie ook

* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* naamruimte [Aspose.Zip](../../archive/)
* montage [Aspose.Zip](../../../)

---

## Archive(Stream, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`Archive`](../) klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd.

```csharp
public Archive(Stream sourceStream, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | Stream | De bron van het archief. |
| loadOptions | ArchiveLoadOptions | Opties om bestaand archief mee te laden. |
| newEntrySettings | ArchiveEntrySettings | Compressie- en coderingsinstellingen gebruikt voor nieuw toegevoegde[`ArchiveEntry`](../../archiveentry/) items. Indien niet gespecificeerd, zou de meest gebruikelijke Deflate-compressie zonder codering worden gebruikt. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentException | *sourceStream* is niet zoek. |
| InvalidDataException | Versleutelingsheader voor AES is in tegenspraak met de WinZip-compressiemethode. |

### Opmerkingen

Deze constructor decomprimeert geen enkel item. Zien[`Open`](../../archiveentry/open/) methode voor decomprimeren.

### Voorbeelden

Het volgende voorbeeld extraheert een versleuteld archief en decomprimeert vervolgens het eerste item in een`MemoryStream`.

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

### Zie ook

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* naamruimte [Aspose.Zip](../../archive/)
* montage [Aspose.Zip](../../../)

---

## Archive(string, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_2}

Initialiseert een nieuw exemplaar van het[`Archive`](../) klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd.

```csharp
public Archive(string path, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Het volledig gekwalificeerde of relatieve pad naar het archiefbestand. |
| loadOptions | ArchiveLoadOptions | Opties om bestaand archief mee te laden. |
| newEntrySettings | ArchiveEntrySettings | Compressie- en coderingsinstellingen gebruikt voor nieuw toegevoegde[`ArchiveEntry`](../../archiveentry/) items. Indien niet gespecificeerd, zou de meest gebruikelijke Deflate-compressie zonder codering worden gebruikt. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *path* is niets. |
| SecurityException | De beller heeft niet de vereiste toegangsrechten. |
| ArgumentException | De*path* is leeg, bevat alleen spaties of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot dossier*path* wordt ontkend. |
| PathTooLongException | De opgegeven*path*, bestandsnaam of beide overschrijden de door het systeem gedefinieerde maximale lengte. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. |
| NotSupportedException | Dossier bij*path* bevat een dubbele punt (:) in het midden van de tekenreeks. |

### Opmerkingen

Deze constructor decomprimeert geen enkel item. Zien[`Open`](../../archiveentry/open/) methode voor decomprimeren.

### Voorbeelden

Het volgende voorbeeld extraheert een versleuteld archief en decomprimeert vervolgens het eerste item in een`MemoryStream`.

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

### Zie ook

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* naamruimte [Aspose.Zip](../../archive/)
* montage [Aspose.Zip](../../../)


