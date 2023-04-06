---
title: SnappyArchive.Extract
second_title: Aspose.ZIP für .NET-API-Referenz
description: SnappyArchive methode. Extrahiert SnappyArchive in einen Stream.
type: docs
weight: 30
url: /de/net/aspose.zip.snappy/snappyarchive/extract/
---
## Extract(Stream) {#extract_2}

Extrahiert Snappy-Archive in einen Stream.

```csharp
public void Extract(Stream destination)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destination | Stream | Stream zum Speichern dekomprimierter Daten. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| InvalidOperationException | Archivheader und Serviceinformationen wurden nicht gelesen. |
| InvalidDataException | Datenfehler im Header oder in der Prüfsumme. |
| ArgumentNullException | Zielstream ist null. |
| ArgumentException | Der Zielstream unterstützt kein Schreiben. |

### Beispiele

```csharp
using (FileStream sourceSnappyFile = File.Open(sourceFileName, FileMode.Open))
{
   using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
   {
       using (var archive = new SnappyArchive(sourceSnappyFile))
       {
           archive.Extract(extractedFile);
       }
   }
}
```

### Siehe auch

* class [SnappyArchive](../)
* namensraum [Aspose.Zip.Snappy](../../snappyarchive/)
* Montage [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Extrahiert Snappy-Archive in eine Datei.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo zum Speichern dekomprimierter Daten. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| InvalidOperationException | Archivheader und Serviceinformationen wurden nicht gelesen. |
| SecurityException | Der Anrufer hat nicht die erforderliche Berechtigung zum Öffnen der*fileInfo*. |
| ArgumentException | Dateipfad ist leer oder enthält nur Leerzeichen. |
| FileNotFoundException | Die Datei wird nicht gefunden. |
| UnauthorizedAccessException | Pfad zur Datei ist schreibgeschützt oder ist ein Verzeichnis. |
| ArgumentNullException | *fileInfo* ist Null. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig, da er sich beispielsweise auf einem nicht zugeordneten Laufwerk befindet. |
| IOException | Die Datei ist bereits geöffnet. |

### Beispiele

```csharp
using (FileStream snappyFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new SnappyArchive(snappyFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### Siehe auch

* class [SnappyArchive](../)
* namensraum [Aspose.Zip.Snappy](../../snappyarchive/)
* Montage [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Extrahiert Snappy-Archive nach Pfad in eine Datei.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | String | Pfad zur Datei, in der dekomprimierte Daten gespeichert werden. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| InvalidOperationException | Archivheader und Serviceinformationen wurden nicht gelesen. |
| ArgumentNullException | *path* ist Null. |
| SecurityException | Der Anrufer verfügt nicht über die erforderliche Zugriffsberechtigung. |
| ArgumentException | Der*path* leer ist, nur Leerzeichen enthält oder ungültige Zeichen enthält. |
| UnauthorizedAccessException | Zugriff auf Datei*path* ist abgelehnt. |
| PathTooLongException | Die angegebene*path*, Dateiname oder beide überschreiten die vom System definierte maximale Länge. Beispielsweise müssen auf Windows-basierten Plattformen Pfade weniger als 248 Zeichen und Dateinamen weniger als 260 Zeichen umfassen. |
| NotSupportedException | Datei unter*path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenfolge. |

### Beispiele

```csharp
using (FileStream snappyFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new SnappyArchive(snappyFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### Siehe auch

* class [SnappyArchive](../)
* namensraum [Aspose.Zip.Snappy](../../snappyarchive/)
* Montage [Aspose.Zip](../../../)


