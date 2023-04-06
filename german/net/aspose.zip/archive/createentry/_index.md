---
title: Archive.CreateEntry
second_title: Aspose.ZIP für .NET-API-Referenz
description: Archive methode. Einzelner Eintrag im Archiv erstellen.
type: docs
weight: 50
url: /de/net/aspose.zip/archive/createentry/
---
## CreateEntry(string, string, bool, ArchiveEntrySettings) {#createentry_3}

Einzelner Eintrag im Archiv erstellen.

```csharp
public ArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| path | String | Der vollständig qualifizierte Name der neuen Datei oder der relative Dateiname, der komprimiert werden soll. |
| openImmediately | Boolean | Wahr, wenn die Datei sofort geöffnet wird, andernfalls die Datei beim Archivspeichern öffnen. |
| newEntrySettings | ArchiveEntrySettings | Komprimierungs- und Verschlüsselungseinstellungen für hinzugefügt[`ArchiveEntry`](../../archiveentry/) Artikel. |

### Rückgabewert

Zip-Eintragsinstanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *path* ist Null. |
| SecurityException | Der Anrufer verfügt nicht über die erforderliche Zugriffsberechtigung. |
| ArgumentException | Der*path* leer ist, nur Leerzeichen enthält oder ungültige Zeichen enthält. |
| UnauthorizedAccessException | Zugriff auf Datei*path* ist abgelehnt. |
| PathTooLongException | Die angegebene*path*, Dateiname oder beide überschreiten die vom System definierte maximale Länge. Beispielsweise müssen auf Windows-basierten Plattformen Pfade weniger als 248 Zeichen und Dateinamen weniger als 260 Zeichen umfassen. |
| NotSupportedException | Datei unter*path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenfolge. |

### Bemerkungen

Der Eintragsname wird ausschließlich innerhalb gesetzt*name* Parameter. Der Dateiname, der in bereitgestellt wird*path* Parameter wirkt sich nicht auf den Eintragsnamen aus.

Wird die Datei sofort mit geöffnet*openImmediately* Parameter wird es gesperrt, bis das Archiv gespeichert wird.

### Beispiele

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

### Siehe auch

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namensraum [Aspose.Zip](../../archive/)
* Montage [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings) {#createentry_1}

Einzelner Eintrag im Archiv erstellen.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| source | Stream | Der Eingabestream für den Eintrag. |
| newEntrySettings | ArchiveEntrySettings | Komprimierungs- und Verschlüsselungseinstellungen für hinzugefügt[`ArchiveEntry`](../../archiveentry/) Artikel. |

### Rückgabewert

Zip-Eintragsinstanz.

### Beispiele

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.zip");
}
```

### Siehe auch

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namensraum [Aspose.Zip](../../archive/)
* Montage [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool, ArchiveEntrySettings) {#createentry}

Einzelner Eintrag im Archiv erstellen.

```csharp
public ArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| fileInfo | FileInfo | Die Metadaten der zu komprimierenden Datei. |
| openImmediately | Boolean | Wahr, wenn die Datei sofort geöffnet wird, andernfalls die Datei beim Archivspeichern öffnen. |
| newEntrySettings | ArchiveEntrySettings | Komprimierungs- und Verschlüsselungseinstellungen für hinzugefügt[`ArchiveEntry`](../../archiveentry/) Artikel. |

### Rückgabewert

Zip-Eintragsinstanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* ist schreibgeschützt oder ein Verzeichnis. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig, da er sich beispielsweise auf einem nicht zugeordneten Laufwerk befindet. |
| IOException | Die Datei ist bereits geöffnet. |

### Bemerkungen

Der Eintragsname wird ausschließlich innerhalb gesetzt*name* Parameter. Der Dateiname, der in bereitgestellt wird*fileInfo* Parameter wirkt sich nicht auf den Eintragsnamen aus.

Wird die Datei sofort mit geöffnet*openImmediately* Parameter wird es gesperrt, bis das Archiv gespeichert wird.

### Beispiele

Erstellen Sie ein Archiv mit Einträgen, die mit jeweils unterschiedlichen Verschlüsselungsmethoden und Passwörtern verschlüsselt sind.

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

### Siehe auch

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namensraum [Aspose.Zip](../../archive/)
* Montage [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings, FileSystemInfo) {#createentry_2}

Einzelner Eintrag im Archiv erstellen.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, ArchiveEntrySettings newEntrySettings, 
    FileSystemInfo fileInfo)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| source | Stream | Der Eingabestream für den Eintrag. |
| newEntrySettings | ArchiveEntrySettings | Komprimierungs- und Verschlüsselungseinstellungen für hinzugefügt[`ArchiveEntry`](../../archiveentry/) Artikel. |
| fileInfo | FileSystemInfo | Die Metadaten der zu komprimierenden Datei oder des Ordners. |

### Rückgabewert

Zip-Eintragsinstanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| InvalidOperationException | Beide*source* Und*fileInfo* sind null oder*source*ist null und*fileInfo* steht für Verzeichnis. |

### Bemerkungen

Der Eintragsname wird ausschließlich innerhalb gesetzt*name* Parameter. Der Dateiname, der in bereitgestellt wird*fileInfo* Parameter wirkt sich nicht auf den Eintragsnamen aus.

*fileInfo* verweisen kannDirectoryInfo wenn der Eintrag Verzeichnis ist.

### Beispiele

Archiv mit verschlüsseltem Eintrag erstellen.

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

### Siehe auch

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namensraum [Aspose.Zip](../../archive/)
* Montage [Aspose.Zip](../../../)


