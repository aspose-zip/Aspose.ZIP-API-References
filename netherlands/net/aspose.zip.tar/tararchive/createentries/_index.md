---
title: TarArchive.CreateEntries
second_title: Aspose.ZIP voor .NET API-referentie
description: TarArchive methode. Voegt recursief alle bestanden en mappen toe aan het archief in de gegeven map.
type: docs
weight: 70
url: /nl/net/aspose.zip.tar/tararchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Voegt recursief alle bestanden en mappen toe aan het archief in de gegeven map.

```csharp
public TarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| directory | DirectoryInfo | Directory om te comprimeren. |
| includeRootDirectory | Boolean | Geeft aan of de hoofdmap zelf moet worden opgenomen of niet. |

### Winstwaarde

Het archief met inzendingen samengesteld.

### Voorbeelden

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(tarFile);
    }
}
```

### Zie ook

* class [TarArchive](../)
* naamruimte [Aspose.Zip.Tar](../../tararchive/)
* montage [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Voegt recursief alle bestanden en mappen toe aan het archief in de gegeven map.

```csharp
public TarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceDirectory | String | Directory om te comprimeren. |
| includeRootDirectory | Boolean | Geeft aan of de hoofdmap zelf moet worden opgenomen of niet. |

### Winstwaarde

Het archief met inzendingen samengesteld.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *sourceDirectory* is niets. |
| SecurityException | De beller heeft niet de vereiste toegangsrechten*sourceDirectory*. |
| ArgumentException | *sourceDirectory* bevat ongeldige tekens zoals ", &lt;, &gt; of &#x7C;. |
| PathTooLongException | Het opgegeven pad, de bestandsnaam of beide overschrijden de door het systeem gedefinieerde maximale lengte. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. Het opgegeven pad, de bestandsnaam of beide zijn te lang. |

### Voorbeelden

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(tarFile);
    }
}
```

### Zie ook

* class [TarArchive](../)
* naamruimte [Aspose.Zip.Tar](../../tararchive/)
* montage [Aspose.Zip](../../../)


