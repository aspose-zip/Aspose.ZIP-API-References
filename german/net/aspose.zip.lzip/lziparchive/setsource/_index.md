---
title: LzipArchive.SetSource
second_title: Aspose.ZIP für .NET-API-Referenz
description: LzipArchive methode. Legt den Inhalt fest der innerhalb des Archivs komprimiert werden soll.
type: docs
weight: 60
url: /de/net/aspose.zip.lzip/lziparchive/setsource/
---
## SetSource(Stream) {#setsource_1}

Legt den Inhalt fest, der innerhalb des Archivs komprimiert werden soll.

```csharp
public void SetSource(Stream source)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | Stream | Der Eingabestream für das Archiv. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | Der*source* Stream ist unauffindbar. |

### Beispiele

```csharp
using (var archive = new LzipArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.lz");

```

### Siehe auch

* class [LzipArchive](../)
* namensraum [Aspose.Zip.Lzip](../../lziparchive/)
* Montage [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

Legt den Inhalt fest, der innerhalb des Archivs komprimiert werden soll.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo, die als Eingabestream geöffnet wird. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| SecurityException | Der Anrufer hat nicht die erforderliche Berechtigung zum Öffnen der*fileInfo*. |
| ArgumentException | Dateipfad ist leer oder enthält nur Leerzeichen. |
| FileNotFoundException | Die Datei wird nicht gefunden. |
| UnauthorizedAccessException | Pfad zur Datei ist schreibgeschützt oder ist ein Verzeichnis. |
| ArgumentNullException | *fileInfo* ist Null. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig, da er sich beispielsweise auf einem nicht zugeordneten Laufwerk befindet. |
| IOException | Die Datei ist bereits geöffnet. |

### Beispiele

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.lz");
}
```

### Siehe auch

* class [LzipArchive](../)
* namensraum [Aspose.Zip.Lzip](../../lziparchive/)
* Montage [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Legt den Inhalt fest, der innerhalb des Archivs komprimiert werden soll.

```csharp
public void SetSource(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | String | Pfad zur zu komprimierenden Datei.. |

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
using (var archive = new LzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz");
}
```

### Siehe auch

* class [LzipArchive](../)
* namensraum [Aspose.Zip.Lzip](../../lziparchive/)
* Montage [Aspose.Zip](../../../)


