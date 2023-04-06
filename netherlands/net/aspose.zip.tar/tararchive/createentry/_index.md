---
title: TarArchive.CreateEntry
second_title: Aspose.ZIP voor .NET API-referentie
description: TarArchive methode. Maak een enkel item binnen het archief.
type: docs
weight: 80
url: /nl/net/aspose.zip.tar/tararchive/createentry/
---
## CreateEntry(string, Stream, FileSystemInfo) {#createentry_1}

Maak een enkel item binnen het archief.

```csharp
public TarEntry CreateEntry(string name, Stream source, FileSystemInfo fileInfo = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| source | Stream | De invoerstroom voor het item. |
| fileInfo | FileSystemInfo | De metadata van het bestand of de map die moet worden gecomprimeerd. |

### Winstwaarde

Tar ingangsinstantie.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| PathTooLongException | *name* is te lang voor tar vanaf de IEEE 1003.1-1998-standaard. |
| ArgumentException | Bestandsnaam, als onderdeel van*name*, overschrijdt 100 symbolen. |

### Opmerkingen

De naam van het item wordt alleen binnen ingesteld*name* parameter. De bestandsnaam die is opgegeven in*fileInfo* parameter heeft geen invloed op de naam van het item.

*fileInfo* kan verwijzen naarDirectoryInfo als de vermelding directory is.

### Voorbeelden

```csharp
using (var archive = new TarArchive())
{
   archive.CreateEntry("bytes", new MemoryStream(new byte[] {0x00, 0xFF}));
   archive.Save(tarFile);
}
```

### Zie ook

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* naamruimte [Aspose.Zip.Tar](../../tararchive/)
* montage [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Maak een enkel item binnen het archief.

```csharp
public TarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| fileInfo | FileInfo | De metadata van het bestand of de map die moet worden gecomprimeerd. |
| openImmediately | Boolean | Waar als het bestand onmiddellijk wordt geopend, anders opent u het bestand bij opslaan in het archief. |

### Winstwaarde

Tar ingangsinstantie.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| PathTooLongException | *name* is te lang voor tar vanaf de IEEE 1003.1-1998-standaard. |
| ArgumentException | Bestandsnaam, als onderdeel van*name*, overschrijdt 100 symbolen. |

### Opmerkingen

De naam van het item wordt alleen binnen ingesteld*name* parameter. De bestandsnaam die is opgegeven in*fileInfo* parameter heeft geen invloed op de naam van het item.

*fileInfo* kan verwijzen naarDirectoryInfo als de vermelding directory is.

Als het bestand direct wordt geopend met*openImmediately*parameter wordt het geblokkeerd totdat het archief is verwijderd.

### Voorbeelden

```csharp
FileInfo fi = new FileInfo("data.bin");
using (var archive = new TarArchive())
{
   archive.CreateEntry("data.bin", fi);
   archive.Save(tarFile);
}
```

### Zie ook

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* naamruimte [Aspose.Zip.Tar](../../tararchive/)
* montage [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Maak een enkel item binnen het archief.

```csharp
public TarEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| path | String | Pad naar te comprimeren bestand. |
| openImmediately | Boolean | Waar als het bestand onmiddellijk wordt geopend, anders opent u het bestand bij opslaan in het archief. |

### Winstwaarde

Tar ingangsinstantie.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *path* is niets. |
| SecurityException | De beller heeft niet de vereiste toegangsrechten. |
| ArgumentException | De*path* is leeg, bevat alleen spaties of bevat ongeldige tekens. - of - Bestandsnaam, als onderdeel van*name*, overschrijdt 100 symbolen. |
| UnauthorizedAccessException | Toegang tot dossier*path* wordt ontkend. |
| PathTooLongException | De opgegeven*path* , bestandsnaam of beide overschrijden de door het systeem gedefinieerde maximale lengte. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. - of -*name* is te lang voor tar vanaf de IEEE 1003.1-1998-standaard. |
| NotSupportedException | Dossier bij*path* bevat een dubbele punt (:) in het midden van de tekenreeks. |

### Opmerkingen

De naam van het item wordt alleen binnen ingesteld*name* parameter. De bestandsnaam die is opgegeven in*path* parameter heeft geen invloed op de naam van het item.

Als het bestand direct wordt geopend met*openImmediately*parameter wordt het geblokkeerd totdat het archief is verwijderd.

### Voorbeelden

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save(outputTarFile);
}
```

### Zie ook

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* naamruimte [Aspose.Zip.Tar](../../tararchive/)
* montage [Aspose.Zip](../../../)


