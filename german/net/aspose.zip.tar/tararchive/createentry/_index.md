---
title: CreateEntry
second_title: Aspose.ZIP für .NET-API-Referenz
description: Einzelner Eintrag im Archiv erstellen.
type: docs
weight: 80
url: /de/net/aspose.zip.tar/tararchive/createentry/
---
## CreateEntry(string, Stream, FileSystemInfo) {#createentry_1}

Einzelner Eintrag im Archiv erstellen.

```csharp
public TarEntry CreateEntry(string name, Stream source, FileSystemInfo fileInfo = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| source | Stream | Der Eingabestream für den Eintrag. |
| fileInfo | FileSystemInfo | Die Metadaten der zu komprimierenden Datei oder des Ordners. |

### Rückgabewert

Tar-Eintragsinstanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| PathTooLongException | *name* ist nach IEEE 1003.1-1998-Standard zu lang für tar. |
| ArgumentException | Dateiname, als Teil von*name*, überschreitet 100 Symbole. |

### Bemerkungen

Der Eintragsname wird ausschließlich innerhalb festgelegt*name* Parameter. Der Dateiname, der in bereitgestellt wird*fileInfo* Parameter wirkt sich nicht auf den Eintragsnamen aus.

*fileInfo* verweisen kannDirectoryInfo wenn der Eintrag Verzeichnis ist.

### Beispiele

```csharp
using (var archive = new TarArchive())
{
   archive.CreateEntry("bytes", new MemoryStream(new byte[] {0x00, 0xFF}));
   archive.Save(tarFile);
}
```

### Siehe auch

* class [TarEntry](../../tarentry)
* class [TarArchive](../../tararchive)
* namensraum [Aspose.Zip.Tar](../../tararchive)
* Montage [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Einzelner Eintrag im Archiv erstellen.

```csharp
public TarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| fileInfo | FileInfo | Die Metadaten der zu komprimierenden Datei oder des Ordners. |
| openImmediately | Boolean | Wahr, wenn die Datei sofort geöffnet wird, andernfalls die Datei beim Archivspeichern öffnen. |

### Rückgabewert

Tar-Eintragsinstanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| PathTooLongException | *name* ist nach IEEE 1003.1-1998-Standard zu lang für tar. |
| ArgumentException | Dateiname, als Teil von*name*, überschreitet 100 Symbole. |

### Bemerkungen

Der Eintragsname wird ausschließlich innerhalb festgelegt*name* Parameter. Der Dateiname, der in bereitgestellt wird*fileInfo* Parameter wirkt sich nicht auf den Eintragsnamen aus.

*fileInfo* verweisen kannDirectoryInfo wenn der Eintrag Verzeichnis ist.

Wird die Datei sofort mit geöffnet*openImmediately* Parameter wird es blockiert, bis das Archiv entsorgt wird.

### Beispiele

```csharp
FileInfo fi = new FileInfo("data.bin");
using (var archive = new TarArchive())
{
   archive.CreateEntry("data.bin", fi);
   archive.Save(tarFile);
}
```

### Siehe auch

* class [TarEntry](../../tarentry)
* class [TarArchive](../../tararchive)
* namensraum [Aspose.Zip.Tar](../../tararchive)
* Montage [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Einzelner Eintrag im Archiv erstellen.

```csharp
public TarEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Der Name des Eintrags. |
| path | String | Pfad zur zu komprimierenden Datei. |
| openImmediately | Boolean | Wahr, wenn die Datei sofort geöffnet wird, andernfalls die Datei beim Archivspeichern öffnen. |

### Rückgabewert

Tar-Eintragsinstanz.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *path* ist Null. |
| SecurityException | Der Anrufer verfügt nicht über die erforderliche Zugriffsberechtigung |
| ArgumentException | Das*path* leer ist, nur Leerzeichen enthält oder ungültige Zeichen enthält. - oder - Dateiname, als Teil von*name*, überschreitet 100 Symbole. |
| UnauthorizedAccessException | Zugriff auf Datei*path* ist abgelehnt. |
| PathTooLongException | Die angegebene*path* , Dateiname oder beide überschreiten die vom System definierte maximale Länge. Beispielsweise müssen auf Windows-basierten Plattformen Pfade weniger als 248 Zeichen und Dateinamen weniger als 260 Zeichen umfassen. - oder -*name* ist nach IEEE 1003.1-1998-Standard zu lang für tar. |
| NotSupportedException | Datei unter*path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenfolge. |

### Bemerkungen

Der Eintragsname wird ausschließlich innerhalb festgelegt*name* Parameter. Der Dateiname, der in bereitgestellt wird*path* Parameter wirkt sich nicht auf den Eintragsnamen aus.

Wird die Datei sofort mit geöffnet*openImmediately* Parameter wird es blockiert, bis das Archiv entsorgt wird.

### Beispiele

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save(outputTarFile);
}
```

### Siehe auch

* class [TarEntry](../../tarentry)
* class [TarArchive](../../tararchive)
* namensraum [Aspose.Zip.Tar](../../tararchive)
* Montage [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
