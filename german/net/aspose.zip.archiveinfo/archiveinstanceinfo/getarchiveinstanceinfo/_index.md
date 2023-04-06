---
title: ArchiveInstanceInfo.GetArchiveInstanceInfo
second_title: Aspose.ZIP für .NET-API-Referenz
description: ArchiveInstanceInfo methode. Ruft Archivinstanzinformationen ab.
type: docs
weight: 10
url: /de/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveinstanceinfo/
---
## GetArchiveInstanceInfo(string) {#getarchiveinstanceinfo_1}

Ruft Archivinstanzinformationen ab.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(string fileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Der Dateiname der Archivdatei. |

### Rückgabewert

Informationen zur Archivinstanz oder null, wenn das Format nicht erkannt wurde.

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

* class [ArchiveInstanceInfo](../)
* namensraum [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* Montage [Aspose.Zip](../../../)

---

## GetArchiveInstanceInfo(Stream) {#getarchiveinstanceinfo}

Ruft Archivinstanzinformationen ab.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Der Stream der Archivdatei. |

### Rückgabewert

Informationen zur Archivinstanz oder null, wenn das Format nicht erkannt wurde.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *stream* ist Null. |
| ArgumentException | *stream* ist nicht auffindbar. |

### Siehe auch

* class [ArchiveInstanceInfo](../)
* namensraum [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* Montage [Aspose.Zip](../../../)


