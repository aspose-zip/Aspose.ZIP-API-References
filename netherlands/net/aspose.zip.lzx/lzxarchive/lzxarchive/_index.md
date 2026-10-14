---
title: "LzxArchive.LzxArchive"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "LzxArchive constructor. Initialiseert een nieuw exemplaar van de LzxArchive-klasse en stelt een lijst met items samen die uit het archief kunnen worden geëxtraheerd."
type: docs
weight: 10
url: /nl/net/aspose.zip.lzx/lzxarchive/lzxarchive/
---
## LzxArchive(Stream, LzxLoadOptions) {#constructor}

Initialiseert een nieuw exemplaar van de [`LzxArchive`](../)-klasse en stelt een lijst met items samen die uit het archief kunnen worden geëxtraheerd.

```csharp
public LzxArchive(Stream extractionSource, LzxLoadOptions loadOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| extractionSource | Stream | De bron van het archief. |
| loadOptions | LzxLoadOptions | Opties om een bestaand archief mee te laden. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *extractionSource* is null. |
| ArgumentException | *extractionSource* ondersteunt geen zoeken. |
| InvalidDataException | Verkeerde handtekening voor archief. - of - Het bestand is geen LZX-archief. |
| NotImplementedException | Lzx-archief bevat samengevoegde items. |
| EndOfStreamException | De *extractionSource*-stroom is te kort. |
| ObjectDisposedException | Wordt gegooid als de stroom is gesloten. |
| IOException | Er treedt een I/O-fout op. |

## Opmerkingen

Deze constructor decompresseert geen enkel item. Zie de [`Extract`](../../lzxarchiveentry/extract/)-methode voor decompressie.

### Zie ook

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzxArchive(string, LzxLoadOptions) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`LzxArchive`](../)-klasse en stelt een lijst met items samen die uit het archief kunnen worden geëxtraheerd.

```csharp
public LzxArchive(string path, LzxLoadOptions loadOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Het volledig gekwalificeerde of het relatieve pad naar het archiefbestand. |
| loadOptions | LzxLoadOptions | Opties om een bestaand archief mee te laden. |

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
| NotImplementedException | Lzx-archief bevat samengevoegde items. |
| EndOfStreamException | Het bestand is te kort. |
| ObjectDisposedException | Wordt gegooid als de stroom is gesloten. |

## Opmerkingen

Deze constructor decompresseert geen enkel item. Zie de [`Extract`](../../lzxarchiveentry/extract/)-methode voor decompressie.

## Voorbeelden

Het volgende voorbeeld extraheert een archief en decompresseert vervolgens de eerste entry naar een `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LzxArchive archive = new LzxArchive("sample.lzx"))
{
    archive.Entries[0].Extract(extracted);
}
```

### Zie ook

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)


