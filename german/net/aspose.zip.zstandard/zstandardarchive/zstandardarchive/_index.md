---
title: "ZstandardArchive.ZstandardArchive"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "ZstandardArchive-Konstruktor. Initialisiert eine neue Instanz der ZstandardArchive-Klasse, die zum Komprimieren vorbereitet ist."
type: docs
weight: 10
url: /de/net/aspose.zip.zstandard/zstandardarchive/zstandardarchive/
---
## ZstandardArchive() {#constructor}

Initialisiert eine neue Instanz der [`ZstandardArchive`](../)-Klasse, die zum Komprimieren vorbereitet ist.

```csharp
public ZstandardArchive()
```

## Beispiele

Das folgende Beispiel zeigt, wie man eine Datei komprimiert.

```csharp
using (ZstandardArchive archive = new ZstandardArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.zst");
}
```

### Siehe auch

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(Stream, ZstandardLoadOptions) {#constructor_1}

Initialisiert eine neue Instanz der [`ZstandardArchive`](../)-Klasse, die zum Dekomprimieren vorbereitet ist.

```csharp
public ZstandardArchive(Stream sourceStream, ZstandardLoadOptions options = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | Stream | Die Quelle des Archivs. |
| Optionen | ZstandardLoadOptions | Die Optionen, mit denen das Archiv geladen wird. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Wird ausgelöst, wenn der Quellstream freigegeben wurde. |
| EndOfStreamException | Wird ausgelöst, wenn das Ende des Streams unerwartet erreicht wird. |
| IOException | Ein I/O-Fehler ist aufgetreten. |
| InvalidDataException | Wird ausgelöst, wenn die Daten ungültig oder beschädigt sind. |

## Hinweise

Dieser Konstruktor dekomprimiert nicht. Siehe die [`Open`](../open/)-Methode zum Dekomprimieren.

## Beispiele

Öffnen Sie ein Archiv aus einem Stream und extrahieren Sie es in einen `MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new ZstandardArchive(File.OpenRead("archive.zst")))
  archive.Open().CopyTo(ms);
```

### Siehe auch

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(string, ZstandardLoadOptions) {#constructor_2}

Initialisiert eine neue Instanz der [`ZstandardArchive`](../)-Klasse.

```csharp
public ZstandardArchive(string path, ZstandardLoadOptions options = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der Pfad zur Archivdatei. |
| Optionen | ZstandardLoadOptions | Die Optionen, mit denen das Archiv geladen wird. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *path* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung zum Zugriff. |
| ArgumentException | Der *path* ist leer, enthält nur Leerzeichen oder ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf Datei *path* wurde verweigert. |
| PathTooLongException | Der angegebene *path*, Dateiname oder beides überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Datei bei *path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenkette. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig, z. B. weil er sich auf einem nicht zugeordneten Laufwerk befindet. |
| EndOfStreamException | Wird ausgelöst, wenn das Ende des Streams unerwartet erreicht wird. |
| FileNotFoundException | Die Datei wurde nicht gefunden. |
| IOException | Die Datei ist bereits geöffnet. |
| InvalidDataException | Wird ausgelöst, wenn die Daten ungültig oder beschädigt sind. |

## Hinweise

Dieser Konstruktor dekomprimiert nicht. Siehe die [`Open`](../open/)-Methode zum Dekomprimieren.

## Beispiele

Öffnen Sie ein Archiv aus einer Datei über den Pfad und extrahieren Sie es in einen `MemoryStream`.

```csharp
var ms = new MemoryStream();
using (ZstandardArchive archive = new ZstandardArchive("archive.zst"))
  archive.Open().CopyTo(ms);
```

### Siehe auch

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


