---
title: ArchiveInstanceInfo.GetArchiveFormatInfo
second_title: Aspose.ZIP für .NET-API-Referenz
description: ArchiveInstanceInfo methode. Ruft Informationen zum Archivformat ab.
type: docs
weight: 50
url: /de/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveformatinfo/
---
## GetArchiveFormatInfo(string) {#getarchiveformatinfo_1}

Ruft Informationen zum Archivformat ab.

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(string fileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Der Dateiname der Archivdatei. |

### Rückgabewert

Informationen über das Archivformat oder null, wenn das Format nicht erkannt wurde.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *fileName* ist Null. |
| SecurityException | Der Anrufer verfügt nicht über die erforderliche Zugriffsberechtigung. |
| ArgumentException | Der*fileName* leer ist, nur Leerzeichen enthält oder ungültige Zeichen enthält. |
| UnauthorizedAccessException | Zugriff auf Datei*fileName* ist abgelehnt. |
| PathTooLongException | Die angegebene*fileName* die systemdefinierte maximale Länge überschreitet. Beispielsweise müssen auf Windows-basierten Plattformen Pfade weniger als 248 Zeichen und Dateinamen weniger als 260 Zeichen umfassen. |
| NotSupportedException | Datei unter*fileName* enthält einen Doppelpunkt (:) in der Mitte der Zeichenfolge. |
| IOException | Beim Öffnen der Datei ist ein E/A-Fehler aufgetreten. |

### Siehe auch

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* namensraum [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* Montage [Aspose.Zip](../../../)

---

## GetArchiveFormatInfo(Stream) {#getarchiveformatinfo}

Ruft Informationen zum Archivformat ab.

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Der Stream der Archivdatei. |

### Rückgabewert

Informationen über das Archivformat oder null, wenn das Format nicht erkannt wurde.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *stream* ist Null. |
| ArgumentException | *stream* ist nicht auffindbar. |

### Siehe auch

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* namensraum [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* Montage [Aspose.Zip](../../../)


