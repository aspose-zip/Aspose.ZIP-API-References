---
title: "XarArchive.CreateEntries"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "XarArchive-methode. Voegt alle bestanden en mappen recursief toe aan het archief in de opgegeven map."
type: docs
weight: 30
url: /nl/net/aspose.zip.xar/xararchive/createentries/
---
## CreateEntries(string, bool, XarCompressionSettings) {#createentries_1}

Voegt alle bestanden en mappen recursief toe aan het archief in de opgegeven map.

```csharp
public XarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceDirectory | String | Map om te comprimeren. |
| compressionSettings | Boolean | De compressie-instellingen die worden gebruikt voor toegevoegde [`XarEntry`](../../xarentry/) items. |
| includeRootDirectory | XarCompressionSettings | Geeft aan of de hoofdmap zelf moet worden opgenomen of niet. |

### Retourwaarde

Xar entry instantie.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *sourceDirectory* is null. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om *sourceDirectory* te benaderen. |
| ArgumentException | *sourceDirectory* bevat ongeldige tekens zoals ", &lt;, &gt;, of &#x7C;. |
| PathTooLongException | Het opgegeven pad, de bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens, en bestandsnamen korter dan 260 tekens. Het opgegeven pad, de bestandsnaam, of beide zijn te lang. |
| IOException | *sourceDirectory* staat voor een bestand, niet voor een map. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |

## Voorbeelden

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(@"C:\folder", false);
        archive.Save(xarFile);
    }
}
```

### Zie ook

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool, XarCompressionSettings) {#createentries}

Voegt alle bestanden en mappen recursief toe aan het archief in de opgegeven map.

```csharp
public XarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| directory | DirectoryInfo | Map om te comprimeren. |
| compressionSettings | Boolean | De compressie-instellingen die worden gebruikt voor toegevoegde [`XarEntry`](../../xarentry/) items. |
| includeRootDirectory | XarCompressionSettings | Geeft aan of de hoofdmap zelf moet worden opgenomen of niet. |

### Retourwaarde

Xar entry instantie.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *directory* is null. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om *directory* te benaderen. |
| IOException | *directory* staat voor een bestand, niet voor een map. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |

## Voorbeelden

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(new DirectoryInfo(@"C:\folder"), false);
        archive.Save(xarFile);
    }
}
```

### Zie ook

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


