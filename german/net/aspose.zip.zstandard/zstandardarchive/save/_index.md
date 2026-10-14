---
title: "ZstandardArchive.Save"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "ZstandardArchive-Methode. Speichert das Archiv in den bereitgestellten Stream."
type: docs
weight: 60
url: /de/net/aspose.zip.zstandard/zstandardarchive/save/
---
## Save(Stream, ZstandardSaveOptions) {#save_1}

Speichert das Archiv in den bereitgestellten Stream.

```csharp
public void Save(Stream outputStream, ZstandardSaveOptions settings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| outputStream | Stream | Ziel-Stream. |
| Einstellungen | ZstandardSaveOptions | Optionale Einstellungen für die Archivzusammensetzung. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| ArgumentException | *outputStream* ist nicht beschreibbar. |
| InvalidOperationException | Quelle wurde nicht angegeben. |

## Hinweise

*outputStream* must be writable.

## Beispiele

Komprimierte Daten in den HTTP-Antwort-Stream schreiben.

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Siehe auch

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, ZstandardSaveOptions) {#save_2}

Speichert das Archiv in die angegebene Zieldatei.

```csharp
public void Save(string destinationFileName, ZstandardSaveOptions settings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationFileName | String | Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine vorhandene Datei verweist, wird diese überschrieben. |
| Einstellungen | ZstandardSaveOptions | Optionale Einstellungen für die Archivzusammensetzung. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| ArgumentNullException | *destinationFileName* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung zum Zugriff. |
| ArgumentException | Der *destinationFileName* ist leer, enthält nur Leerzeichen oder enthält ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf die Datei *destinationFileName* wurde verweigert. |
| PathTooLongException | Der angegebene *destinationFileName*, Dateiname oder beide überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Die Datei bei *destinationFileName* enthält einen Doppelpunkt (:) in der Mitte der Zeichenkette. |
| Exception | Wird ausgelöst, wenn ein Laufzeitfehler auftritt. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig (zum Beispiel, weil er sich auf einem nicht zugeordneten Laufwerk befindet). |
| IOException | Beim Öffnen der Datei ist ein I/O-Fehler aufgetreten. |
| InvalidOperationException | Quelle wurde nicht angegeben. |

## Beispiele

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.zst");
}
```

### Siehe auch

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo, ZstandardSaveOptions) {#save}

Speichert das Archiv in die angegebene Zieldatei.

```csharp
public void Save(FileInfo destination, ZstandardSaveOptions settings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ziel | FileInfo | FileInfo, das als Ziel-Stream geöffnet wird. |
| Einstellungen | ZstandardSaveOptions | Optionale Einstellungen für die Archivzusammensetzung. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung, das *destination* zu öffnen. |
| ArgumentException | Der Dateipfad ist leer oder enthält nur Leerzeichen. |
| FileNotFoundException | Die Datei wurde nicht gefunden. |
| UnauthorizedAccessException | Der Pfad zur Datei ist schreibgeschützt oder ein Verzeichnis. |
| ArgumentNullException | *destination* ist null. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig, z. B. weil er sich auf einem nicht zugeordneten Laufwerk befindet. |
| IOException | Die Datei ist bereits geöffnet. |
| InvalidOperationException | Quelle wurde nicht angegeben. |

## Beispiele

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.zst"));
}
```

### Siehe auch

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


