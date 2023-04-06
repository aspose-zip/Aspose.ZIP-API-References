---
title: Bzip2Archive.Bzip2Archive
second_title: Aspose.ZIP für .NET-API-Referenz
description: Bzip2Archive constructeur. Initialisiert eine neue Instanz vonBzip2Archive Klasse zum Komprimieren vorbereitet.
type: docs
weight: 10
url: /de/net/aspose.zip.bzip2/bzip2archive/bzip2archive/
---
## Bzip2Archive() {#constructor}

Initialisiert eine neue Instanz von[`Bzip2Archive`](../) Klasse zum Komprimieren vorbereitet.

```csharp
public Bzip2Archive()
```

### Beispiele

Das folgende Beispiel zeigt, wie eine Datei komprimiert wird.

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### Siehe auch

* class [Bzip2Archive](../)
* namensraum [Aspose.Zip.Bzip2](../../bzip2archive/)
* Montage [Aspose.Zip](../../../)

---

## Bzip2Archive(Stream) {#constructor_1}

Initialisiert eine neue Instanz von[`Bzip2Archive`](../) Klasse zum Dekomprimieren vorbereitet.

```csharp
public Bzip2Archive(Stream sourceStream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | Stream | Die Quelle des Archivs. |

### Bemerkungen

Dieser Konstruktor wird nicht dekomprimiert. Sehen[`Open`](../open/) Methode zum Dekomprimieren.

### Beispiele

Öffnen Sie ein Archiv aus einem Stream und extrahieren Sie es in a`MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive(File.OpenRead("archive.bz2")))
  archive.Open().CopyTo(ms);
```

### Siehe auch

* class [Bzip2Archive](../)
* namensraum [Aspose.Zip.Bzip2](../../bzip2archive/)
* Montage [Aspose.Zip](../../../)

---

## Bzip2Archive(string) {#constructor_2}

Initialisiert eine neue Instanz von[`Bzip2Archive`](../) Klasse zum Dekomprimieren vorbereitet.

```csharp
public Bzip2Archive(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | String | Der Pfad zur Archivdatei. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *path* ist Null. |
| SecurityException | Der Anrufer verfügt nicht über die erforderliche Zugriffsberechtigung. |
| ArgumentException | Der*path* leer ist, nur Leerzeichen enthält oder ungültige Zeichen enthält. |
| UnauthorizedAccessException | Zugriff auf Datei*path* ist abgelehnt. |
| PathTooLongException | Die angegebene*path*, Dateiname oder beide überschreiten die vom System definierte maximale Länge. Beispielsweise müssen auf Windows-basierten Plattformen Pfade weniger als 248 Zeichen und Dateinamen weniger als 260 Zeichen umfassen. |
| NotSupportedException | Datei unter*path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenfolge. |

### Bemerkungen

Dieser Konstruktor wird nicht dekomprimiert. Sehen[`Open`](../open/) Methode zum Dekomprimieren.

### Beispiele

Öffnen Sie ein Archiv aus Datei nach Pfad und extrahieren Sie es in a`MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
  archive.Open().CopyTo(ms);
```

### Siehe auch

* class [Bzip2Archive](../)
* namensraum [Aspose.Zip.Bzip2](../../bzip2archive/)
* Montage [Aspose.Zip](../../../)


