---
title: "ZstandardArchive.SetSource"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "ZstandardArchive methode. Stelt de inhoud in die binnen het archief moet worden gecomprimeerd."
type: docs
weight: 70
url: /nl/net/aspose.zip.zstandard/zstandardarchive/setsource/
---
## SetSource(Stream) {#setsource_1}

Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```csharp
public void SetSource(Stream source)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bron | Stream | De invoerstream voor het archief. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |

## Voorbeelden

```csharp
using (var archive = new ZstandardArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.zst");
}
```

### Zie ook

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileInfo | FileInfo | De referentie naar een bestand dat moet worden gecomprimeerd. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |

## Voorbeelden

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.zst");
}
```

### Zie ook

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```csharp
public void SetSource(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Pad naar bestand dat moet worden gecomprimeerd. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| ArgumentNullException | *path* is null. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om toegang te krijgen. |
| ArgumentException | Het *path* is leeg, bevat alleen witruimtes, of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot bestand *path* is geweigerd. |
| PathTooLongException | Het opgegeven *path*, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens, en bestandsnamen korter dan 260 tekens. |
| NotSupportedException | Bestand op *path* bevat een dubbele punt (:) in het midden van de tekenreeks. |

## Voorbeelden

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.zst");
}
```

### Zie ook

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


