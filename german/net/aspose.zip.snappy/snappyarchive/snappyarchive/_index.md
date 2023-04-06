---
title: SnappyArchive.SnappyArchive
second_title: Aspose.ZIP für .NET-API-Referenz
description: SnappyArchive constructeur. Initialisiert eine neue Instanz vonSnappyArchive Klasse zum Komprimieren vorbereitet.
type: docs
weight: 10
url: /de/net/aspose.zip.snappy/snappyarchive/snappyarchive/
---
## SnappyArchive() {#constructor}

Initialisiert eine neue Instanz von[`SnappyArchive`](../) Klasse zum Komprimieren vorbereitet.

```csharp
public SnappyArchive()
```

### Beispiele

Das folgende Beispiel zeigt, wie eine Datei komprimiert wird.

```csharp
using (SnappyArchive archive = new SnappyArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.snapy");
}
```

### Siehe auch

* class [SnappyArchive](../)
* namensraum [Aspose.Zip.Snappy](../../snappyarchive/)
* Montage [Aspose.Zip](../../../)

---

## SnappyArchive(Stream) {#constructor_1}

Initialisiert eine neue Instanz von[`SnappyArchive`](../) Klasse zum Dekomprimieren vorbereitet.

```csharp
public SnappyArchive(Stream source)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | Stream | Die Quelle des Archivs. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | *source* ist nicht auffindbar. |
| ArgumentNullException | *source* ist Null. |

### Bemerkungen

Dieser Konstruktor wird nicht dekomprimiert. Sehen[`Extract`](../extract/) Methode zum Dekomprimieren.

### Siehe auch

* class [SnappyArchive](../)
* namensraum [Aspose.Zip.Snappy](../../snappyarchive/)
* Montage [Aspose.Zip](../../../)

---

## SnappyArchive(string) {#constructor_2}

Initialisiert eine neue Instanz von[`SnappyArchive`](../) Klasse zum Dekomprimieren vorbereitet.

```csharp
public SnappyArchive(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | String | Pfad zur Quelle des Archivs. |

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

Dieser Konstruktor wird nicht dekomprimiert. Sehen[`Extract`](../extract/) Methode zum Dekomprimieren.

### Beispiele

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new SnappyArchive(sourceSnappyFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### Siehe auch

* class [SnappyArchive](../)
* namensraum [Aspose.Zip.Snappy](../../snappyarchive/)
* Montage [Aspose.Zip](../../../)


