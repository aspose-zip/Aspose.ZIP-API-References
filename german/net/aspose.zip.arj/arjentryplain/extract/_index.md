---
title: "ArjEntryPlain.Extract"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "ArjEntryPlain-Methode. Extrahiert den Eintrag in das Dateisystem anhand des angegebenen Pfads."
type: docs
weight: 40
url: /de/net/aspose.zip.arj/arjentryplain/extract/
---
## Extract(string) {#extract}

Extrahiert den Eintrag in das Dateisystem anhand des angegebenen Pfads.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der Pfad zur Zieldatei. Wenn die Datei bereits existiert, wird sie überschrieben. |

### Rückgabewert

Die Dateiinformation einer zusammengesetzten Datei.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *path* ist null oder leer. |
| ObjectDisposedException | Wird ausgelöst, wenn das Archiv freigegeben wurde. |
| FileNotFoundException | Die Datei wurde nicht gefunden. |
| InvalidDataException | Prüfsummen‑Fehler für Header oder Daten. – oder – Das Archiv ist beschädigt. |
| PathTooLongException | Der angegebene Pfad, Dateiname oder beides überschreitet die systemdefinierte maximale Länge. |
| NotImplementedException | Eintrag komprimiert mit Methode 4. |

## Beispiele

Extrahiere zwei Einträge aus einem RAR-Archiv.

```csharp
using (FileStream arjFile = File.Open("archive.arj", FileMode.Open))
{
    using (ArjArchive archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract("first.bin");
        archive.Entries[1].Extract("second.bin");
    }
}
```

### Siehe auch

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Extrahiert einen ARJ‑Archiveintrag in eine Datei.

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
| ObjectDisposedException | Wird ausgelöst, wenn das Archiv freigegeben wurde. |
| InvalidDataException | Prüfsummen‑Fehler für Header oder Daten. – oder – Das Archiv ist beschädigt. |
| NotImplementedException | Eintrag komprimiert mit Methode 4. |

## Beispiele

```csharp
using (var arjFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### Siehe auch

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
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
| InvalidDataException | Prüfsummen‑Fehler für Header oder Daten. – oder – Das Archiv ist beschädigt. |
| NotImplementedException | Eintrag komprimiert mit Methode 4. |
| OperationCanceledException | In .NET Framework 4.0 und höher: Wird ausgelöst, wenn die Extraktion über das bereitgestellte Abbruch-Token abgebrochen wird. |
| ObjectDisposedException | Wird ausgelöst, wenn das Archiv freigegeben wurde. |

### Siehe auch

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)


