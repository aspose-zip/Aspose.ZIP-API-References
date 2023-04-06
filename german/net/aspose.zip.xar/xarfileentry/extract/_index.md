---
title: XarFileEntry.Extract
second_title: Aspose.ZIP für .NET-API-Referenz
description: XarFileEntry methode. Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad.
type: docs
weight: 20
url: /de/net/aspose.zip.xar/xarfileentry/extract/
---
## Extract(string) {#extract}

Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad.

```csharp
public abstract FileInfo Extract(string path)
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
using (var archive = new XarArchive("archive.xar"))
{
    archive.Entries.First().Extract("data.bin");
}
```

### Siehe auch

* class [XarFileEntry](../)
* namensraum [Aspose.Zip.Xar](../../xarfileentry/)
* Montage [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extrahiert den Eintrag zum bereitgestellten Stream.

```csharp
public abstract void Extract(Stream destination)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destination | Stream | Zielstrom. Muss beschreibbar sein. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | *destination* unterstützt das Schreiben nicht. |

### Beispiele

Extrahieren Sie einen Eintrag des WIM-Archivs.

```csharp
using (var archive = new WimArchive("archive.wim"))
{
    archive.Images[0].RootDirectory.Files[0].Extract(httpResponseStream);
}
```

### Siehe auch

* class [XarFileEntry](../)
* namensraum [Aspose.Zip.Xar](../../xarfileentry/)
* Montage [Aspose.Zip](../../../)


