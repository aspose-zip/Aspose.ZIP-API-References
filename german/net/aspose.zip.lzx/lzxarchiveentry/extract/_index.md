---
title: "LzxArchiveEntry.Extract"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "LzxArchiveEntry-Methode. Extrahiert den Lzx-Archiveintrag in ein Dateisystem nach Pfad"
type: docs
weight: 80
url: /de/net/aspose.zip.lzx/lzxarchiveentry/extract/
---
## Extract(string) {#extract}

Extrahiert den Lzx-Archiveintrag in ein Dateisystem anhand des Pfads.

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
| InvalidDataException | Prüfsummen‑Fehler für Header oder Daten. – oder – Das Archiv ist beschädigt. |
| OperationCanceledException | In .NET Framework 4.0 und höher: Wird ausgelöst, wenn die Extraktion über das bereitgestellte Abbruch-Token abgebrochen wird. |
| NotSupportedException | Ungültige Komprimierungsmethode. |
| ObjectDisposedException | Wird ausgelöst, wenn der Quellstream freigegeben wurde. |
| EndOfStreamException | Wird ausgelöst, wenn das Ende des Streams unerwartet erreicht wird. |

## Beispiele

```csharp
using (FileStream lzxFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzxArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### Siehe auch

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

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
| ArgumentNullException | Ziel-Stream ist null. |
| NotSupportedException | Ungültige Komprimierungsmethode. |
| OperationCanceledException | In .NET Framework 4.0 und höher: Wird ausgelöst, wenn die Extraktion über das bereitgestellte Abbruch-Token abgebrochen wird. |
| ObjectDisposedException | Wird ausgelöst, wenn der Quellstream freigegeben wurde. |
| EndOfStreamException | Wird ausgelöst, wenn das Ende des Streams unerwartet erreicht wird. |

### Siehe auch

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)


