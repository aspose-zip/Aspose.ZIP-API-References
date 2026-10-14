---
title: "LhaArchiveEntry.Extract"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "LhaArchiveEntry-Methode. Extrahiert den Lha-Archiveintrag in ein Dateisystem anhand des Pfads"
type: docs
weight: 60
url: /de/net/aspose.zip.lha/lhaarchiveentry/extract/
---
## Extract(string) {#extract}

Extrahiert Lha-Archiveintrag in ein Dateisystem nach Pfad.

```csharp
public FileSystemInfo Extract(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Pfad zu der Datei, die die dekomprimierten Daten speichert. |

### Rückgabewert

FileSystemInfoInstance, das extrahierte Daten enthält.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| InvalidOperationException | Archivköpfe und Serviceinformationen wurden nicht gelesen. |
| ArgumentNullException | *path* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung zum Zugriff. |
| ArgumentException | Der *path* ist leer, enthält nur Leerzeichen oder ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf Datei *path* wurde verweigert. |
| PathTooLongException | Der angegebene *path*, Dateiname oder beides überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Datei bei *path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenkette. |
| OperationCanceledException | In .NET Framework 4.0 und höher: Wird ausgelöst, wenn die Extraktion über das bereitgestellte Abbruch-Token abgebrochen wird. |
| ObjectDisposedException | Wird ausgelöst, wenn der Quellstream freigegeben wurde. |
| InvalidDataException | Wird ausgelöst, wenn die Daten ungültig oder beschädigt sind. |

## Beispiele

```csharp
using (FileStream lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### Siehe auch

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_2}

Extrahiert den Eintrag in den bereitgestellten Stream.

```csharp
public void Extract(Stream destination)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ziel | Stream | Ziel-Stream. Muss beschreibbar sein. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | *destination* unterstützt das Schreiben nicht. |
| OperationCanceledException | In .NET Framework 4.0 und höher: Wird ausgelöst, wenn die Extraktion über das bereitgestellte Abbruch-Token abgebrochen wird. |
| ObjectDisposedException | Wird ausgelöst, wenn der Quellstream freigegeben wurde. |
| InvalidDataException | Wird ausgelöst, wenn die Daten ungültig oder beschädigt sind. |

## Hinweise

Tut nichts für Verzeichniseintrag.

### Siehe auch

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Extrahiert Lha-Archiveintrag in eine Datei.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo zum Speichern entkomprimierter Daten. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| InvalidOperationException | Archivköpfe und Serviceinformationen wurden nicht gelesen. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung, um *fileInfo* zu öffnen. |
| ArgumentException | Der Dateipfad ist leer oder enthält nur Leerzeichen. |
| FileNotFoundException | Die Datei wurde nicht gefunden. |
| UnauthorizedAccessException | Der Pfad zur Datei ist schreibgeschützt oder ein Verzeichnis. |
| ArgumentNullException | *fileInfo* ist null. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig, z. B. weil er sich auf einem nicht zugeordneten Laufwerk befindet. |
| IOException | Die Datei ist bereits geöffnet. |
| OperationCanceledException | In .NET Framework 4.0 und höher: Wird ausgelöst, wenn die Extraktion über das bereitgestellte Abbruch-Token abgebrochen wird. |
| ObjectDisposedException | Wird ausgelöst, wenn der Quellstream freigegeben wurde. |

## Hinweise

Tut nichts für Verzeichniseintrag.

## Beispiele

```csharp
using (var lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### Siehe auch

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)


