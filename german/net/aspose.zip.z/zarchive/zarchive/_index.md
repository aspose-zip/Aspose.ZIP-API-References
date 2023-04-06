---
title: ZArchive.ZArchive
second_title: Aspose.ZIP für .NET-API-Referenz
description: ZArchive constructeur. Initialisiert eine neue Instanz vonZArchive Klasse zum Komprimieren vorbereitet.
type: docs
weight: 10
url: /de/net/aspose.zip.z/zarchive/zarchive/
---
## ZArchive() {#constructor}

Initialisiert eine neue Instanz von[`ZArchive`](../) Klasse zum Komprimieren vorbereitet.

```csharp
public ZArchive()
```

### Siehe auch

* class [ZArchive](../)
* namensraum [Aspose.Zip.Z](../../zarchive/)
* Montage [Aspose.Zip](../../../)

---

## ZArchive(Stream) {#constructor_1}

Initialisiert eine neue Instanz von[`ZArchive`](../) Klasse zum Dekomprimieren vorbereitet.

```csharp
public ZArchive(Stream source)
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

* class [ZArchive](../)
* namensraum [Aspose.Zip.Z](../../zarchive/)
* Montage [Aspose.Zip](../../../)

---

## ZArchive(string) {#constructor_2}

Initialisiert eine neue Instanz von[`ZArchive`](../) Klasse zum Dekomprimieren vorbereitet.

```csharp
public ZArchive(string path)
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

### Siehe auch

* class [ZArchive](../)
* namensraum [Aspose.Zip.Z](../../zarchive/)
* Montage [Aspose.Zip](../../../)


