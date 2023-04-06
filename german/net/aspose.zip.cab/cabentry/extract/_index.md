---
title: CabEntry.Extract
second_title: Aspose.ZIP für .NET-API-Referenz
description: CabEntry methode. Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad.
type: docs
weight: 30
url: /de/net/aspose.zip.cab/cabentry/extract/
---
## Extract(string) {#extract}

Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | String | Der Pfad zur Zieldatei. Wenn die Datei bereits existiert, wird sie überschrieben. |

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

### Beispiele

```csharp
using (var archive = new CabArchive("archive.cab"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Siehe auch

* class [CabEntry](../)
* namensraum [Aspose.Zip.Cab](../../cabentry/)
* Montage [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extrahiert den Eintrag zum bereitgestellten Stream.

```csharp
public void Extract(Stream destination)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destination | Stream | Zielstrom. Muss beschreibbar sein. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | *destination* unterstützt das Schreiben nicht. |

### Beispiele

Extrahieren Sie einen Eintrag aus dem cab-Archiv.

```csharp
using (var archive = new CabArchive("archive.cab"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Siehe auch

* class [CabEntry](../)
* namensraum [Aspose.Zip.Cab](../../cabentry/)
* Montage [Aspose.Zip](../../../)


