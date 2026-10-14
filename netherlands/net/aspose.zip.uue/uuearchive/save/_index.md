---
title: "UueArchive.Save"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "UueArchive-methode. Slaat het archief op in de opgegeven stream"
type: docs
weight: 70
url: /nl/net/aspose.zip.uue/uuearchive/save/
---
## Save(Stream, UueSaveOptions) {#save}

Slaat het archief op in de opgegeven stream.

```csharp
public void Save(Stream outputStream, UueSaveOptions saveOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| outputStream | Stream | Doelstream. |
| saveOptions | UueSaveOptions | Opties voor het opslaan van het archief. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| InvalidOperationException | De bron van de te archiveren gegevens is niet opgegeven. |
| ArgumentException | *outputStream* is niet beschrijfbaar. |
| UnauthorizedAccessException | Bestandsbron is alleen-lezen of is een map. |
| DirectoryNotFoundException | Het opgegeven pad van de bestandsbron is ongeldig, bijvoorbeeld omdat het zich op een niet-toegewezen station bevindt. |
| IOException | De bestandsbron is al geopend. |

## Opmerkingen

*outputStream* must be writable.

## Voorbeelden

Schrijf gecomprimeerde gegevens naar de http-responsestream.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Zie ook

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, UueSaveOptions) {#save_1}

Slaat het archief op in een opgegeven bestemmingsbestand.

```csharp
public void Save(string destinationFileName, UueSaveOptions saveOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationFileName | String | Het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand verwijst, wordt dit overschreven. |
| saveOptions | UueSaveOptions | Opties voor het opslaan van het archief. |

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
| InvalidOperationException | De bron van de te archiveren gegevens is niet opgegeven. |

## Voorbeelden

Schrijf gecodeerde gegevens naar bestand.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.uue");
}
```

### Zie ook

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


