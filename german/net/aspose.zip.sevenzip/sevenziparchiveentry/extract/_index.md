---
title: SevenZipArchiveEntry.Extract
second_title: Aspose.ZIP für .NET-API-Referenz
description: SevenZipArchiveEntry methode. Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad.
type: docs
weight: 80
url: /de/net/aspose.zip.sevenzip/sevenziparchiveentry/extract/
---
## Extract(string, string) {#extract}

Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad.

```csharp
public FileInfo Extract(string path, string password = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | String | Der Pfad zur Zieldatei. Wenn die Datei bereits existiert, wird sie überschrieben. |
| password | String | Optionales Passwort für die Entschlüsselung. |

### Rückgabewert

Die Dateiinformationen der zusammengesetzten Datei.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *path* ist Null. |
| SecurityException | Der Anrufer verfügt nicht über die erforderliche Zugriffsberechtigung. |
| ArgumentException | Der*path* leer ist, nur Leerzeichen enthält oder ungültige Zeichen enthält. |
| UnauthorizedAccessException | Zugriff auf Datei*path* ist abgelehnt. |
| PathTooLongException | Die angegebene*path*, Dateiname oder beide überschreiten die vom System definierte maximale Länge. Beispielsweise müssen auf Windows-basierten Plattformen Pfade weniger als 248 Zeichen und Dateinamen weniger als 260 Zeichen umfassen. |
| NotSupportedException | Datei unter*path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenfolge. |

### Beispiele

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Siehe auch

* class [SevenZipArchiveEntry](../)
* namensraum [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* Montage [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Extrahiert den Eintrag zum bereitgestellten Stream.

```csharp
public void Extract(Stream destination, string password = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destination | Stream | Zielstrom. Muss beschreibbar sein. |
| password | String | Optionales Passwort für die Entschlüsselung. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | *destination* unterstützt das Schreiben nicht. |
| InvalidOperationException | Das Archiv wird nicht zum Entpacken geöffnet. - oder - Dieser Eintrag ist ein Verzeichnis. |
| InvalidDataException | Falsche Daten im Eintrag. |

### Beispiele

Extrahieren Sie einen Eintrag des Zip-Archivs mit Passwort.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Siehe auch

* class [SevenZipArchiveEntry](../)
* namensraum [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* Montage [Aspose.Zip](../../../)


