---
title: "ZstandardArchive.ZstandardArchive"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "ZstandardArchive constructor. Initialiseert een nieuw exemplaar van de ZstandardArchive-klasse, voorbereid op comprimeren"
type: docs
weight: 10
url: /nl/net/aspose.zip.zstandard/zstandardarchive/zstandardarchive/
---
## ZstandardArchive() {#constructor}

Initialiseert een nieuw exemplaar van de [`ZstandardArchive`](../)-klasse, voorbereid op comprimeren.

```csharp
public ZstandardArchive()
```

## Voorbeelden

Het volgende voorbeeld toont hoe een bestand te comprimeren.

```csharp
using (ZstandardArchive archive = new ZstandardArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.zst");
}
```

### Zie ook

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(Stream, ZstandardLoadOptions) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`ZstandardArchive`](../)-klasse, voorbereid op decomprimeren.

```csharp
public ZstandardArchive(Stream sourceStream, ZstandardLoadOptions options = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | Stream | De bron van het archief. |
| opties | ZstandardLoadOptions | De opties om het archief mee te laden. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Wordt opgegooid als de bronstroom is verwijderd. |
| EndOfStreamException | Wordt opgegooid wanneer het einde van de stroom onverwacht wordt bereikt. |
| IOException | Er treedt een I/O-fout op. |
| InvalidDataException | Wordt gegooid wanneer de gegevens ongeldig of beschadigd zijn. |

## Opmerkingen

Deze constructor decompresseert niet. Zie de [`Open`](../open/) methode voor decompressie.

## Voorbeelden

Open een archief vanuit een stream en extraheer het naar een `MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new ZstandardArchive(File.OpenRead("archive.zst")))
  archive.Open().CopyTo(ms);
```

### Zie ook

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(string, ZstandardLoadOptions) {#constructor_2}

Initialiseert een nieuw exemplaar van de [`ZstandardArchive`](../)-klasse.

```csharp
public ZstandardArchive(string path, ZstandardLoadOptions options = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Het pad naar het archiefbestand. |
| opties | ZstandardLoadOptions | De opties om het archief mee te laden. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *path* is null. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om toegang te krijgen. |
| ArgumentException | Het *path* is leeg, bevat alleen witruimtes, of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot bestand *path* is geweigerd. |
| PathTooLongException | Het opgegeven *path*, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens, en bestandsnamen korter dan 260 tekens. |
| NotSupportedException | Bestand op *path* bevat een dubbele punt (:) in het midden van de tekenreeks. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, bijvoorbeeld omdat het zich op een niet-toegewezen station bevindt. |
| EndOfStreamException | Wordt opgegooid wanneer het einde van de stroom onverwacht wordt bereikt. |
| FileNotFoundException | Het bestand is niet gevonden. |
| IOException | Het bestand is al geopend. |
| InvalidDataException | Wordt gegooid wanneer de gegevens ongeldig of beschadigd zijn. |

## Opmerkingen

Deze constructor decompresseert niet. Zie de [`Open`](../open/) methode voor decompressie.

## Voorbeelden

Open een archief vanuit een bestand via pad en extraheer het naar een `MemoryStream`

```csharp
var ms = new MemoryStream();
using (ZstandardArchive archive = new ZstandardArchive("archive.zst"))
  archive.Open().CopyTo(ms);
```

### Zie ook

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


