---
title: "CabArchive.CreateEntries"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "CabArchive‑methode. Voegt alle bestanden recursief toe aan het archief vanuit de opgegeven map"
type: docs
weight: 30
url: /nl/net/aspose.zip.cab/cabarchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Voegt alle bestanden recursief toe aan het archief vanuit de opgegeven map.

```csharp
public CabArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| directory | DirectoryInfo | Map om te comprimeren. |
| includeRootDirectory | Boolean | Geeft aan of de naam van de hoofdmap moet worden opgenomen in de entry‑paden. |

### Retourwaarde

De huidige [`CabArchive`](../)‑instantie.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *directory* is null. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| DirectoryNotFoundException | *directory* kan niet worden gevonden. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om *directory* of de inhoud ervan te benaderen. |
| UnauthorizedAccessException | Toegang tot *directory* of een van de bestanden ervan is geweigerd. |
| IOException | Er treedt een I/O-fout op tijdens het benaderen van *directory*. |
| PathTooLongException | Een gegenereerd invoerpad overschrijdt de systeemgedefinieerde maximale lengte. |
| InvalidOperationException | Het archief is voorbereid op extractie en kan geen items toevoegen. |

## Voorbeelden

```csharp
using (var archive = new CabArchive())
{
    var directory = new DirectoryInfo("logs");
    archive.CreateEntries(directory);
    archive.Save("logs.cab");
}
```

### Zie ook

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Voegt alle bestanden recursief toe aan het archief vanaf het opgegeven directorypad.

```csharp
public CabArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceDirectory | String | Directorypad om te comprimeren. |
| includeRootDirectory | Boolean | Geeft aan of de naam van de hoofdmap moet worden opgenomen in de entry‑paden. |

### Retourwaarde

De huidige [`CabArchive`](../)‑instantie.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| ArgumentNullException | *sourceDirectory* is null. |
| DirectoryNotFoundException | *sourceDirectory* kan niet worden gevonden. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om *sourceDirectory* te benaderen. |
| UnauthorizedAccessException | Toegang tot *sourceDirectory* is geweigerd. |
| PathTooLongException | Het opgegeven *sourceDirectory* overschrijdt de systeemgedefinieerde maximale lengte. |
| ArgumentException | *sourceDirectory* is leeg, bevat alleen witruimtes, of bevat ongeldige tekens. |
| IOException | Er treedt een I/O-fout op tijdens het benaderen van *sourceDirectory*. |
| InvalidOperationException | Het archief is voorbereid op extractie en kan geen items toevoegen. |

## Voorbeelden

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabStoreCompressionSettings())))
{
    archive.CreateEntries("data", includeRootDirectory: false);
    archive.Save("stored_data.cab");
}
```

### Zie ook

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


