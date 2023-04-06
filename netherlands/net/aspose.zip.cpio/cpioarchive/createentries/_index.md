---
title: CpioArchive.CreateEntries
second_title: Aspose.ZIP voor .NET API-referentie
description: CpioArchive methode. Voegt recursief alle bestanden en mappen toe aan het archief in de gegeven map.
type: docs
weight: 30
url: /nl/net/aspose.zip.cpio/cpioarchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

Voegt recursief alle bestanden en mappen toe aan het archief in de gegeven map.

```csharp
public CpioArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceDirectory | String | Directory om te comprimeren. |
| includeRootDirectory | Boolean | Geeft aan of de hoofdmap zelf moet worden opgenomen of niet. |

### Winstwaarde

Cpio ingangsinstantie.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *sourceDirectory* is niets. |
| SecurityException | De beller heeft niet de vereiste toegangsrechten*sourceDirectory*. |
| ArgumentException | *sourceDirectory* bevat ongeldige tekens zoals ", &lt;, &gt; of &#x7C;. |
| PathTooLongException | Het opgegeven pad, de bestandsnaam of beide overschrijden de door het systeem gedefinieerde maximale lengte. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. Het opgegeven pad, de bestandsnaam of beide zijn te lang. |
| IOException | *sourceDirectory* staat voor een bestand, niet voor een map. |

### Voorbeelden

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(cpioFile);
    }
}
```

### Zie ook

* class [CpioArchive](../)
* naamruimte [Aspose.Zip.Cpio](../../cpioarchive/)
* montage [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

Voegt recursief alle bestanden en mappen toe aan het archief in de gegeven map.

```csharp
public CpioArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| directory | DirectoryInfo | Directory om te comprimeren. |
| includeRootDirectory | Boolean | Geeft aan of de hoofdmap zelf moet worden opgenomen of niet. |

### Winstwaarde

Cpio ingangsinstantie.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *directory* is niets. |
| SecurityException | De beller heeft niet de vereiste toegangsrechten*directory*. |
| IOException | *directory* staat voor een bestand, niet voor een map. |

### Voorbeelden

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(cpioFile);
    }
}
```

### Zie ook

* class [CpioArchive](../)
* naamruimte [Aspose.Zip.Cpio](../../cpioarchive/)
* montage [Aspose.Zip](../../../)


