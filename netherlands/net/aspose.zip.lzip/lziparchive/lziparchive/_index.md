---
title: LzipArchive.LzipArchive
second_title: Aspose.ZIP voor .NET API-referentie
description: LzipArchive constructeur. Initialiseert een nieuw exemplaar van hetLzipArchive .
type: docs
weight: 10
url: /nl/net/aspose.zip.lzip/lziparchive/lziparchive/
---
## LzipArchive(LzipArchiveSettings) {#constructor}

Initialiseert een nieuw exemplaar van het[`LzipArchive`](../) .

```csharp
public LzipArchive(LzipArchiveSettings settings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| settings | LzipArchiveSettings | Instelling van een bepaald lzip-archief met definitie van woordenboekgrootte. |

### Zie ook

* class [LzipArchiveSettings](../../lziparchivesettings/)
* class [LzipArchive](../)
* naamruimte [Aspose.Zip.Lzip](../../lziparchive/)
* montage [Aspose.Zip](../../../)

---

## LzipArchive(Stream) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`LzipArchive`](../) klasse voorbereid voor decomprimeren.

```csharp
public LzipArchive(Stream sourceStream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | Stream | De bron van het archief. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentException | *sourceStream* is niet zoek. |
| ArgumentNullException | *sourceStream* is niets. |
| InvalidDataException | Kopteksten komen niet overeen met het lzip-archieftype. |

### Opmerkingen

Deze constructor decomprimeert niet. Zien[`Extract`](../extract/) methode voor decomprimeren.

### Zie ook

* class [LzipArchive](../)
* naamruimte [Aspose.Zip.Lzip](../../lziparchive/)
* montage [Aspose.Zip](../../../)

---

## LzipArchive(string) {#constructor_2}

Initialiseert een nieuw exemplaar van het[`LzipArchive`](../) klasse voorbereid voor decomprimeren.

```csharp
public LzipArchive(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Pad naar de bron van het archief. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *path* is niets. |
| SecurityException | De beller heeft niet de vereiste toegangsrechten. |
| ArgumentException | De*path* is leeg, bevat alleen spaties of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot dossier*path* wordt ontkend. |
| PathTooLongException | De opgegeven*path*, bestandsnaam of beide overschrijden de door het systeem gedefinieerde maximale lengte. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. |
| NotSupportedException | Dossier bij*path* bevat een dubbele punt (:) in het midden van de tekenreeks. |
| InvalidDataException | Kopteksten komen niet overeen met het lzip-archieftype. |

### Opmerkingen

Deze constructor decomprimeert niet. Zien[`Extract`](../extract/) methode voor decomprimeren.

### Voorbeelden

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzipArchive(sourceLzipFile))
    {
         archive.Extract(extractedFile);
       }
   }
```

### Zie ook

* class [LzipArchive](../)
* naamruimte [Aspose.Zip.Lzip](../../lziparchive/)
* montage [Aspose.Zip](../../../)


