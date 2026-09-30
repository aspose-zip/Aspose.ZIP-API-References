---
title: "EggArchive.EggArchive"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "EggArchive-Konstruktor. Initialisiert eine neue Instanz der EggArchive-Klasse aus einem Stream"
type: docs
weight: 10
url: /de/net/aspose.zip.egg/eggarchive/eggarchive/
---
## EggArchive(Stream, EggArchiveLoadOptions) {#constructor}

Initialisiert eine neue Instanz der [`EggArchive`](../)-Klasse aus einem Stream.

```csharp
public EggArchive(Stream stream, EggArchiveLoadOptions loadOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Der EGG-Archiv-Stream. Der Stream muss das Lesen und Suchen unterstützen. |
| loadOptions | EggArchiveLoadOptions | Optionen zum Laden des Archivs. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *stream* ist null. |
| ArgumentException | *stream* ist nicht lesbar und nicht suchbar. |

### Siehe auch

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)

---

## EggArchive(string, EggArchiveLoadOptions) {#constructor_1}

Initialisiert eine neue Instanz der [`EggArchive`](../)-Klasse aus einem Dateipfad.

```csharp
public EggArchive(string path, EggArchiveLoadOptions loadOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Pfad zur EGG-Archivdatei. |
| loadOptions | EggArchiveLoadOptions | Optionen zum Laden des Archivs. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *path* ist null. |
| FileNotFoundException | Die Datei existiert nicht. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung zum Zugriff. |
| ArgumentException | Der *path* ist leer, enthält nur Leerzeichen oder ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf Datei *path* wurde verweigert. |
| PathTooLongException | Der angegebene *path*, Dateiname oder beides überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Datei bei *path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenkette. |
| FileNotFoundException | Die Datei wurde nicht gefunden. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig, z. B. weil er sich auf einem nicht zugeordneten Laufwerk befindet. |
| IOException | Die Datei ist bereits geöffnet. |

### Siehe auch

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)


