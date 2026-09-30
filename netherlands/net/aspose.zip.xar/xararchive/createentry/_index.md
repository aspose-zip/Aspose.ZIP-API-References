---
title: "XarArchive.CreateEntry"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "XarArchive methode. Maak een enkel item binnen het archief"
type: docs
weight: 40
url: /nl/net/aspose.zip.xar/xararchive/createentry/
---
## CreateEntry(string, FileInfo, bool, XarCompressionSettings) {#createentry}

Maak een enkel item binnen het archief.

```csharp
public XarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| fileInfo | FileInfo | De metadata van het bestand of de map die moet worden gecomprimeerd. |
| openImmediately | Boolean | True, als het bestand onmiddellijk moet worden geopend, anders wordt het bestand geopend bij het opslaan van het archief. |
| compressionSettings | XarCompressionSettings | De compressie-instellingen die worden gebruikt voor het toegevoegde [`XarEntry`](../../xarentry/) item. |

### Retourwaarde

Xar entry instantie.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *name* is null. |
| ArgumentException | *name* is leeg. |
| ArgumentNullException | *fileInfo* is null. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |

## Opmerkingen

Als het bestand onmiddellijk wordt geopend met de *openImmediately* parameter, wordt het geblokkeerd totdat het archief wordt vrijgegeven.

## Voorbeelden

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new XarArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.xar");
}
```

### Zie ook

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, XarCompressionSettings) {#createentry_2}

Maak een enkel item binnen het archief.

```csharp
public XarEntry CreateEntry(string name, string sourcePath, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| sourcePath | String | Pad naar bestand dat moet worden gecomprimeerd. |
| openImmediately | Boolean | True, als het bestand onmiddellijk moet worden geopend, anders wordt het bestand geopend bij het opslaan van het archief. |
| compressionSettings | XarCompressionSettings | De compressie-instellingen die worden gebruikt voor het toegevoegde [`XarEntry`](../../xarentry/) item. |

### Retourwaarde

Xar entry instantie.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *sourcePath* is null. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om toegang te krijgen. |
| ArgumentException | De *sourcePath* is leeg, bevat alleen witruimtes, of bevat ongeldige tekens. - of - Bestandsnaam, als onderdeel van *name*, overschrijdt 100 tekens. |
| UnauthorizedAccessException | Toegang tot bestand *sourcePath* is geweigerd. |
| PathTooLongException | De opgegeven *sourcePath*, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens, en bestandsnamen korter dan 260 tekens. - of - *name* is te lang voor xar. |
| NotSupportedException | Bestand op *sourcePath* bevat een dubbele punt (:) in het midden van de tekenreeks. |
| InvalidOperationException | Het is niet mogelijk om het xar-archief te wijzigen. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |

## Opmerkingen

De entrynaam wordt uitsluitend ingesteld via de *name* parameter. De bestandsnaam die is opgegeven in de *sourcePath* parameter heeft geen invloed op de entrynaam.

Als het bestand onmiddellijk wordt geopend met de *openImmediately* parameter, wordt het geblokkeerd totdat het archief wordt vrijgegeven.

## Voorbeelden

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### Zie ook

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, XarCompressionSettings) {#createentry_1}

Maak een enkel item binnen het archief.

```csharp
public XarEntry CreateEntry(string name, Stream source, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| bron | Stream | De invoerstroom voor het item. |
| compressionSettings | XarCompressionSettings | De compressie-instellingen die worden gebruikt voor het toegevoegde [`XarEntry`](../../xarentry/) item. |

### Retourwaarde

Xar entry instantie.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *name* is null. |
| ArgumentNullException | *source* is null. |
| ArgumentException | *name* is leeg. |
| InvalidOperationException | Het is niet mogelijk om het xar-archief te wijzigen. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |

## Voorbeelden

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.xar");
}
```

### Zie ook

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


