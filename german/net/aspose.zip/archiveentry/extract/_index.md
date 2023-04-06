---
title: ArchiveEntry.Extract
second_title: Aspose.ZIP für .NET-API-Referenz
description: ArchiveEntry methode. Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad.
type: docs
weight: 100
url: /de/net/aspose.zip/archiveentry/extract/
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
| InvalidDataException | CRC- oder MAC-Verifizierung für den Eintrag fehlgeschlagen. |

### Beispiele

Extrahieren Sie zwei Einträge des Zip-Archivs mit jeweils eigenem Passwort

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Open))
{
    using (Archive archive = new Archive(zipFile))
    {
        archive.Entries[0].Extract("first.bin", "first_pass");
        archive.Entries[1].Extract("second.bin", "second_pass");
    }
}
```

### Siehe auch

* class [ArchiveEntry](../)
* namensraum [Aspose.Zip](../../archiveentry/)
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
| InvalidDataException | CRC- oder MAC-Verifizierung für den Eintrag fehlgeschlagen. |
| ArgumentException | *destination* unterstützt das Schreiben nicht. |

### Beispiele

Extrahieren Sie einen Eintrag des Zip-Archivs mit Passwort.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Open))
{
    using (Archive archive = new Archive(zipFile))
    {
        archive.Entries[0].Extract(httpResponseStream, "p@s$");
    }
}
```

### Siehe auch

* class [ArchiveEntry](../)
* namensraum [Aspose.Zip](../../archiveentry/)
* Montage [Aspose.Zip](../../../)


