---
title: SharArchive.CreateEntry
second_title: Aspose.ZIP voor .NET API-referentie
description: SharArchive methode. Maak een enkel item binnen het archief.
type: docs
weight: 40
url: /nl/net/aspose.zip.shar/shararchive/createentry/
---
## CreateEntry(string, FileInfo, bool) {#createentry}

Maak een enkel item binnen het archief.

```csharp
public SharEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| fileInfo | FileInfo | De metadata van het bestand of de map die moet worden gecomprimeerd. |
| openImmediately | Boolean | Waar als het bestand onmiddellijk wordt geopend, anders opent u het bestand bij opslaan in het archief. |

### Winstwaarde

Shar entry-exemplaar.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *name* is niets. |
| ArgumentException | *name* is leeg. |
| ArgumentNullException | *fileInfo* is niets. |

### Opmerkingen

Als het bestand direct wordt geopend met*openImmediately*parameter wordt het geblokkeerd totdat het archief is verwijderd.

### Voorbeelden

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new SharArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.shar");
}
```

### Zie ook

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* naamruimte [Aspose.Zip.Shar](../../shararchive/)
* montage [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Maak een enkel item binnen het archief.

```csharp
public SharEntry CreateEntry(string name, string sourcePath, bool openImmediately = false)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| sourcePath | String | Pad naar te comprimeren bestand. |
| openImmediately | Boolean | Waar als het bestand onmiddellijk wordt geopend, anders opent u het bestand bij opslaan in het archief. |

### Winstwaarde

Shar entry-exemplaar.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *sourcePath* is niets. |
| SecurityException | De beller heeft niet de vereiste toegangsrechten. |
| ArgumentException | De*sourcePath* is leeg, bevat alleen spaties of bevat ongeldige tekens. - of - Bestandsnaam, als onderdeel van*name*, overschrijdt 100 symbolen. |
| UnauthorizedAccessException | Toegang tot dossier*sourcePath* wordt ontkend. |
| PathTooLongException | De opgegeven*sourcePath* , bestandsnaam of beide overschrijden de door het systeem gedefinieerde maximale lengte. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. - of -*name* is te lang voor shar. |
| NotSupportedException | Dossier bij*sourcePath* bevat een dubbele punt (:) in het midden van de tekenreeks. |

### Opmerkingen

De naam van het item wordt alleen binnen ingesteld*name* parameter. De bestandsnaam die is opgegeven in*sourcePath* parameter heeft geen invloed op de naam van het item.

Als het bestand direct wordt geopend met*openImmediately*parameter wordt het geblokkeerd totdat het archief is verwijderd.

### Voorbeelden

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### Zie ook

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* naamruimte [Aspose.Zip.Shar](../../shararchive/)
* montage [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Maak een enkel item binnen het archief.

```csharp
public SharEntry CreateEntry(string name, Stream source)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| source | Stream | De invoerstroom voor het item. |

### Winstwaarde

Shar entry-exemplaar.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *name* is niets. |
| ArgumentNullException | *source* is niets. |
| ArgumentException | *name* is leeg. |

### Voorbeelden

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.shar");
}
```

### Zie ook

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* naamruimte [Aspose.Zip.Shar](../../shararchive/)
* montage [Aspose.Zip](../../../)


