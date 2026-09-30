---
title: "ArjArchive.ArjArchive"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "ArjArchive-Konstruktor. Initialisiert eine neue Instanz der ArjArchive-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann."
type: docs
weight: 10
url: /de/net/aspose.zip.arj/arjarchive/arjarchive/
---
## ArjArchive(Stream, ArjLoadOptions) {#constructor}

Initialisiert eine neue Instanz der [`ArjArchive`](../)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

```csharp
public ArjArchive(Stream extractionSource, ArjLoadOptions loadOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| extractionSource | Stream | Die Quelle des Archivs. |
| loadOptions | ArjLoadOptions | Optionen zum Laden eines vorhandenen Archivs. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *extractionSource* ist null. |
| ArgumentException | &gt;*extractionSource* unterstützt kein Suchen. |
| InvalidDataException | Falsche Signatur für das Archiv. - oder - Die Datei ist kein ARJ-Archiv. |
| EndOfStreamException | Wird ausgelöst, wenn das Ende des Streams erreicht wird, bevor alle Header‑Bytes oder Namens‑Bytes gelesen wurden. |
| NotSupportedException | Das Archiv ist beschädigt. |

## Hinweise

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methode [`Extract`](../../arjentryplain/extract/) zum Dekomprimieren.

### Siehe auch

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)

---

## ArjArchive(string, ArjLoadOptions) {#constructor_1}

Initialisiert eine neue Instanz der [`ArjArchive`](../)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

```csharp
public ArjArchive(string path, ArjLoadOptions loadOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der Pfad zur Archivdatei. |
| loadOptions | ArjLoadOptions | Optionen zum Laden eines vorhandenen Archivs. |

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
| EndOfStreamException | Wird ausgelöst, wenn das Ende des Streams erreicht wird, bevor alle Header‑Bytes oder Namens‑Bytes gelesen wurden. |
| InvalidDataException | Die ARJ-Magische Zahl ist ungültig oder die Header‑Größe liegt außerhalb des zulässigen Bereichs. |

## Hinweise

Dieser Konstruktor packt keinen Eintrag aus. Siehe die Methode [`Extract`](../../arjentryplain/extract/) zum Dekomprimieren.

## Beispiele

Das folgende Beispiel zeigt, wie alle Einträge in ein Verzeichnis extrahiert werden.

```csharp
using (var archive = new ArjArchive("archive.arj")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Siehe auch

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


