---
title: XzArchive.XzArchive
second_title: Aspose.ZIP für .NET-API-Referenz
description: XzArchive constructeur. Initialisiert eine neue Instanz vonXzArchive Klasse und erstellt das Archiv im xzFormat.
type: docs
weight: 10
url: /de/net/aspose.zip.xz/xzarchive/xzarchive/
---
## XzArchive(XzArchiveSettings) {#constructor}

Initialisiert eine neue Instanz von[`XzArchive`](../) Klasse und erstellt das Archiv im xz-Format.

```csharp
public XzArchive(XzArchiveSettings settings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| settings | XzArchiveSettings | Einstellungssatz für bestimmte xz-Archive: Wörterbuchgröße, Blockgröße, Überprüfungstyp. |

### Siehe auch

* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [XzArchive](../)
* namensraum [Aspose.Zip.Xz](../../xzarchive/)
* Montage [Aspose.Zip](../../../)

---

## XzArchive(Stream) {#constructor_1}

Initialisiert eine neue Instanz von[`XzArchive`](../) Klasse zum Dekomprimieren vorbereitet.

```csharp
public XzArchive(Stream source)
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

* class [XzArchive](../)
* namensraum [Aspose.Zip.Xz](../../xzarchive/)
* Montage [Aspose.Zip](../../../)

---

## XzArchive(string) {#constructor_2}

Initialisiert eine neue Instanz von[`XzArchive`](../) Klasse zum Dekomprimieren vorbereitet.

```csharp
public XzArchive(string path)
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

* class [XzArchive](../)
* namensraum [Aspose.Zip.Xz](../../xzarchive/)
* Montage [Aspose.Zip](../../../)


