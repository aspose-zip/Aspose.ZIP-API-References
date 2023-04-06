---
title: SevenZipArchive.CreateEntries
second_title: Aspose.ZIP voor .NET API-referentie
description: SevenZipArchive methode. Voegt recursief alle bestanden en mappen toe aan het archief in de opgegeven map.
type: docs
weight: 40
url: /nl/net/aspose.zip.sevenzip/sevenziparchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Voegt recursief alle bestanden en mappen toe aan het archief in de opgegeven map.

```csharp
public SevenZipArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
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
using (SevenZipArchive archive = new SevenZipArchive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.7z");
}
```

### Zie ook

* class [SevenZipArchive](../)
* naamruimte [Aspose.Zip.SevenZip](../../sevenziparchive/)
* montage [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Voegt recursief alle bestanden en mappen toe aan het archief in de opgegeven map.

```csharp
public SevenZipArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceDirectory | String | Directory om te comprimeren. |
| includeRootDirectory | Boolean | Geeft aan of de hoofdmap zelf moet worden opgenomen of niet. |

### Winstwaarde

Het archief met inzendingen samengesteld.

### Voorbeelden

Stel 7z-archief samen met LZMA2-compressie.

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.7z");
}
```

### Zie ook

* class [SevenZipArchive](../)
* naamruimte [Aspose.Zip.SevenZip](../../sevenziparchive/)
* montage [Aspose.Zip](../../../)


