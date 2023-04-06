---
title: GzipArchive.SetSource
second_title: Aspose.ZIP für .NET-API-Referenz
description: GzipArchive methode. Legt den Inhalt fest der innerhalb des Archivs komprimiert werden soll.
type: docs
weight: 70
url: /de/net/aspose.zip.gzip/gziparchive/setsource/
---
## SetSource(Stream) {#setsource_2}

Legt den Inhalt fest, der innerhalb des Archivs komprimiert werden soll.

```csharp
public void SetSource(Stream source)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | Stream | Der Eingabestream für das Archiv. |

### Beispiele

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.gz");
}
```

### Siehe auch

* class [GzipArchive](../)
* namensraum [Aspose.Zip.Gzip](../../gziparchive/)
* Montage [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

Legt den Inhalt fest, der innerhalb des Archivs komprimiert werden soll.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileInfo | FileInfo | Der Verweis auf eine zu komprimierende Datei. |

### Beispiele

Öffnen Sie ein Archiv aus einem Stream und extrahieren Sie es in a`MemoryStream`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.gz");
}
```

### Siehe auch

* class [GzipArchive](../)
* namensraum [Aspose.Zip.Gzip](../../gziparchive/)
* Montage [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

Legt den Inhalt fest, der innerhalb des Archivs komprimiert werden soll.

```csharp
public void SetSource(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | String | Pfad zur zu komprimierenden Datei. |

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

Öffnen Sie ein Archiv aus Datei nach Pfad und extrahieren Sie es in a`MemoryStream`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Siehe auch

* class [GzipArchive](../)
* namensraum [Aspose.Zip.Gzip](../../gziparchive/)
* Montage [Aspose.Zip](../../../)

---

## SetSource(TarArchive) {#setsource}

Legt den Inhalt fest, der innerhalb des Archivs komprimiert werden soll.

```csharp
public void SetSource(TarArchive tarArchive)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| tarArchive | TarArchive | Tar-Archiv zu komprimieren. |

### Bemerkungen

Verwenden Sie diese Methode, um ein gemeinsames tar.gz-Archiv zu erstellen.

### Beispiele

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var gzippedArchive = new GzipArchive())
    {
           gzippedArchive.SetSource(tarArchive);
           gzippedArchive.Save("archive.tar.gz");
    }
}
```

### Siehe auch

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* class [GzipArchive](../)
* namensraum [Aspose.Zip.Gzip](../../gziparchive/)
* Montage [Aspose.Zip](../../../)


