---
title: "UueArchive.UueArchive"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "UueArchive-constructor. Initialiseert een nieuw exemplaar van de UueArchive-klasse, voorbereid op codering"
type: docs
weight: 10
url: /nl/net/aspose.zip.uue/uuearchive/uuearchive/
---
## UueArchive() {#constructor}

Initialiseert een nieuw exemplaar van de [`UueArchive`](../) klasse, voorbereid op codering.

```csharp
public UueArchive()
```

## Voorbeelden

Het volgende voorbeeld toont hoe een bestand uuencode.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.uue");
}
```

### Zie ook

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(Stream) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`UueArchive`](../) klasse, voorbereid op decodering.

```csharp
public UueArchive(Stream sourceStream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | Stream | De bron van het archief. |

## Opmerkingen

Deze constructor decodeert niet. Zie de [`Open`](../open/) methode voor decompressie.

## Voorbeelden

Open een archief vanuit een stream en extraheer het naar een `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive(File.OpenRead("archive.001")))
  archive.Open().CopyTo(ms);
```

### Zie ook

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(string) {#constructor_2}

Initialiseert een nieuw exemplaar van de [`UueArchive`](../) klasse.

```csharp
public UueArchive(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Het pad naar het archiefbestand. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *path* is null. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om toegang te krijgen. |
| ArgumentException | Het *path* is leeg, bevat alleen witruimtes, of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot bestand *path* is geweigerd. |
| PathTooLongException | Het opgegeven *path*, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens, en bestandsnamen korter dan 260 tekens. |
| NotSupportedException | Bestand op *path* bevat een dubbele punt (:) in het midden van de tekenreeks. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, bijvoorbeeld omdat het zich op een niet-toegewezen station bevindt. |
| FileNotFoundException | Het bestand is niet gevonden. |
| IOException | Het bestand is al geopend. |

## Opmerkingen

Deze constructor decompresseert niet. Zie de [`Open`](../open/) methode voor decompressie.

## Voorbeelden

Open een archief vanuit een bestand via pad en decodeer het naar een `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive("archive.uue"))
  archive.Open().CopyTo(ms);
```

### Zie ook

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


