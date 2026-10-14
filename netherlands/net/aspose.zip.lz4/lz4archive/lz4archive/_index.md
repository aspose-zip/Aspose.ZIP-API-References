---
title: "Lz4Archive.Lz4Archive"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "Lz4Archive‑constructor. Initialiseert een nieuw exemplaar van de Lz4Archive‑klasse, voorbereid voor decompressie."
type: docs
weight: 10
url: /nl/net/aspose.zip.lz4/lz4archive/lz4archive/
---
## Lz4Archive(Stream, Lz4LoadOptions) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`Lz4Archive`](../)‑klasse, voorbereid voor decompressie.

```csharp
public Lz4Archive(Stream sourceStream, Lz4LoadOptions loadOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | Stream | De bron van het archief. |
| loadOptions | Lz4LoadOptions | De opties om het archief mee te laden. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentException | Kan niet lezen van *sourceStream* |
| ArgumentNullException | *sourceStream* is null. |
| EndOfStreamException | *sourceStream* is te kort. |
| InvalidDataException | De *sourceStream* heeft een onjuiste handtekening. |
| ObjectDisposedException | Wordt opgegooid als de bronstroom is verwijderd. |
| IOException | Er treedt een I/O-fout op. |

## Opmerkingen

Deze constructor decompresseert niet. Zie de [`Open`](../open/) methode voor decompressie.

## Voorbeelden

Open een archief vanuit een stream en extraheer het naar een `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive(File.OpenRead("archive.lz4")))
  archive.Open().CopyTo(ms);
```

### Zie ook

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(string, Lz4LoadOptions) {#constructor_2}

Initialiseert een nieuw exemplaar van de [`Lz4Archive`](../)‑klasse.

```csharp
public Lz4Archive(string path, Lz4LoadOptions loadOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Het pad naar het archiefbestand. |
| loadOptions | Lz4LoadOptions | De opties om het archief mee te laden. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *path* is null. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om toegang te krijgen |
| ArgumentException | Het *path* is leeg, bevat alleen witruimtes, of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot bestand *path* is geweigerd. |
| PathTooLongException | Het opgegeven *path*, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens, en bestandsnamen korter dan 260 tekens. |
| NotSupportedException | Bestand op *path* bevat een dubbele punt (:) in het midden van de tekenreeks. |
| EndOfStreamException | Het bestand is te kort. |
| InvalidDataException | Gegevens in het bestand hebben een onjuiste handtekening. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, bijvoorbeeld omdat het zich op een niet-toegewezen station bevindt. |
| FileNotFoundException | Het bestand is niet gevonden. |
| IOException | Het bestand is al geopend. |

## Opmerkingen

Deze constructor decompresseert niet. Zie de [`Open`](../open/) methode voor decompressie.

## Voorbeelden

Open een archief vanuit een bestand via pad en extraheer het naar een `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive("archive.lz4"))
  archive.Open().CopyTo(ms);
```

### Zie ook

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(Lz4ArchiveSetting) {#constructor}

Initialiseert een nieuw exemplaar van de [`Lz4Archive`](../)‑klasse, voorbereid voor compressie.

```csharp
public Lz4Archive(Lz4ArchiveSetting settings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| instellingen | Lz4ArchiveSetting | De instelling van het samengestelde archief. |

### Zie ook

* class [Lz4ArchiveSetting](../../lz4archivesetting/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


