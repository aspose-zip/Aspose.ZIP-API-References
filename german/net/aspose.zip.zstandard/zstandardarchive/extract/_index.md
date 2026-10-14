---
title: "ZstandardArchive.Extract"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "ZstandardArchive-Methode. Extrahiert das Archiv in den bereitgestellten Stream."
type: docs
weight: 30
url: /de/net/aspose.zip.zstandard/zstandardarchive/extract/
---
## Extract(Stream) {#extract_1}

Extrahiert das Archiv in den bereitgestellten Stream.

```csharp
public void Extract(Stream destination)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ziel | Stream | Ziel-Stream. Muss beschreibbar sein. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| ArgumentException | *destination* unterstützt das Schreiben nicht. |
| OperationCanceledException | In .NET Framework 4.0 und höher: Wird ausgelöst, wenn die Extraktion über das bereitgestellte Abbruch-Token abgebrochen wird. |

## Beispiele

```csharp
using (var archive = new GzipArchive("archive.zst"))
{
     archive.Extract(httpResponseStream);
}
```

### Siehe auch

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Extrahiert das Archiv in die Datei über den Pfad.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der Pfad zur Zieldatei. Wenn die Datei bereits existiert, wird sie überschrieben. |

### Rückgabewert

Informationen einer extrahierten Datei.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| ArgumentNullException | *path* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung zum Zugriff. |
| ArgumentException | Der *path* ist leer, enthält nur Leerzeichen oder ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf Datei *path* wurde verweigert. |
| PathTooLongException | Der angegebene *path*, Dateiname oder beides überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Datei bei *path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenkette. |
| OperationCanceledException | In .NET Framework 4.0 und höher: Wird ausgelöst, wenn die Extraktion über das bereitgestellte Abbruch-Token abgebrochen wird. |

### Siehe auch

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


