---
title: "AlzEntry.Extract"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "AlzEntry method. Extrahiert den Eintrag in das Dateisystem anhand des angegebenen Pfads."
type: docs
weight: 60
url: /de/net/aspose.zip.alz/alzentry/extract/
---
## Extract(string, string) {#extract}

Extrahiert den Eintrag in das Dateisystem anhand des angegebenen Pfads.

```csharp
public FileInfo Extract(string path, string password = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der Pfad zur Zieldatei. Wenn die Datei bereits existiert, wird sie überschrieben. |
| Passwort | String | Optionales Passwort für die Entschlüsselung. |

### Rückgabewert

Die Dateiinformation einer zusammengesetzten Datei.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *path* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung zum Zugriff. |
| ArgumentException | Der *path* ist leer, enthält nur Leerzeichen oder ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf Datei *path* wurde verweigert. |
| PathTooLongException | Der angegebene *path*, Dateiname oder beides überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Datei bei *path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenkette. |
| InvalidDataException | Das Archiv ist beschädigt. |
| OperationCanceledException | In .NET Framework 4.0 und höher: Wird ausgelöst, wenn die Extraktion über das bereitgestellte Abbruch-Token abgebrochen wird. |
| ObjectDisposedException | Wird ausgelöst, wenn der Quellstream freigegeben wurde. |
| FileNotFoundException | Die Datei wurde nicht gefunden. |

## Beispiele

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Siehe auch

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Extrahiert den Eintrag in den bereitgestellten Stream.

```csharp
public void Extract(Stream destination, string password = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ziel | Stream | Ziel-Stream. Muss beschreibbar sein. |
| Passwort | String | Optionales Passwort für die Entschlüsselung. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | *destination* unterstützt das Schreiben nicht. |
| InvalidOperationException | Das Archiv ist nicht für die Extraktion geöffnet. - oder - Dieser Eintrag ist ein Verzeichnis. |
| InvalidDataException | Falsche Daten im Eintrag. |
| OperationCanceledException | In .NET Framework 4.0 und höher: Wird ausgelöst, wenn die Extraktion über das bereitgestellte Abbruch-Token abgebrochen wird. |

## Beispiele

Extrahiere einen Eintrag aus dem ALZ-Archiv mit Passwort.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Siehe auch

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)


