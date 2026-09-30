---
title: "XarArchive.CreateEntries"
second_title: "Aspose.ZIP för .NET API-referens"
description: "XarArchive-metod. Lägger till i arkivet alla filer och kataloger rekursivt i den angivna katalogen"
type: docs
weight: 30
url: /sv/net/aspose.zip.xar/xararchive/createentries/
---
## CreateEntries(string, bool, XarCompressionSettings) {#createentries_1}

Lägger till i arkivet alla filer och kataloger rekursivt i den angivna katalogen.

```csharp
public XarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceDirectory | String | Katalog att komprimera. |
| compressionSettings | Boolean | Komprimeringsinställningarna som används för tillagda [`XarEntry`](../../xarentry/)‑objekt. |
| includeRootDirectory | XarCompressionSettings | Anger om rotkatalogen själv ska inkluderas eller inte. |

### Returvärde

Xar-objektinstans.

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *sourceDirectory* är null. |
| SecurityException | Anroparen har inte den nödvändiga behörigheten för att komma åt *sourceDirectory*. |
| ArgumentException | *sourceDirectory* innehåller ogiltiga tecken såsom \", &lt;, &gt;, eller &#x7C;. |
| PathTooLongException | Den angivna sökvägen, filnamnet eller båda överskrider den systemdefinierade maximala längden. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken, och filnamn måste vara kortare än 260 tecken. Den angivna sökvägen, filnamnet eller båda är för långa. |
| IOException | *sourceDirectory* representerar en fil, inte en katalog. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Exempel

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

### Se även

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool, XarCompressionSettings) {#createentries}

Lägger till i arkivet alla filer och kataloger rekursivt i den angivna katalogen.

```csharp
public XarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| directory | DirectoryInfo | Katalog att komprimera. |
| compressionSettings | Boolean | Komprimeringsinställningarna som används för tillagda [`XarEntry`](../../xarentry/)‑objekt. |
| includeRootDirectory | XarCompressionSettings | Anger om rotkatalogen själv ska inkluderas eller inte. |

### Returvärde

Xar-objektinstans.

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *directory* är null. |
| SecurityException | Anroparen har inte den nödvändiga behörigheten för att komma åt *directory*. |
| IOException | *directory* representerar en fil, inte en katalog. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Exempel

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

### Se även

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


