---
title: LzmaArchive.LzmaArchive
second_title: Aspose.ZIP voor .NET API-referentie
description: LzmaArchive constructeur. Initialiseert een nieuw exemplaar van hetLzmaArchive klasse en stelt het archief samen in lzmaindeling.
type: docs
weight: 10
url: /nl/net/aspose.zip.lzma/lzmaarchive/lzmaarchive/
---
## LzmaArchive(LzmaArchiveSettings) {#constructor}

Initialiseert een nieuw exemplaar van het[`LzmaArchive`](../) klasse en stelt het archief samen in lzma-indeling.

```csharp
public LzmaArchive(LzmaArchiveSettings settings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| settings | LzmaArchiveSettings | Set van het instellen van een bepaald lzma-archief. |

### Zie ook

* class [LzmaArchiveSettings](../../lzmaarchivesettings/)
* class [LzmaArchive](../)
* naamruimte [Aspose.Zip.LZMA](../../lzmaarchive/)
* montage [Aspose.Zip](../../../)

---

## LzmaArchive(Stream) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`LzmaArchive`](../) klasse voorbereid voor decomprimeren.

```csharp
public LzmaArchive(Stream source)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | Stream | De bron van het archief. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentException | *source* is niet zoek. |
| ArgumentNullException | *source* is niets. |

### Opmerkingen

Deze constructor decomprimeert niet. Zien[`Extract`](../extract/) methode voor decomprimeren.

### Zie ook

* class [LzmaArchive](../)
* naamruimte [Aspose.Zip.LZMA](../../lzmaarchive/)
* montage [Aspose.Zip](../../../)

---

## LzmaArchive(string) {#constructor_2}

Initialiseert een nieuw exemplaar van het[`LzmaArchive`](../) klasse voorbereid voor decomprimeren.

```csharp
public LzmaArchive(string path)
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

### Opmerkingen

Deze constructor decomprimeert niet. Zien[`Extract`](../extract/) methode voor decomprimeren.

### Voorbeelden

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzmaArchive(sourceLzmaFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### Zie ook

* class [LzmaArchive](../)
* naamruimte [Aspose.Zip.LZMA](../../lzmaarchive/)
* montage [Aspose.Zip](../../../)


