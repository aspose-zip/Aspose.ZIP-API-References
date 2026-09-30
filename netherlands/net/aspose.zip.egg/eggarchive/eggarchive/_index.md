---
title: "EggArchive.EggArchive"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "EggArchive constructor. Initialiseert een nieuwe instantie van de EggArchive‑klasse vanuit een stream"
type: docs
weight: 10
url: /nl/net/aspose.zip.egg/eggarchive/eggarchive/
---
## EggArchive(Stream, EggArchiveLoadOptions) {#constructor}

Initialiseert een nieuwe instantie van de [`EggArchive`](../) klasse vanuit een stream.

```csharp
public EggArchive(Stream stream, EggArchiveLoadOptions loadOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | Stream | De EGG-archiefstream. De stream moet lezen en zoeken ondersteunen. |
| loadOptions | EggArchiveLoadOptions | Opties om het archief mee te laden. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *stream* is null. |
| ArgumentException | *stream* is niet leesbaar en zoekbaar. |

### Zie ook

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)

---

## EggArchive(string, EggArchiveLoadOptions) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`EggArchive`](../) klasse vanuit een bestandspad.

```csharp
public EggArchive(string path, EggArchiveLoadOptions loadOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Pad naar het EGG-archiefbestand. |
| loadOptions | EggArchiveLoadOptions | Opties om het archief mee te laden. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *path* is null. |
| FileNotFoundException | Het bestand bestaat niet. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om toegang te krijgen. |
| ArgumentException | Het *path* is leeg, bevat alleen witruimtes, of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot bestand *path* is geweigerd. |
| PathTooLongException | Het opgegeven *path*, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens, en bestandsnamen korter dan 260 tekens. |
| NotSupportedException | Bestand op *path* bevat een dubbele punt (:) in het midden van de tekenreeks. |
| FileNotFoundException | Het bestand is niet gevonden. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, bijvoorbeeld omdat het zich op een niet-toegewezen station bevindt. |
| IOException | Het bestand is al geopend. |

### Zie ook

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)


