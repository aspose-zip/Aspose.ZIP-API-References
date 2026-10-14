---
title: "GetFormatInfo"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: 
type: docs
weight: 20
url: /de/net/aspose.zip.archiveinfo/archiveformatdetector/getformatinfo/
---
## ArchiveFormatDetector.GetFormatInfo method (1 of 2)

Ruft Formatinformationen ab.

```csharp
public ArchiveFormatInfo GetFormatInfo(string fileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Der Dateiname der Archivdatei. |

### Rückgabewert

Informationen zum Archivformat oder null, wenn das Format nicht erkannt wurde.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *fileName* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung zum Zugriff. |
| ArgumentException | Der *fileName* ist leer, enthält nur Leerzeichen oder enthält ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf die Datei *fileName* wurde verweigert. |
| PathTooLongException | Der angegebene *fileName* überschreitet die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows-basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Die Datei bei *fileName* enthält einen Doppelpunkt (:) in der Mitte der Zeichenkette. |
| IOException | Beim Öffnen der Datei ist ein I/O-Fehler aufgetreten. |

### Siehe auch

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

---

## ArchiveFormatDetector.GetFormatInfo method (2 of 2)

Ruft Formatinformationen ab.

```csharp
public ArchiveFormatInfo GetFormatInfo(Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Der Stream der Archivdatei. |

### Rückgabewert

Informationen zum Archivformat oder null, wenn das Format nicht erkannt wurde.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *stream* ist null. |
| ArgumentException | *stream* ist nicht suchbar. |

### Siehe auch

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

<!-- NICHT BEARBEITEN: erzeugt von xmldocmd für Aspose.Zip.dll -->
