---
title: "IsoArchive.CreateEntry"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "IsoArchive-Methode. Fügt eine Datei zum ISO‑Image hinzu"
type: docs
weight: 40
url: /de/net/aspose.zip.iso/isoarchive/createentry/
---
## CreateEntry(string, string) {#createentry_2}

Fügt dem ISO-Image eine Datei hinzu.

```csharp
public IsoEntry CreateEntry(string name, string filePath)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Pfad der Datei im ISO‑Image. |
| Dateipfad | String | Pfad der Datei. |

### Rückgabewert

Der ISO-Eintrag wurde erstellt.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | Der *filePath* ist null. |
| ArgumentException | Der *filePath* ist leer, enthält nur Leerzeichen oder ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf Datei *filePath* wurde verweigert. |
| PathTooLongException | Der angegebene *filePath* überschreitet die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Datei bei *filePath* enthält einen Doppelpunkt (:) in der Mitte der Zeichenkette. |
| IOException | Beim Öffnen der Datei ist ein I/O-Fehler aufgetreten. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig (zum Beispiel, weil er sich auf einem nicht zugeordneten Laufwerk befindet). |
| FileNotFoundException | Die in *filePath* angegebene Datei wurde nicht gefunden. |
| InvalidOperationException | Das Archiv befindet sich nicht im Bearbeitungsmodus. |

### Siehe auch

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Fügt dem ISO-Image eine Datei hinzu.

```csharp
public IsoEntry CreateEntry(string name, Stream source)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Pfad der Datei im ISO‑Image. |
| Quelle | Stream | Stream, der die Dateidaten enthält. |

### Rückgabewert

Der ISO-Eintrag wurde erstellt.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |
| ArgumentNullException | Wird ausgelöst, wenn ein *name* oder *source* null ist. |
| InvalidOperationException | Das Archiv befindet sich nicht im Bearbeitungsmodus. |

### Siehe auch

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string) {#createentry}

Fügt dem ISO-Image eine Datei hinzu.

```csharp
public IsoEntry CreateEntry(string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | String | Pfad des Verzeichnisses im ISO. |

### Rückgabewert

Der ISO-Eintrag wurde erstellt.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | `name` ist null oder leer. |
| InvalidOperationException | Das Archiv ist zum Extrahieren geöffnet. |
| ObjectDisposedException | Das Archiv wurde freigegeben und kann nicht verwendet werden. |

### Siehe auch

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


