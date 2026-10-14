---
title: "Lz4Archive.Lz4Archive"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "Lz4Archive-Konstruktor. Initialisiert eine neue Instanz der Lz4Archive-Klasse, die für die Dekomprimierung vorbereitet ist."
type: docs
weight: 10
url: /de/net/aspose.zip.lz4/lz4archive/lz4archive/
---
## Lz4Archive(Stream, Lz4LoadOptions) {#constructor_1}

Initialisiert eine neue Instanz der [`Lz4Archive`](../)-Klasse, die für die Dekomprimierung vorbereitet ist.

```csharp
public Lz4Archive(Stream sourceStream, Lz4LoadOptions loadOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | Stream | Die Quelle des Archivs. |
| loadOptions | Lz4LoadOptions | Die Optionen, mit denen das Archiv geladen wird. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | Kann nicht von *sourceStream* lesen |
| ArgumentNullException | *sourceStream* ist null. |
| EndOfStreamException | *sourceStream* ist zu kurz. |
| InvalidDataException | Der *sourceStream* hat eine falsche Signatur. |
| ObjectDisposedException | Wird ausgelöst, wenn der Quellstream freigegeben wurde. |
| IOException | Ein I/O-Fehler ist aufgetreten. |

## Hinweise

Dieser Konstruktor dekomprimiert nicht. Siehe die [`Open`](../open/)-Methode zum Dekomprimieren.

## Beispiele

Öffnen Sie ein Archiv aus einem Stream und extrahieren Sie es in einen `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive(File.OpenRead("archive.lz4")))
  archive.Open().CopyTo(ms);
```

### Siehe auch

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(string, Lz4LoadOptions) {#constructor_2}

Initialisiert eine neue Instanz der [`Lz4Archive`](../)-Klasse.

```csharp
public Lz4Archive(string path, Lz4LoadOptions loadOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der Pfad zur Archivdatei. |
| loadOptions | Lz4LoadOptions | Die Optionen, mit denen das Archiv geladen wird. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *path* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung zum Zugriff. |
| ArgumentException | Der *path* ist leer, enthält nur Leerzeichen oder ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf Datei *path* wurde verweigert. |
| PathTooLongException | Der angegebene *path*, Dateiname oder beides überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Datei bei *path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenkette. |
| EndOfStreamException | Die Datei ist zu kurz. |
| InvalidDataException | Daten in der Datei haben die falsche Signatur. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig, z. B. weil er sich auf einem nicht zugeordneten Laufwerk befindet. |
| FileNotFoundException | Die Datei wurde nicht gefunden. |
| IOException | Die Datei ist bereits geöffnet. |

## Hinweise

Dieser Konstruktor dekomprimiert nicht. Siehe die [`Open`](../open/)-Methode zum Dekomprimieren.

## Beispiele

Öffnen Sie ein Archiv aus einer Datei über den Pfad und extrahieren Sie es in einen `MemoryStream`.

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive("archive.lz4"))
  archive.Open().CopyTo(ms);
```

### Siehe auch

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(Lz4ArchiveSetting) {#constructor}

Initialisiert eine neue Instanz der [`Lz4Archive`](../)-Klasse, die für die Komprimierung vorbereitet ist.

```csharp
public Lz4Archive(Lz4ArchiveSetting settings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Einstellungen | Lz4ArchiveSetting | Die Einstellung des zusammengesetzten Archivs. |

### Siehe auch

* class [Lz4ArchiveSetting](../../lz4archivesetting/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


