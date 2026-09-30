---
title: "LzxArchive.LzxArchive"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "LzxArchive-Konstruktor. Initialisiert eine neue Instanz der LzxArchive-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann."
type: docs
weight: 10
url: /de/net/aspose.zip.lzx/lzxarchive/lzxarchive/
---
## LzxArchive(Stream, LzxLoadOptions) {#constructor}

Initialisiert eine neue Instanz der [`LzxArchive`](../)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

```csharp
public LzxArchive(Stream extractionSource, LzxLoadOptions loadOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| extractionSource | Stream | Die Quelle des Archivs. |
| loadOptions | LzxLoadOptions | Optionen zum Laden eines vorhandenen Archivs. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *extractionSource* ist null. |
| ArgumentException | *extractionSource* unterstützt kein Suchen. |
| InvalidDataException | Falsche Signatur für das Archiv. - oder - Die Datei ist kein LZX-Archiv. |
| NotImplementedException | Lzx-Archiv enthält zusammengeführte Einträge. |
| EndOfStreamException | Der *extractionSource*-Stream ist zu kurz. |
| ObjectDisposedException | Wird ausgelöst, wenn der Stream geschlossen wurde. |
| IOException | Ein I/O-Fehler ist aufgetreten. |

## Hinweise

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die [`Extract`](../../lzxarchiveentry/extract/)-Methode zum Dekomprimieren.

### Siehe auch

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzxArchive(string, LzxLoadOptions) {#constructor_1}

Initialisiert eine neue Instanz der [`LzxArchive`](../)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

```csharp
public LzxArchive(string path, LzxLoadOptions loadOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der vollständig qualifizierte oder relative Pfad zur Archivdatei. |
| loadOptions | LzxLoadOptions | Optionen zum Laden eines vorhandenen Archivs. |

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
| InvalidDataException | Die Datei ist beschädigt. |
| NotImplementedException | Lzx-Archiv enthält zusammengeführte Einträge. |
| EndOfStreamException | Die Datei ist zu kurz. |
| ObjectDisposedException | Wird ausgelöst, wenn der Stream geschlossen wurde. |

## Hinweise

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die [`Extract`](../../lzxarchiveentry/extract/)-Methode zum Dekomprimieren.

## Beispiele

Das folgende Beispiel extrahiert ein Archiv und dekomprimiert dann den ersten Eintrag in einen `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LzxArchive archive = new LzxArchive("sample.lzx"))
{
    archive.Entries[0].Extract(extracted);
}
```

### Siehe auch

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)


