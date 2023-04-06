---
title: LzipArchive.Save
second_title: Aspose.ZIP für .NET-API-Referenz
description: LzipArchive methode. Speichert das lzipArchiv im bereitgestellten Stream.
type: docs
weight: 50
url: /de/net/aspose.zip.lzip/lziparchive/save/
---
## Save(Stream) {#save_1}

Speichert das lzip-Archiv im bereitgestellten Stream.

```csharp
public void Save(Stream outputStream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| outputStream | Stream | Zielstrom. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | *outputStream* unterstützt nicht das Suchen. |
| ArgumentNullException | *outputStream* ist Null. |

### Bemerkungen

*outputStream* muss auffindbar sein.

### Beispiele

```csharp
using (FileStream lzFile = File.Open("archive.lz", FileMode.Create))
{
    using (var archive = new LzipArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(lzFile);
     }
}
```

### Siehe auch

* class [LzipArchive](../)
* namensraum [Aspose.Zip.Lzip](../../lziparchive/)
* Montage [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

Speichert das lzip-Archiv in der bereitgestellten Zieldatei.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationFileName | String | Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine vorhandene Datei verweist, wird diese überschrieben. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *destinationFileName* ist Null. |
| SecurityException | Der Anrufer verfügt nicht über die erforderliche Zugriffsberechtigung. |
| ArgumentException | Der*destinationFileName* leer ist, nur Leerzeichen enthält oder ungültige Zeichen enthält. |
| UnauthorizedAccessException | Zugriff auf Datei*destinationFileName* ist abgelehnt. |
| PathTooLongException | Die angegebene*destinationFileName*, Dateiname oder beide überschreiten die vom System definierte maximale Länge. Beispielsweise müssen auf Windows-basierten Plattformen Pfade weniger als 248 Zeichen und Dateinamen weniger als 260 Zeichen umfassen. |
| NotSupportedException | Datei unter*destinationFileName* enthält einen Doppelpunkt (:) in der Mitte der Zeichenfolge. |

### Beispiele

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.lz");
}
```

### Siehe auch

* class [LzipArchive](../)
* namensraum [Aspose.Zip.Lzip](../../lziparchive/)
* Montage [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Speichert das lzip-Archiv in der bereitgestellten Zieldatei.

```csharp
public void Save(FileInfo destination)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destination | FileInfo | FileInfo, die als Zielstream geöffnet wird. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| SecurityException | Der Anrufer hat nicht die erforderliche Berechtigung zum Öffnen der*destination*. |
| ArgumentException | Dateipfad ist leer oder enthält nur Leerzeichen. |
| FileNotFoundException | Die Datei wird nicht gefunden. |
| UnauthorizedAccessException | Pfad zur Datei ist schreibgeschützt oder ist ein Verzeichnis. |
| ArgumentNullException | *destination* ist Null. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig, da er sich beispielsweise auf einem nicht zugeordneten Laufwerk befindet. |
| IOException | Die Datei ist bereits geöffnet. |

### Beispiele

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz"));
}
```

### Siehe auch

* class [LzipArchive](../)
* namensraum [Aspose.Zip.Lzip](../../lziparchive/)
* Montage [Aspose.Zip](../../../)


