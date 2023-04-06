---
title: CpioArchive.Save
second_title: Aspose.ZIP voor .NET API-referentie
description: CpioArchive methode. Slaat archief op in opgegeven bestemmingsbestand.
type: docs
weight: 80
url: /nl/net/aspose.zip.cpio/cpioarchive/save/
---
## Save(string, CpioFormat) {#save_1}

Slaat archief op in opgegeven bestemmingsbestand.

```csharp
public void Save(string destinationFileName, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationFileName | String | Het pad van het aan te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand verwijst, wordt dit overschreven. |
| cpioFormat | CpioFormat | Definieert de indeling van de cpio-header. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentException | *destinationFileName* is een tekenreeks met lengte nul, bevat alleen witruimte of bevat een of meer ongeldige tekens zoals gedefinieerd door System.IO.Path.InvalidPathChars. |
| ArgumentNullException | *destinationFileName* is niets. |
| PathTooLongException | De opgegeven*destinationFileName*, bestandsnaam of beide overschrijden de door het systeem gedefinieerde maximale lengte. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. |
| DirectoryNotFoundException | De opgegeven*destinationFileName* ongeldig is (het staat bijvoorbeeld op een niet-toegewezen schijf). |
| IOException | Er is een I/O-fout opgetreden bij het openen van het bestand. |
| UnauthorizedAccessException | *destinationFileName* heeft een bestand opgegeven dat alleen-lezen is en de toegang is niet Read.-of- path heeft een map opgegeven.-of- De beller heeft niet de vereiste machtigingen. |
| NotSupportedException | *destinationFileName* heeft een ongeldig formaat. |

### Opmerkingen

Het is mogelijk om een archief op te slaan in hetzelfde pad als waaruit het is geladen. Dit wordt echter niet aanbevolen, omdat deze aanpak gebruikmaakt van kopiëren naar een tijdelijk bestand.

### Voorbeelden

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.cpio");
}       
```

### Zie ook

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* naamruimte [Aspose.Zip.Cpio](../../cpioarchive/)
* montage [Aspose.Zip](../../../)

---

## Save(Stream, CpioFormat) {#save}

Slaat archief op in de geleverde stream.

```csharp
public void Save(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| output | Stream | Bestemmingsstroom. |
| cpioFormat | CpioFormat | Definieert de indeling van de cpio-header. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *output* is niets. |
| ArgumentException | *output* is niet beschrijfbaar. - of -*output* is dezelfde stream waaruit we extraheren. - OF - Het is onmogelijk om het archief op te slaan in*cpioFormat* vanwege formaatbeperkingen. |

### Opmerkingen

*output*moet beschrijfbaar zijn.

### Voorbeelden

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(cpioFile);
    }
}       
```

### Zie ook

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* naamruimte [Aspose.Zip.Cpio](../../cpioarchive/)
* montage [Aspose.Zip](../../../)


