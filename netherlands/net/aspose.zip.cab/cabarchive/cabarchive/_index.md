---
title: CabArchive.CabArchive
second_title: Aspose.ZIP voor .NET API-referentie
description: CabArchive constructeur. Initialiseert een nieuw exemplaar van hetCabArchive klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd.
type: docs
weight: 10
url: /nl/net/aspose.zip.cab/cabarchive/cabarchive/
---
## CabArchive(Stream) {#constructor}

Initialiseert een nieuw exemplaar van het[`CabArchive`](../) klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd.

```csharp
public CabArchive(Stream sourceStream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | Stream | De bron van het archief. Het moet vindbaar zijn. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *sourceStream* is niets. |
| ArgumentException | *sourceStream* is niet zoek. |
| InvalidDataException | *sourceStream* is geen geldig cab-archief. |

### Opmerkingen

Deze constructor pakt geen enkel item uit. Zien[`Open`](../../cabentry/open/)methode voor uitpakken.

### Voorbeelden

Het volgende voorbeeld laat zien hoe u alle vermeldingen naar een directory kunt extraheren.

```csharp
using (var archive = new CabArchive(File.OpenRead("archive.cab")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Zie ook

* class [CabArchive](../)
* naamruimte [Aspose.Zip.Cab](../../cabarchive/)
* montage [Aspose.Zip](../../../)

---

## CabArchive(string) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`CabArchive`](../) klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd.

```csharp
public CabArchive(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Het pad naar het archiefbestand. |

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

Deze constructor pakt geen enkel item uit. Zien[`Open`](../../cabentry/open/)methode voor uitpakken.

### Voorbeelden

Het volgende voorbeeld laat zien hoe u alle vermeldingen naar een directory kunt extraheren.

```csharp
using (var archive = new CabArchive("archive.cab")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Zie ook

* class [CabArchive](../)
* naamruimte [Aspose.Zip.Cab](../../cabarchive/)
* montage [Aspose.Zip](../../../)


