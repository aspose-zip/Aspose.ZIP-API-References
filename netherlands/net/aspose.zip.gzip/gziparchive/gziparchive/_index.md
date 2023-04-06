---
title: GzipArchive.GzipArchive
second_title: Aspose.ZIP voor .NET API-referentie
description: GzipArchive constructeur. Initialiseert een nieuw exemplaar van hetGzipArchive klasse voorbereid voor compressie.
type: docs
weight: 10
url: /nl/net/aspose.zip.gzip/gziparchive/gziparchive/
---
## GzipArchive() {#constructor}

Initialiseert een nieuw exemplaar van het[`GzipArchive`](../) klasse voorbereid voor compressie.

```csharp
public GzipArchive()
```

### Voorbeelden

In het volgende voorbeeld ziet u hoe u een bestand kunt comprimeren.

```csharp
using (GzipArchive archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Zie ook

* class [GzipArchive](../)
* naamruimte [Aspose.Zip.Gzip](../../gziparchive/)
* montage [Aspose.Zip](../../../)

---

## GzipArchive(Stream, bool) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`GzipArchive`](../) klasse voorbereid voor decomprimeren.

```csharp
public GzipArchive(Stream sourceStream, bool parseHeader = false)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | Stream | De bron van het archief. |
| parseHeader | Boolean | Of de streamkoptekst moet worden geparseerd om eigenschappen, inclusief naam, te achterhalen. Alleen zinvol voor doorzoekbare streams. |

### Opmerkingen

Deze constructor decomprimeert niet. Zien[`Open`](../open/) methode voor decomprimeren.

### Voorbeelden

Open een archief vanuit een stream en pak het uit naar een`MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz")))
  archive.Open().CopyTo(ms);
```

### Zie ook

* class [GzipArchive](../)
* naamruimte [Aspose.Zip.Gzip](../../gziparchive/)
* montage [Aspose.Zip](../../../)

---

## GzipArchive(string, bool) {#constructor_2}

Initialiseert een nieuw exemplaar van het[`GzipArchive`](../) klasse.

```csharp
public GzipArchive(string path, bool parseHeader = false)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Het pad naar het archiefbestand. |
| parseHeader | Boolean | Of de streamkoptekst moet worden geparseerd om eigenschappen, inclusief naam, te achterhalen. Alleen zinvol voor doorzoekbare streams. |

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

Deze constructor decomprimeert niet. Zien[`Open`](../open/) methode voor decomprimeren.

### Voorbeelden

Open een archief vanuit bestand op pad en pak het uit naar een`MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive("archive.gz"))
  archive.Open().CopyTo(ms);
```

### Zie ook

* class [GzipArchive](../)
* naamruimte [Aspose.Zip.Gzip](../../gziparchive/)
* montage [Aspose.Zip](../../../)


