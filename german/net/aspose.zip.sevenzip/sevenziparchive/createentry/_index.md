---
title: CreateEntry
second_title: Aspose.ZIP für .NET-API-Referenz
description: Einzelner Eintrag im Archiv erstellen.
type: docs
weight: 50
url: /de/net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## CreateEntry(string, FileInfo, bool, SevenZipEntrySettings) {#createentry}

Einzelner Eintrag im Archiv erstellen.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| fileInfo | FileInfo | Die Metadaten der zu komprimierenden Datei. |
| openImmediately | Boolean | Wahr, wenn die Datei sofort geöffnet wird, andernfalls die Datei beim Archivspeichern öffnen. |
| newEntrySettings | SevenZipEntrySettings | Komprimierungs- und Verschlüsselungseinstellungen für hinzugefügt[`SevenZipArchiveEntry`](../../sevenziparchiveentry) Artikel. |

### Rückgabewert

Instanz mit sieben Zip-Einträgen.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* ist schreibgeschützt oder ein Verzeichnis. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig, da er sich beispielsweise auf einem nicht zugeordneten Laufwerk befindet. |
| IOException | Die Datei ist bereits geöffnet. |

### Bemerkungen

Der Eintragsname wird ausschließlich innerhalb festgelegt*name* Parameter. Der Dateiname, der in bereitgestellt wird*fileInfo* Parameter wirkt sich nicht auf den Eintragsnamen aus.

Wird die Datei sofort mit geöffnet*openImmediately* Parameter wird es gesperrt, bis das Archiv gespeichert wird.

### Beispiele

Erstellen Sie ein Archiv mit Einträgen, die mit jeweils unterschiedlichen Passwörtern verschlüsselt sind.

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

### Siehe auch

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* namensraum [Aspose.Zip.SevenZip](../../sevenziparchive)
* Montage [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings, FileSystemInfo) {#createentry_2}

Einzelner Eintrag im Archiv erstellen.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| source | Stream | Der Eingabestream für den Eintrag. |
| newEntrySettings | SevenZipEntrySettings | Komprimierungs- und Verschlüsselungseinstellungen für hinzugefügt[`SevenZipArchiveEntry`](../../sevenziparchiveentry) Artikel. |
| fileInfo | FileSystemInfo | Die Metadaten der zu komprimierenden Datei oder des Ordners. |

### Rückgabewert

SevenZip-Eintragsinstanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| InvalidOperationException | Beide*source* und*fileInfo* sind null oder*source* ist null und*fileInfo* steht für Verzeichnis. |

### Bemerkungen

Der Eintragsname wird ausschließlich innerhalb festgelegt*name* Parameter. Der Dateiname, der in bereitgestellt wird*fileInfo* Parameter wirkt sich nicht auf den Eintragsnamen aus.

*fileInfo* verweisen kannDirectoryInfo wenn der Eintrag Verzeichnis ist.

### Beispiele

Archiv mit LZMA2-komprimiertem verschlüsseltem Eintrag erstellen.

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

### Siehe auch

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* namensraum [Aspose.Zip.SevenZip](../../sevenziparchive)
* Montage [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings) {#createentry_1}

Einzelner Eintrag im Archiv erstellen.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| source | Stream | Der Eingabestream für den Eintrag. |
| newEntrySettings | SevenZipEntrySettings | Komprimierungs- und Verschlüsselungseinstellungen für hinzugefügt[`SevenZipArchiveEntry`](../../sevenziparchiveentry) Artikel. |

### Rückgabewert

Zip-Eintragsinstanz.

### Beispiele

Erstellen Sie ein 7z-Archiv mit LZMA2-Komprimierung und Verschlüsselung aller Einträge.

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.7z");
}
```

### Siehe auch

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* namensraum [Aspose.Zip.SevenZip](../../sevenziparchive)
* Montage [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, SevenZipEntrySettings) {#createentry_3}

Einzelner Eintrag im Archiv erstellen.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| path | String | Der vollständig qualifizierte Name der neuen Datei oder der relative Dateiname, der komprimiert werden soll. |
| openImmediately | Boolean | Wahr, wenn die Datei sofort geöffnet wird, andernfalls die Datei beim Archivspeichern öffnen. |
| newEntrySettings | SevenZipEntrySettings | Komprimierungs- und Verschlüsselungseinstellungen für hinzugefügt[`SevenZipArchiveEntry`](../../sevenziparchiveentry) Artikel. |

### Rückgabewert

Zip-Eintragsinstanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *path* ist Null. |
| SecurityException | Der Anrufer verfügt nicht über die erforderliche Zugriffsberechtigung |
| ArgumentException | Das*path* leer ist, nur Leerzeichen enthält oder ungültige Zeichen enthält. |
| UnauthorizedAccessException | Zugriff auf Datei*path* ist abgelehnt. |
| PathTooLongException | Die angegebene*path*, Dateiname oder beide überschreiten die vom System definierte maximale Länge. Beispielsweise müssen auf Windows-basierten Plattformen Pfade weniger als 248 Zeichen und Dateinamen weniger als 260 Zeichen umfassen. |
| NotSupportedException | Datei unter*path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenfolge. |

### Bemerkungen

Der Eintragsname wird ausschließlich innerhalb festgelegt*name* Parameter. Der Dateiname, der in bereitgestellt wird*path* Parameter wirkt sich nicht auf den Eintragsnamen aus.

Wird die Datei sofort mit geöffnet*openImmediately* Parameter wird es gesperrt, bis das Archiv gespeichert wird.

### Beispiele

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

### Siehe auch

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* namensraum [Aspose.Zip.SevenZip](../../sevenziparchive)
* Montage [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
