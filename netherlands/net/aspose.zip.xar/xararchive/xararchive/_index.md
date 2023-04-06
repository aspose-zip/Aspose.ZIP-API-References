---
title: XarArchive.XarArchive
second_title: Aspose.ZIP voor .NET API-referentie
description: XarArchive constructeur. Initialiseert een nieuw exemplaar van hetXarArchive klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd.
type: docs
weight: 10
url: /nl/net/aspose.zip.xar/xararchive/xararchive/
---
## XarArchive(Stream) {#constructor}

Initialiseert een nieuw exemplaar van het[`XarArchive`](../) klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd.

```csharp
public XarArchive(Stream sourceStream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | Stream | De bron van het archief. Het moet vindbaar zijn. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *sourceStream* is niets. |
| ArgumentException | *sourceStream* is niet zoek. |
| InvalidDataException | *sourceStream* is geen geldig xar-archief. |

### Opmerkingen

Deze constructor pakt geen enkel item uit. Zien[`Open`](../../xarfileentry/open/)methode voor uitpakken.

### Voorbeelden

Het volgende voorbeeld laat zien hoe u alle vermeldingen naar een directory kunt extraheren.

```csharp
using (var archive = new XarArchive(File.OpenRead("archive.xar")))
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Zie ook

* class [XarArchive](../)
* naamruimte [Aspose.Zip.Xar](../../xararchive/)
* montage [Aspose.Zip](../../../)

---

## XarArchive(string) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`XarArchive`](../) klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd.

```csharp
public XarArchive(string path)
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

Deze constructor pakt geen enkel item uit. Zien[`Open`](../../xarfileentry/open/)methode voor uitpakken.

### Voorbeelden

Het volgende voorbeeld laat zien hoe u alle vermeldingen naar een directory kunt extraheren.

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Zie ook

* class [XarArchive](../)
* naamruimte [Aspose.Zip.Xar](../../xararchive/)
* montage [Aspose.Zip](../../../)


