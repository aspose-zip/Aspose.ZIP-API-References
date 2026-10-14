---
title: "IsoArchive.IsoArchive"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "IsoArchive Konstruktor. Initialisiert eine neue Instanz der IsoArchive Klasse und erstellt ein leeres ISO-Archiv zum Hinzufügen neuer Dateien und Verzeichnisse."
type: docs
weight: 10
url: /de/net/aspose.zip.iso/isoarchive/isoarchive/
---
## IsoArchive() {#constructor}

Initialisiert eine neue Instanz der [`IsoArchive`](../) Klasse und erstellt ein leeres ISO-Archiv zum Hinzufügen neuer Dateien und Verzeichnisse.

```csharp
public IsoArchive()
```

## Beispiele

Das folgende Beispiel zeigt, wie ein neues leeres ISO-Archiv erstellt und Dateien zu ihm hinzugefügt werden:

```csharp
// Erstelle ein neues leeres ISO-Archiv
using(IsoArchive isoArchive = new IsoArchive())
{
    // Füge Dateien zum ISO-Archiv hinzu
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // Speichere das ISO-Archiv in einer Datei
    isoArchive.Save("new_archive.iso");
}
```

### Siehe auch

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(Stream, IsoLoadOptions) {#constructor_1}

Initialisiert eine neue Instanz der [`IsoArchive`](../) Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

```csharp
public IsoArchive(Stream sourceStream, IsoLoadOptions loadOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | Stream | Die Quelle des Archivs. Sie muss suchbar sein. |
| loadOptions | IsoLoadOptions | Die Optionen, mit denen das Archiv geladen wird. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *sourceStream* ist null. |
| ArgumentException | *sourceStream* ist nicht suchbar. |
| InvalidDataException | *sourceStream* ist kein gültiges ISO-Archiv. |
| ObjectDisposedException | Wird ausgelöst, wenn der Quellstream freigegeben wurde. |
| EndOfStreamException | Wird ausgelöst, wenn das Ende des Streams unerwartet erreicht wird. |
| IOException | Ein I/O-Fehler ist aufgetreten. |
| NotSupportedException | Der Stream unterstützt kein Lesen. |

## Hinweise

Dieser Konstruktor entpackt keinen Eintrag.

## Beispiele

Das folgende Beispiel zeigt, wie alle Einträge in ein Verzeichnis extrahiert werden.

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Siehe auch

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(string, IsoLoadOptions) {#constructor_2}

Initialisiert eine neue Instanz der [`IsoArchive`](../) Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

```csharp
public IsoArchive(string path, IsoLoadOptions loadOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der Pfad zur Archivdatei. |
| loadOptions | IsoLoadOptions | Die Optionen, mit denen das Archiv geladen wird. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *path* ist null. |
| SecurityException | Der Aufrufer hat nicht die erforderliche Berechtigung zum Zugriff. |
| ArgumentException | Der *path* ist leer, enthält nur Leerzeichen oder ungültige Zeichen. |
| UnauthorizedAccessException | Zugriff auf Datei *path* wurde verweigert. |
| PathTooLongException | Der angegebene *path*, Dateiname oder beides überschreiten die systemdefinierte maximale Länge. Zum Beispiel müssen Pfade auf Windows‑basierten Plattformen weniger als 248 Zeichen lang sein und Dateinamen weniger als 260 Zeichen. |
| NotSupportedException | Datei bei *path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenkette. |
| FileNotFoundException | Die Datei wurde nicht gefunden. |
| DirectoryNotFoundException | Der angegebene Pfad ist ungültig, z. B. weil er sich auf einem nicht zugeordneten Laufwerk befindet. |
| IOException | Die Datei ist bereits geöffnet. |
| EndOfStreamException | Die Datei ist zu kurz. |
| InvalidDataException | Wird ausgelöst, wenn die Daten ungültig oder beschädigt sind. |

## Hinweise

Dieser Konstruktor entpackt keinen Eintrag.

## Beispiele

Das folgende Beispiel zeigt, wie alle Einträge in ein Verzeichnis extrahiert werden.

```csharp
using (var archive = new IsoArchive("archive.iso")) 
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Siehe auch

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


