---
title: Archive.CreateEntry
second_title: Aspose.ZIP voor .NET API-referentie
description: Archive methode. Maak een enkel item binnen het archief.
type: docs
weight: 50
url: /nl/net/aspose.zip/archive/createentry/
---
## CreateEntry(string, string, bool, ArchiveEntrySettings) {#createentry_3}

Maak een enkel item binnen het archief.

```csharp
public ArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| path | String | De volledig gekwalificeerde naam van het nieuwe bestand, of de relatieve bestandsnaam die moet worden gecomprimeerd. |
| openImmediately | Boolean | Waar als het bestand onmiddellijk wordt geopend, anders opent u het bestand bij opslaan in het archief. |
| newEntrySettings | ArchiveEntrySettings | Compressie- en coderingsinstellingen gebruikt voor toegevoegd[`ArchiveEntry`](../../archiveentry/) item. |

### Winstwaarde

Zip-invoerinstantie.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *path* is niets. |
| SecurityException | De beller heeft niet de vereiste toegangsrechten. |
| ArgumentException | De*path* is leeg, bevat alleen spaties of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot dossier*path* wordt ontkend. |
| PathTooLongException | De opgegeven*path*, bestandsnaam of beide overschrijden de door het systeem gedefinieerde maximale lengte. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. |
| NotSupportedException | Dossier bij*path* bevat een dubbele punt (:) in het midden van de tekenreeks. |

### Opmerkingen

De naam van het item wordt alleen binnen ingesteld*name* parameter. De bestandsnaam die is opgegeven in*path* parameter heeft geen invloed op de naam van het item.

Als het bestand direct wordt geopend met*openImmediately* parameter wordt het geblokkeerd totdat het archief is opgeslagen.

### Voorbeelden

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### Zie ook

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* naamruimte [Aspose.Zip](../../archive/)
* montage [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings) {#createentry_1}

Maak een enkel item binnen het archief.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| source | Stream | De invoerstroom voor het item. |
| newEntrySettings | ArchiveEntrySettings | Compressie- en coderingsinstellingen gebruikt voor toegevoegd[`ArchiveEntry`](../../archiveentry/) item. |

### Winstwaarde

Zip-invoerinstantie.

### Voorbeelden

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.zip");
}
```

### Zie ook

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* naamruimte [Aspose.Zip](../../archive/)
* montage [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool, ArchiveEntrySettings) {#createentry}

Maak een enkel item binnen het archief.

```csharp
public ArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| fileInfo | FileInfo | De metadata van het te comprimeren bestand. |
| openImmediately | Boolean | Waar als het bestand onmiddellijk wordt geopend, anders opent u het bestand bij opslaan in het archief. |
| newEntrySettings | ArchiveEntrySettings | Compressie- en coderingsinstellingen gebruikt voor toegevoegd[`ArchiveEntry`](../../archiveentry/) item. |

### Winstwaarde

Zip-invoerinstantie.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* is alleen-lezen of is een map. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, omdat het zich bijvoorbeeld op een niet-toegewezen schijf bevindt. |
| IOException | Het bestand is al geopend. |

### Opmerkingen

De naam van het item wordt alleen binnen ingesteld*name* parameter. De bestandsnaam die is opgegeven in*fileInfo* parameter heeft geen invloed op de naam van het item.

Als het bestand direct wordt geopend met*openImmediately* parameter wordt het geblokkeerd totdat het archief is opgeslagen.

### Voorbeelden

Stel een archief samen met vermeldingen die elk zijn versleuteld met verschillende coderingsmethoden en wachtwoorden.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
        archive.CreateEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass2", EncryptionMethod.AES128)));
        archive.CreateEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass3", EncryptionMethod.AES256)));
        archive.Save(zipFile);
    }
}
```

### Zie ook

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* naamruimte [Aspose.Zip](../../archive/)
* montage [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings, FileSystemInfo) {#createentry_2}

Maak een enkel item binnen het archief.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, ArchiveEntrySettings newEntrySettings, 
    FileSystemInfo fileInfo)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| source | Stream | De invoerstroom voor het item. |
| newEntrySettings | ArchiveEntrySettings | Compressie- en coderingsinstellingen gebruikt voor toegevoegd[`ArchiveEntry`](../../archiveentry/) item. |
| fileInfo | FileSystemInfo | De metadata van het bestand of de map die moet worden gecomprimeerd. |

### Winstwaarde

Zip-invoerinstantie.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| InvalidOperationException | Beide*source* En*fileInfo* zijn nul of*source*is nul en*fileInfo* staat voor map. |

### Opmerkingen

De naam van het item wordt alleen binnen ingesteld*name* parameter. De bestandsnaam die is opgegeven in*fileInfo* parameter heeft geen invloed op de naam van het item.

*fileInfo* kan verwijzen naarDirectoryInfo als de vermelding directory is.

### Voorbeelden

Archief samenstellen met gecodeerde invoer.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF} ), new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")), new FileInfo("data1.bin")); 
        archive.Save(zipFile);
    }
}
```

### Zie ook

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* naamruimte [Aspose.Zip](../../archive/)
* montage [Aspose.Zip](../../../)


