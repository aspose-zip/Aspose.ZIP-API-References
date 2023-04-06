---
title: ZArchive.Extract
second_title: Aspose.ZIP voor .NET API-referentie
description: ZArchive methode. Extraheert Zarchief naar een stream.
type: docs
weight: 30
url: /nl/net/aspose.zip.z/zarchive/extract/
---
## Extract(Stream) {#extract_2}

Extraheert Z-archief naar een stream.

```csharp
public void Extract(Stream destination)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destination | Stream | Stream voor het opslaan van gedecomprimeerde gegevens. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| InvalidDataException | Gegevens kunnen niet worden gedecomprimeerd. |

### Voorbeelden

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new ZArchive(zFile))
        {
            archive.Extract(extractedFile);
        }
    }
}
```

### Zie ook

* class [ZArchive](../)
* naamruimte [Aspose.Zip.Z](../../zarchive/)
* montage [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Pakt het Z-archief uit naar een bestand.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo voor het opslaan van gedecomprimeerde gegevens. |

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
| InvalidDataException | Gegevens kunnen niet worden gedecomprimeerd. |

### Voorbeelden

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ZArchive(zFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### Zie ook

* class [ZArchive](../)
* naamruimte [Aspose.Zip.Z](../../zarchive/)
* montage [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Pakt Z-archief uit naar een bestand op pad.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Pad naar bestand waarin gedecomprimeerde gegevens worden opgeslagen. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *path* is niets. |
| SecurityException | De beller heeft niet de vereiste toegangsrechten. |
| ArgumentException | De*path* is leeg, bevat alleen spaties of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot dossier*path* wordt ontkend. |
| PathTooLongException | De opgegeven*path*, bestandsnaam of beide overschrijden de door het systeem gedefinieerde maximale lengte. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. |
| NotSupportedException | Dossier bij*path* bevat een dubbele punt (:) in het midden van de tekenreeks. |
| InvalidDataException | Gegevens kunnen niet worden gedecomprimeerd. |

### Voorbeelden

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ZArchive(zFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Zie ook

* class [ZArchive](../)
* naamruimte [Aspose.Zip.Z](../../zarchive/)
* montage [Aspose.Zip](../../../)


