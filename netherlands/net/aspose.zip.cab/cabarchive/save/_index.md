---
title: "CabArchive.Save"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "CabArchive-methode. Slaat het archief op naar de opgegeven stream."
type: docs
weight: 70
url: /nl/net/aspose.zip.cab/cabarchive/save/
---
## Save(Stream, CabSaveOptions) {#save}

Slaat het archief op in de opgegeven stream.

```csharp
public void Save(Stream outputStream, CabSaveOptions saveOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| outputStream | Stream | Doelstream. |
| saveOptions | CabSaveOptions | Opties voor het opslaan van het archief. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentException | *outputStream* is niet schrijfbaar en zoekbaar. |
| ObjectDisposedException | Het archief is vrijgegeven. |
| InvalidOperationException | Het archief is voorbereid voor extractie en kan niet worden opgeslagen. |

## Opmerkingen

*outputStream* must be writable.

## Voorbeelden

```csharp
using (FileStream cabFile = File.Open("archive.cab", FileMode.Create))
{
    using (var archive = new CabArchive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(cabFile);
    }
}
```

### Zie ook

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, CabSaveOptions) {#save_1}

Slaat het archief op naar het opgegeven bestemmingsbestand.

```csharp
public void Save(string destinationFileName, CabSaveOptions saveOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationFileName | String | Het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand verwijst, wordt dit overschreven. |
| saveOptions | CabSaveOptions | Opties voor het opslaan van het archief. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *destinationFileName* is null. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om toegang te krijgen. |
| ArgumentException | De *destinationFileName* is leeg, bevat alleen witruimtes, of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot bestand *destinationFileName* is geweigerd. |
| PathTooLongException | De opgegeven *destinationFileName*, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens en bestandsnamen korter dan 260 tekens. |
| NotSupportedException | Bestand op *destinationFileName* bevat een dubbele punt (:) in het midden van de tekenreeks. |
| FileNotFoundException | Het bestand is niet gevonden. |
| InvalidOperationException | Het archief is geopend voor extractie. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, bijvoorbeeld omdat het zich op een niet-toegewezen station bevindt. |
| IOException | Het bestand is al geopend. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |

## Opmerkingen

Het is mogelijk om een archief op te slaan naar hetzelfde pad waarvan het is geladen. Dit wordt echter niet aanbevolen omdat deze aanpak een kopie naar een tijdelijk bestand gebruikt.

## Voorbeelden

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### Zie ook

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


