---
title: SevenZipArchive.Save
second_title: Aspose.ZIP voor .NET API-referentie
description: SevenZipArchive methode. Slaat 7zarchief op in de geleverde stream.
type: docs
weight: 80
url: /nl/net/aspose.zip.sevenzip/sevenziparchive/save/
---
## Save(Stream) {#save}

Slaat 7z-archief op in de geleverde stream.

```csharp
public void Save(Stream output)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| output | Stream | Bestemmingsstroom. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentException | *output* ondersteunt het zoeken niet. |
| ArgumentNullException | *output* is niets. |
| InvalidOperationException | Encoder kan gegevens niet comprimeren. |

### Opmerkingen

*output* moet vindbaar zijn.

### Voorbeelden

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
  using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
  {
    using (var archive = new SevenZipArchive())
    {
      archive.CreateEntry("data", source);
      archive.Save(sevenZipFile);
    }
  }
}
```

### Zie ook

* class [SevenZipArchive](../)
* naamruimte [Aspose.Zip.SevenZip](../../sevenziparchive/)
* montage [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Slaat archief op in opgegeven bestemmingsbestand.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationFileName | String | Het pad van het aan te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand verwijst, wordt dit overschreven. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *destinationFileName* is niets. |
| SecurityException | De beller heeft niet de vereiste toegangsrechten. |
| ArgumentException | De*destinationFileName* is leeg, bevat alleen spaties of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot dossier*destinationFileName* wordt ontkend. |
| PathTooLongException | De opgegeven*destinationFileName*, bestandsnaam of beide overschrijden de door het systeem gedefinieerde maximale lengte. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. |
| NotSupportedException | Dossier bij*destinationFileName* bevat een dubbele punt (:) in het midden van de tekenreeks. |

### Opmerkingen

Het is mogelijk om een archief op te slaan in hetzelfde pad als waaruit het is geladen. Dit wordt echter niet aanbevolen, omdat deze aanpak gebruikmaakt van kopiëren naar een tijdelijk bestand.

### Voorbeelden

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
   using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
   {
      archive.CreateEntry("data", source);
      archive.Save("archive.7z");
   }
}
```

### Zie ook

* class [SevenZipArchive](../)
* naamruimte [Aspose.Zip.SevenZip](../../sevenziparchive/)
* montage [Aspose.Zip](../../../)


