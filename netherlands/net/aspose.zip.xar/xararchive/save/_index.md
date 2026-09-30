---
title: "XarArchive.Save"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "XarArchive-methode. Slaat het archief op naar het opgegeven bestemmingsbestand."
type: docs
weight: 80
url: /nl/net/aspose.zip.xar/xararchive/save/
---
## Save(string, XarSaveOptions) {#save_1}

Slaat het archief op naar het opgegeven bestemmingsbestand.

```csharp
public void Save(string destinationFileName, XarSaveOptions saveOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationFileName | String | Het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand verwijst, wordt dit overschreven. |
| saveOptions | XarSaveOptions | Opties om het xar-archief mee op te slaan. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *destinationFileName* is null. |
| InvalidOperationException | Het is niet mogelijk om het xar-archief te wijzigen. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| IOException | Er trad een I/O-fout op tijdens het openen van het bestand. |
| PathTooLongException | Het opgegeven pad, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. |
| UnauthorizedAccessException | *destinationFileName* gaf een bestand op dat alleen-lezen is. -of- *destinationFileName* gaf een map op. -of- De aanroeper heeft niet de vereiste toestemming. |

### Zie ook

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, XarSaveOptions) {#save}

Slaat het archief op in de opgegeven stream.

```csharp
public void Save(Stream output, XarSaveOptions saveOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| uitvoer | Stream | Doelstream. |
| saveOptions | XarSaveOptions | Opties om het xar-archief mee op te slaan. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *output* is null. |
| ArgumentException | *output* is niet schrijfbaar/leesbaar of niet doorzoekbaar. |
| InvalidOperationException | Het is niet mogelijk om het xar-archief te wijzigen. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |

### Zie ook

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


