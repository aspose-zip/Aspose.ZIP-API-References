---
title: SevenZipArchive.SevenZipArchive
second_title: Aspose.ZIP voor .NET API-referentie
description: SevenZipArchive constructeur. Initialiseert een nieuw exemplaar van hetSevenZipArchive klasse met optionele instellingen voor zijn ingangen.
type: docs
weight: 10
url: /nl/net/aspose.zip.sevenzip/sevenziparchive/sevenziparchive/
---
## SevenZipArchive(SevenZipEntrySettings) {#constructor}

Initialiseert een nieuw exemplaar van het[`SevenZipArchive`](../) klasse met optionele instellingen voor zijn ingangen.

```csharp
public SevenZipArchive(SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| newEntrySettings | SevenZipEntrySettings | Compressie- en coderingsinstellingen gebruikt voor nieuw toegevoegde[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) items. Indien niet gespecificeerd, zou LZMA-compressie zonder codering worden gebruikt. |

### Voorbeelden

Het volgende voorbeeld laat zien hoe een enkel bestand met standaardinstellingen kan worden gecomprimeerd: LZMA-compressie zonder codering.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### Zie ook

* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* naamruimte [Aspose.Zip.SevenZip](../../sevenziparchive/)
* montage [Aspose.Zip](../../../)

---

## SevenZipArchive(Stream) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`SevenZipArchive`](../) klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd.

```csharp
public SevenZipArchive(Stream sourceStream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | Stream | De bron van het archief. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentException | *sourceStream* is niet zoek. |
| ArgumentNullException | *sourceStream* is niets. |
| NotImplementedException | Archief bevat meer dan één coder. Nu wordt alleen LZMA-compressie ondersteund. |

### Opmerkingen

Deze constructor decomprimeert geen enkel item. Zien[`ExtractToDirectory`](../extracttodirectory/) methode voor decomprimeren.

### Voorbeelden

```csharp
using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z")))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### Zie ook

* class [SevenZipArchive](../)
* naamruimte [Aspose.Zip.SevenZip](../../sevenziparchive/)
* montage [Aspose.Zip](../../../)

---

## SevenZipArchive(string) {#constructor_2}

Initialiseert een nieuw exemplaar van het[`SevenZipArchive`](../) klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd.

```csharp
public SevenZipArchive(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Het volledig gekwalificeerde of relatieve pad naar het archiefbestand. |

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

Deze constructor decomprimeert geen enkel item. Zien[`ExtractToDirectory`](../extracttodirectory/) methode voor decomprimeren.

### Voorbeelden

```csharp
using (SevenZipArchive archive = new SevenZipArchive("archive.7z"))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### Zie ook

* class [SevenZipArchive](../)
* naamruimte [Aspose.Zip.SevenZip](../../sevenziparchive/)
* montage [Aspose.Zip](../../../)


