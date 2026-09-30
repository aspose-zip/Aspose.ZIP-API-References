---
title: "Lz4Archive.Save"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "Lz4Archive-methode. Slaat het lz4-archief op in de opgegeven stream"
type: docs
weight: 60
url: /nl/net/aspose.zip.lz4/lz4archive/save/
---
## Save(Stream) {#save_1}

Slaat het lz4-archief op naar de opgegeven stream.

```csharp
public void Save(Stream output)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| uitvoer | Stream | Doelstream. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *output* is null. |
| ArgumentException | *output* is niet beschrijfbaar. |
| InvalidOperationException | Het archief is klaar voor extractie. - of - Bron is niet opgegeven. |
| OperationCanceledException | In .NET Framework 4.0 en hoger: Wordt gegooid wanneer de compressie wordt geannuleerd via het opgegeven annulerings‑token. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |

## Opmerkingen

*output* must be seekable.

## Voorbeelden

```csharp
using (FileStream lz4File = File.Open("archive.lz4", FileMode.Create))
{
    using (var archive = new Lz4Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(lz4File);
     }
}
```

### Zie ook

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Slaat het lz4-archief op naar het opgegeven bestemmingsbestand.

```csharp
public void Save(FileInfo destination)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | FileInfo | FileInfo, die wordt geopend als bestemmings‑stream. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om de *destination* te openen. |
| ArgumentException | Het bestandspad is leeg of bevat alleen witruimtes. |
| FileNotFoundException | Het bestand is niet gevonden. |
| UnauthorizedAccessException | Pad naar bestand is alleen-lezen of is een map. |
| ArgumentNullException | *destination* is null. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, bijvoorbeeld omdat het zich op een niet-toegewezen station bevindt. |
| IOException | Het bestand is al geopend. |
| InvalidOperationException | Het archief is voorbereid op extractie. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |

## Voorbeelden

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz4"));
}
```

### Zie ook

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

Slaat het archief op naar het opgegeven bestemmingsbestand.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationFileName | String | Het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand verwijst, wordt dit overschreven. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *destinationFileName* is null. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om toegang te krijgen |
| ArgumentException | De *destinationFileName* is leeg, bevat alleen witruimtes, of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot bestand *destinationFileName* is geweigerd. |
| PathTooLongException | De opgegeven *destinationFileName*, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens en bestandsnamen korter dan 260 tekens. |
| NotSupportedException | Bestand op *destinationFileName* bevat een dubbele punt (:) in het midden van de tekenreeks. |
| InvalidOperationException | Het archief is voorbereid op extractie. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, (bijvoorbeeld, het bevindt zich op een niet-toegewezen station). |
| FileNotFoundException | Het bestand opgegeven in *destinationFileName* werd niet gevonden. |
| IOException | Er trad een I/O-fout op tijdens het openen van het bestand. |

## Voorbeelden

```csharp
using (var archive = new LZ4Archive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### Zie ook

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


