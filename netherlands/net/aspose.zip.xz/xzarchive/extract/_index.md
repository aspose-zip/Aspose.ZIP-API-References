---
title: XzArchive.Extract
second_title: Aspose.ZIP voor .NET API-referentie
description: XzArchive methode. Extraheert xzarchief naar een stream.
type: docs
weight: 30
url: /nl/net/aspose.zip.xz/xzarchive/extract/
---
## Extract(Stream) {#extract_2}

Extraheert xz-archief naar een stream.

```csharp
public void Extract(Stream destination)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destination | Stream | Stream voor het opslaan van gedecomprimeerde gegevens. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| InvalidOperationException | Archiefkoppen en service-informatie zijn niet gelezen. |

### Voorbeelden

```csharp
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new XzArchive(xzFile))
        {
            archive.Extract(extractedFile);
        }
    }
}
```

### Zie ook

* class [XzArchive](../)
* naamruimte [Aspose.Zip.Xz](../../xzarchive/)
* montage [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Pakt xz-archief uit naar een bestand.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo voor het opslaan van gedecomprimeerde gegevens. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| InvalidOperationException | Archiefkoppen en service-informatie zijn niet gelezen. |
| SecurityException | De beller heeft niet de vereiste toestemming om het*fileInfo*. |
| ArgumentException | Bestandspad is leeg of bevat alleen spaties. |
| FileNotFoundException | Het bestand is niet gevonden. |
| UnauthorizedAccessException | Pad naar bestand is alleen-lezen of is een directory. |
| ArgumentNullException | *fileInfo* is niets. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, omdat het zich bijvoorbeeld op een niet-toegewezen schijf bevindt. |
| IOException | Het bestand is al geopend. |

### Voorbeelden

```csharp
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new XzArchive(xzFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### Zie ook

* class [XzArchive](../)
* naamruimte [Aspose.Zip.Xz](../../xzarchive/)
* montage [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Pakt xz-archief uit naar een bestand op pad.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Pad naar bestand waarin gedecomprimeerde gegevens worden opgeslagen. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| InvalidOperationException | Archiefkoppen en service-informatie zijn niet gelezen. |
| ArgumentNullException | *path* is niets. |
| SecurityException | De beller heeft niet de vereiste toegangsrechten. |
| ArgumentException | De*path* is leeg, bevat alleen spaties of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot dossier*path* wordt ontkend. |
| PathTooLongException | De opgegeven*path*, bestandsnaam of beide overschrijden de door het systeem gedefinieerde maximale lengte. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. |
| NotSupportedException | Dossier bij*path* bevat een dubbele punt (:) in het midden van de tekenreeks. |

### Voorbeelden

```csharp
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new XzArchive(xzFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Zie ook

* class [XzArchive](../)
* naamruimte [Aspose.Zip.Xz](../../xzarchive/)
* montage [Aspose.Zip](../../../)


