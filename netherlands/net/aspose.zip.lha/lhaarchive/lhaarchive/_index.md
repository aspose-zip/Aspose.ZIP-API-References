---
title: "LhaArchive.LhaArchive"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "LhaArchive-constructeur. Initialiseert een nieuwe instantie van de LhaArchive-klasse en stelt een lijst van items samen die uit het archief kunnen worden geëxtraheerd"
type: docs
weight: 10
url: /nl/net/aspose.zip.lha/lhaarchive/lhaarchive/
---
## LhaArchive(Stream, LhaLoadOptions) {#constructor}

Initialiseert een nieuwe instantie van de [`LhaArchive`](../)-klasse en stelt een lijst van items samen die uit het archief kunnen worden geëxtraheerd.

```csharp
public LhaArchive(Stream sourceStream, LhaLoadOptions loadOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | Stream | De bron van het archief. |
| loadOptions | LhaLoadOptions | Opties om een bestaand archief mee te laden. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *sourceStream* is null |
| ArgumentException | *sourceStream* is niet-zoekbaar. |
| InvalidDataException | Ongepaste gegevens gevonden. |
| EndOfStreamException | Wordt gegooid wanneer het einde van de stream wordt bereikt voordat het verwachte aantal bytes is gelezen. |
| ObjectDisposedException | Wordt gegooid wanneer het object is vrijgegeven. |

## Opmerkingen

Deze constructor decompresseert geen enkele entry. Zie de [`Extract`](../../lhaarchiveentry/extract/) methode voor decompressie.

### Zie ook

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LhaArchive(string, LhaLoadOptions) {#constructor_1}

Initialiseert een nieuwe instantie van de [`LhaArchive`](../)-klasse en stelt een lijst van items samen die uit het archief kunnen worden geëxtraheerd.

```csharp
public LhaArchive(string path, LhaLoadOptions loadOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Het volledig gekwalificeerde of het relatieve pad naar het archiefbestand. |
| loadOptions | LhaLoadOptions | Opties om een bestaand archief mee te laden. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *path* is null. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om toegang te krijgen. |
| ArgumentException | Het *path* is leeg, bevat alleen witruimtes, of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot bestand *path* is geweigerd. |
| PathTooLongException | Het opgegeven *path*, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens, en bestandsnamen korter dan 260 tekens. |
| NotSupportedException | Bestand op *path* bevat een dubbele punt (:) in het midden van de tekenreeks. |
| FileNotFoundException | Het bestand is niet gevonden. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, bijvoorbeeld omdat het zich op een niet-toegewezen station bevindt. |
| IOException | Het bestand is al geopend. |
| InvalidDataException | Het bestand is beschadigd. |
| EndOfStreamException | Wordt gegooid wanneer het einde van de stream wordt bereikt voordat het verwachte aantal bytes is gelezen. |
| ObjectDisposedException | Wordt gegooid wanneer het object is vrijgegeven. |

## Opmerkingen

Deze constructor decompresseert geen enkele entry. Zie de [`Extract`](../../lhaarchiveentry/extract/) methode voor decompressie.

## Voorbeelden

Het volgende voorbeeld extraheert een archief en decompresseert vervolgens de eerste entry naar een `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LhaArchive archive = new LhaArchive("sample.lzh"))
{
    archive.Entries[0].Extract(extracted);
}
```

### Zie ook

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)


