---
title: SnappyArchive.SnappyArchive
second_title: Aspose.ZIP voor .NET API-referentie
description: SnappyArchive constructeur. Initialiseert een nieuw exemplaar van hetSnappyArchive klasse voorbereid voor compressie.
type: docs
weight: 10
url: /nl/net/aspose.zip.snappy/snappyarchive/snappyarchive/
---
## SnappyArchive() {#constructor}

Initialiseert een nieuw exemplaar van het[`SnappyArchive`](../) klasse voorbereid voor compressie.

```csharp
public SnappyArchive()
```

### Voorbeelden

In het volgende voorbeeld ziet u hoe u een bestand kunt comprimeren.

```csharp
using (SnappyArchive archive = new SnappyArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.snapy");
}
```

### Zie ook

* class [SnappyArchive](../)
* naamruimte [Aspose.Zip.Snappy](../../snappyarchive/)
* montage [Aspose.Zip](../../../)

---

## SnappyArchive(Stream) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`SnappyArchive`](../) klasse voorbereid voor decomprimeren.

```csharp
public SnappyArchive(Stream source)
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

* class [SnappyArchive](../)
* naamruimte [Aspose.Zip.Snappy](../../snappyarchive/)
* montage [Aspose.Zip](../../../)

---

## SnappyArchive(string) {#constructor_2}

Initialiseert een nieuw exemplaar van het[`SnappyArchive`](../) klasse voorbereid voor decomprimeren.

```csharp
public SnappyArchive(string path)
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
    using (var archive = new SnappyArchive(sourceSnappyFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### Zie ook

* class [SnappyArchive](../)
* naamruimte [Aspose.Zip.Snappy](../../snappyarchive/)
* montage [Aspose.Zip](../../../)


