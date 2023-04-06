---
title: TarArchive.TarArchive
second_title: Aspose.ZIP voor .NET API-referentie
description: TarArchive constructeur. Initialiseert een nieuw exemplaar van hetTarArchive klasse.
type: docs
weight: 10
url: /nl/net/aspose.zip.tar/tararchive/tararchive/
---
## TarArchive() {#constructor}

Initialiseert een nieuw exemplaar van het[`TarArchive`](../) klasse.

```csharp
public TarArchive()
```

### Voorbeelden

Het volgende voorbeeld laat zien hoe u een bestand kunt comprimeren.

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.tar");
}
```

### Zie ook

* class [TarArchive](../)
* naamruimte [Aspose.Zip.Tar](../../tararchive/)
* montage [Aspose.Zip](../../../)

---

## TarArchive(Stream) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`Archive`](../../../aspose.zip/archive/) klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd.

```csharp
public TarArchive(Stream sourceStream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | Stream | De bron van het archief. Het moet vindbaar zijn. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| InvalidDataException | *sourceStream* is niet zoek. |

### Opmerkingen

Deze constructor pakt geen enkel item uit. Zien[`Open`](../../tarentry/open/)methode voor uitpakken.

### Voorbeelden

Het volgende voorbeeld laat zien hoe u alle vermeldingen naar een directory kunt extraheren.

```csharp
using (var archive = new TarArchive(File.OpenRead("archive.tar")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Zie ook

* class [TarArchive](../)
* naamruimte [Aspose.Zip.Tar](../../tararchive/)
* montage [Aspose.Zip](../../../)

---

## TarArchive(string) {#constructor_2}

Initialiseert een nieuw exemplaar van het[`TarArchive`](../) klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd.

```csharp
public TarArchive(string path)
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

Deze constructor pakt geen enkel item uit. Zien[`Open`](../../tarentry/open/)methode voor uitpakken.

### Voorbeelden

Het volgende voorbeeld laat zien hoe u alle vermeldingen naar een directory kunt extraheren.

```csharp
using (var archive = new TarArchive("archive.tar")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Zie ook

* class [TarArchive](../)
* naamruimte [Aspose.Zip.Tar](../../tararchive/)
* montage [Aspose.Zip](../../../)


