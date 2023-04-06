---
title: Archive.CreateEntries
second_title: Aspose.ZIP voor .NET API-referentie
description: Archive methode. Voegt recursief alle bestanden en mappen toe aan het archief in de opgegeven map.
type: docs
weight: 40
url: /nl/net/aspose.zip/archive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Voegt recursief alle bestanden en mappen toe aan het archief in de opgegeven map.

```csharp
public Archive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| directory | DirectoryInfo | Directory om te comprimeren. |
| includeRootDirectory | Boolean | Geeft aan of de hoofdmap zelf moet worden opgenomen of niet. |

### Winstwaarde

Het archief met inzendingen samengesteld.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| DirectoryNotFoundException | Het pad naar*directory* ongeldig is, bijvoorbeeld op een niet-toegewezen schijf. |
| SecurityException | De beller heeft niet de vereiste toegangsrechten*directory*. |

### Voorbeelden

```csharp
using (Archive archive = new Archive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.zip");
}
```

### Zie ook

* class [Archive](../)
* naamruimte [Aspose.Zip](../../archive/)
* montage [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Voegt recursief alle bestanden en mappen toe aan het archief in de opgegeven map.

```csharp
public Archive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceDirectory | String | Directory om te comprimeren. |
| includeRootDirectory | Boolean | Geeft aan of de hoofdmap zelf moet worden opgenomen of niet. |

### Winstwaarde

Het archief met inzendingen samengesteld.

### Voorbeelden

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.zip");
}
```

### Zie ook

* class [Archive](../)
* naamruimte [Aspose.Zip](../../archive/)
* montage [Aspose.Zip](../../../)


