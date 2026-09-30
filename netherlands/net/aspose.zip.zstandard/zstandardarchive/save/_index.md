---
title: "ZstandardArchive.Save"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "ZstandardArchive-methode. Slaat het archief op in de opgegeven stream."
type: docs
weight: 60
url: /nl/net/aspose.zip.zstandard/zstandardarchive/save/
---
## Save(Stream, ZstandardSaveOptions) {#save_1}

Slaat het archief op in de opgegeven stream.

```csharp
public void Save(Stream outputStream, ZstandardSaveOptions settings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| outputStream | Stream | Doelstream. |
| instellingen | ZstandardSaveOptions | Optionele instellingen voor het samenstellen van het archief. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| ArgumentException | *outputStream* is niet beschrijfbaar. |
| InvalidOperationException | Bron is niet opgegeven. |

## Opmerkingen

*outputStream* must be writable.

## Voorbeelden

Schrijf gecomprimeerde gegevens naar de http-responsestream.

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Zie ook

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, ZstandardSaveOptions) {#save_2}

Slaat het archief op naar het opgegeven bestemmingsbestand.

```csharp
public void Save(string destinationFileName, ZstandardSaveOptions settings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationFileName | String | Het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand verwijst, wordt dit overschreven. |
| instellingen | ZstandardSaveOptions | Optionele instellingen voor het samenstellen van het archief. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| ArgumentNullException | *destinationFileName* is null. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om toegang te krijgen. |
| ArgumentException | De *destinationFileName* is leeg, bevat alleen witruimtes, of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot bestand *destinationFileName* is geweigerd. |
| PathTooLongException | De opgegeven *destinationFileName*, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens en bestandsnamen korter dan 260 tekens. |
| NotSupportedException | Bestand op *destinationFileName* bevat een dubbele punt (:) in het midden van de tekenreeks. |
| Exception | Wordt gegooid wanneer een runtime-fout optreedt. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, (bijvoorbeeld, het bevindt zich op een niet-toegewezen station). |
| IOException | Er trad een I/O-fout op tijdens het openen van het bestand. |
| InvalidOperationException | Bron is niet opgegeven. |

## Voorbeelden

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.zst");
}
```

### Zie ook

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo, ZstandardSaveOptions) {#save}

Slaat het archief op naar het opgegeven bestemmingsbestand.

```csharp
public void Save(FileInfo destination, ZstandardSaveOptions settings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | FileInfo | FileInfo, die wordt geopend als bestemmings‑stream. |
| instellingen | ZstandardSaveOptions | Optionele instellingen voor het samenstellen van het archief. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om de *destination* te openen. |
| ArgumentException | Het bestandspad is leeg of bevat alleen witruimtes. |
| FileNotFoundException | Het bestand is niet gevonden. |
| UnauthorizedAccessException | Pad naar bestand is alleen-lezen of is een map. |
| ArgumentNullException | *destination* is null. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, bijvoorbeeld omdat het zich op een niet-toegewezen station bevindt. |
| IOException | Het bestand is al geopend. |
| InvalidOperationException | Bron is niet opgegeven. |

## Voorbeelden

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.zst"));
}
```

### Zie ook

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


