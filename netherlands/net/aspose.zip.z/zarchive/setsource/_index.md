---
title: ZArchive.SetSource
second_title: Aspose.ZIP voor .NET API-referentie
description: ZArchive methode. Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.
type: docs
weight: 50
url: /nl/net/aspose.zip.z/zarchive/setsource/
---
## SetSource(Stream) {#setsource_1}

Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```csharp
public void SetSource(Stream source)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | Stream | De invoerstroom voor het archief. |

### Voorbeelden

```csharp
using (var archive = new ZArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.Z");
}
```

### Zie ook

* class [ZArchive](../)
* naamruimte [Aspose.Zip.Z](../../zarchive/)
* montage [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo die wordt geopend als invoerstroom. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| SecurityException | De beller heeft niet de vereiste toestemming om het*fileInfo*. |
| ArgumentException | Bestandspad is leeg of bevat alleen spaties. |
| FileNotFoundException | Het bestand is niet gevonden. |
| UnauthorizedAccessException | Pad naar bestand is alleen-lezen of is een directory. |
| ArgumentNullException | *fileInfo* is niets. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, omdat het zich bijvoorbeeld op een niet-toegewezen schijf bevindt. |
| IOException | Het bestand is al geopend. |

### Voorbeelden

```csharp
using (var archive = new ZArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bin.Z");
}
```

### Zie ook

* class [ZArchive](../)
* naamruimte [Aspose.Zip.Z](../../zarchive/)
* montage [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```csharp
public void SetSource(string sourcePath)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourcePath | String | Pad naar bestand dat wordt geopend als invoerstroom. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *sourcePath* is null of een lege tekenreeks. |
| SecurityException | De beller heeft niet de vereiste toestemming om toegang te krijgen tot een bron. |
| ArgumentException | De*sourcePath* is leeg, bevat alleen spaties of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot dossier*sourcePath* wordt ontkend. |
| PathTooLongException | De opgegeven*sourcePath*, bestandsnaam of beide overschrijden de door het systeem gedefinieerde maximale lengte. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. |
| NotSupportedException | Dossier bij*sourcePath* bevat een dubbele punt (:) in het midden van de tekenreeks. |

### Voorbeelden

```csharp
using (var archive = new ZArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("data.bin.Z");
}
```

### Zie ook

* class [ZArchive](../)
* naamruimte [Aspose.Zip.Z](../../zarchive/)
* montage [Aspose.Zip](../../../)


