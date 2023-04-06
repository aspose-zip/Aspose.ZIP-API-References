---
title: SevenZipArchive.CreateEntry
second_title: Aspose.ZIP voor .NET API-referentie
description: SevenZipArchive methode. Maak een enkel item binnen het archief.
type: docs
weight: 50
url: /nl/net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## CreateEntry(string, FileInfo, bool, SevenZipEntrySettings) {#createentry}

Maak een enkel item binnen het archief.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| fileInfo | FileInfo | De metadata van het te comprimeren bestand. |
| openImmediately | Boolean | Waar als het bestand onmiddellijk wordt geopend, anders opent u het bestand bij opslaan in het archief. |
| newEntrySettings | SevenZipEntrySettings | Compressie- en coderingsinstellingen gebruikt voor toegevoegd[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) item. |

### Winstwaarde

Seven Zip entry-exemplaar.

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

Stel een archief samen met vermeldingen die elk zijn versleuteld met verschillende wachtwoorden.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
        archive.CreateEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
        archive.CreateEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
        archive.Save(sevenZipFile);
    }
}
```

### Zie ook

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* naamruimte [Aspose.Zip.SevenZip](../../sevenziparchive/)
* montage [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings, FileSystemInfo) {#createentry_2}

Maak een enkel item binnen het archief.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| source | Stream | De invoerstroom voor het item. |
| newEntrySettings | SevenZipEntrySettings | Compressie- en coderingsinstellingen gebruikt voor toegevoegd[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) item. |
| fileInfo | FileSystemInfo | De metadata van het bestand of de map die moet worden gecomprimeerd. |

### Winstwaarde

SevenZip entry-instantie.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| InvalidOperationException | Beide*source* En*fileInfo* zijn nul of*source*is nul en*fileInfo* staat voor map. |

### Opmerkingen

De naam van het item wordt alleen binnen ingesteld*name* parameter. De bestandsnaam die is opgegeven in*fileInfo* parameter heeft geen invloed op de naam van het item.

*fileInfo* kan verwijzen naarDirectoryInfo als de vermelding directory is.

### Voorbeelden

Archief samenstellen met LZMA2 gecomprimeerde gecodeerde invoer.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF}), new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1")), new FileInfo("data1.bin")); 
        archive.Save(sevenZipFile);
    }
}
```

### Zie ook

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* naamruimte [Aspose.Zip.SevenZip](../../sevenziparchive/)
* montage [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings) {#createentry_1}

Maak een enkel item binnen het archief.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| source | Stream | De invoerstroom voor het item. |
| newEntrySettings | SevenZipEntrySettings | Compressie- en coderingsinstellingen gebruikt voor toegevoegd[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) item. |

### Winstwaarde

Zip-invoerinstantie.

### Voorbeelden

Stel 7z-archief samen met LZMA2-compressie en codering van alle items.

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.7z");
}
```

### Zie ook

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* naamruimte [Aspose.Zip.SevenZip](../../sevenziparchive/)
* montage [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, SevenZipEntrySettings) {#createentry_3}

Maak een enkel item binnen het archief.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| path | String | De volledig gekwalificeerde naam van het nieuwe bestand, of de relatieve bestandsnaam die moet worden gecomprimeerd. |
| openImmediately | Boolean | Waar als het bestand onmiddellijk wordt geopend, anders opent u het bestand bij opslaan in het archief. |
| newEntrySettings | SevenZipEntrySettings | Compressie- en coderingsinstellingen gebruikt voor toegevoegd[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) item. |

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
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings())))
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### Zie ook

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* naamruimte [Aspose.Zip.SevenZip](../../sevenziparchive/)
* montage [Aspose.Zip](../../../)


