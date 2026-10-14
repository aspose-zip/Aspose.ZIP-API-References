---
title: "IsoArchive.Save"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "IsoArchive-methode. Slaat het ISO‑beeld op naar het opgegeven pad."
type: docs
weight: 70
url: /nl/net/aspose.zip.iso/isoarchive/save/
---
## Save(string, IsoSaveOptions) {#save_1}

Slaat het ISO‑beeld op op het opgegeven pad.

```csharp
public void Save(string path, IsoSaveOptions saveOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Het pad waar het ISO‑beeld wordt opgeslagen. |
| saveOptions | IsoSaveOptions | Opties om het ISO‑archief mee op te slaan. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| InvalidOperationException | Wordt opgegooid wanneer het archief zich niet in bewerkingsmodus bevindt. |
| ArgumentNullException | Wordt opgegooid wanneer de *path* null is. |
| DirectoryNotFoundException | Wordt opgegooid wanneer het opgegeven pad ongeldig is, bijvoorbeeld omdat het zich op een niet-toegewezen station bevindt. |
| IOException | Wordt opgegooid wanneer het bestand al geopend is. |
| UnauthorizedAccessException | Wordt opgegooid wanneer de toegang tot het bestand *path* wordt geweigerd. |
| PathTooLongException | Wordt opgegooid wanneer het opgegeven *path* de door het systeem gedefinieerde maximale lengte overschrijdt. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |

## Voorbeelden

Het volgende voorbeeld toont hoe een ISO‑archief naar een bestand kan worden opgeslagen:

```csharp
// Maak een nieuw leeg ISO-archief
using(IsoArchive isoArchive = new IsoArchive())
{
    // Voeg bestanden toe aan het ISO-archief
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // Sla het ISO-archief op in een bestand
    isoArchive.Save("new_archive.iso");
}
```

### Zie ook

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, IsoSaveOptions) {#save}

Slaat het ISO‑beeld op in de opgegeven stream.

```csharp
public void Save(Stream stream, IsoSaveOptions saveOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | Stream | De stream waar het ISO‑beeld wordt opgeslagen. |
| saveOptions | IsoSaveOptions | Opties om het ISO‑archief mee op te slaan. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| InvalidOperationException | Wordt opgegooid wanneer het archief zich niet in bewerkingsmodus bevindt. |
| ArgumentNullException | Wordt opgegooid wanneer de *stream* null is. |
| ArgumentException | Wordt gegooid wanneer de *stream* niet schrijfbaar is. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| IOException | Er treedt een I/O-fout op. |

## Voorbeelden

Het volgende voorbeeld laat zien hoe een ISO-archief naar een geheugenstroom wordt opgeslagen:

```csharp

 // Maak een nieuw leeg ISO-archief
 using(IsoArchive isoArchive = new IsoArchive())
 {
     // Voeg bestanden toe aan het ISO-archief
     isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

     // Sla het ISO-archief op naar een geheugenstroom
     isoArchive.Save(memoryStream);
 }
```

### Zie ook

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


