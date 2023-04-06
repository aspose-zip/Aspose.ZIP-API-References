---
title: CpioArchive.CpioArchive
second_title: Aspose.ZIP voor .NET API-referentie
description: CpioArchive constructeur. Initialiseert een nieuw exemplaar van hetCpioArchive klasse.
type: docs
weight: 10
url: /nl/net/aspose.zip.cpio/cpioarchive/cpioarchive/
---
## CpioArchive() {#constructor}

Initialiseert een nieuw exemplaar van het[`CpioArchive`](../) klasse.

```csharp
public CpioArchive()
```

### Voorbeelden

Het volgende voorbeeld laat zien hoe u een bestand kunt comprimeren.

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### Zie ook

* class [CpioArchive](../)
* naamruimte [Aspose.Zip.Cpio](../../cpioarchive/)
* montage [Aspose.Zip](../../../)

---

## CpioArchive(Stream) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`CpioArchive`](../) klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd.

```csharp
public CpioArchive(Stream sourceStream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | Stream | De bron van het archief. Het moet vindbaar zijn. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *sourceStream* is niets. |
| ArgumentException | *sourceStream* is niet zoek. |
| InvalidDataException | *sourceStream* is geen geldig cpio-archief. |

### Opmerkingen

Deze constructor pakt geen enkel item uit. Zien[`Open`](../../cpioentry/open/)methode voor uitpakken.

### Voorbeelden

Het volgende voorbeeld laat zien hoe u alle vermeldingen naar een directory kunt extraheren.

```csharp
using (var archive = new CpioArchive(File.OpenRead("archive.cpio")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Zie ook

* class [CpioArchive](../)
* naamruimte [Aspose.Zip.Cpio](../../cpioarchive/)
* montage [Aspose.Zip](../../../)

---

## CpioArchive(string) {#constructor_2}

Initialiseert een nieuw exemplaar van het[`CpioArchive`](../) klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd.

```csharp
public CpioArchive(string path)
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

Deze constructor pakt geen enkel item uit. Zien[`Open`](../../cpioentry/open/)methode voor uitpakken.

### Voorbeelden

Het volgende voorbeeld laat zien hoe u alle vermeldingen naar een directory kunt extraheren.

```csharp
using (var archive = new CpioArchive("archive.cpio")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Zie ook

* class [CpioArchive](../)
* naamruimte [Aspose.Zip.Cpio](../../cpioarchive/)
* montage [Aspose.Zip](../../../)


