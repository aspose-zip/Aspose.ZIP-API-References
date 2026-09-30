---
title: "LhaArchive.LhaArchive"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "LhaArchive-Konstruktor. Initialisiert eine neue Instanz der LhaArchive-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann"
type: docs
weight: 10
url: /de/net/aspose.zip.lha/lhaarchive/lhaarchive/
---
## LhaArchive(Stream, LhaLoadOptions) {#constructor}

Initialisiert eine neue Instanz der [`LhaArchive`](../)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

```csharp
public LhaArchive(Stream sourceStream, LhaLoadOptions loadOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | Stream | Die Quelle des Archivs. |
| loadOptions | LhaLoadOptions | Optionen zum Laden eines vorhandenen Archivs. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *sourceStream* ist null |
| ArgumentException | *sourceStream* ist nicht suchbar. |
| InvalidDataException | Ungeeignete Daten gefunden. |
| EndOfStreamException | Wird ausgelöst, wenn das Ende des Streams erreicht wird, bevor die erwartete Anzahl von Bytes gelesen wurde. |
| ObjectDisposedException | Wird ausgelöst, wenn das Objekt bereits verworfen wurde. |

## Hinweise

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methode [`Extract`](../../lhaarchiveentry/extract/) zum Dekomprimieren.

### Siehe auch

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LhaArchive(string, LhaLoadOptions) {#constructor_1}

Initialisiert eine neue Instanz der [`LhaArchive`](../)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

```csharp
public LhaArchive(string path, LhaLoadOptions loadOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der vollständig qualifizierte oder relative Pfad zur Archivdatei. |
| loadOptions | LhaLoadOptions | Optionen zum Laden eines vorhandenen Archivs. |

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
| EndOfStreamException | Wird ausgelöst, wenn das Ende des Streams erreicht wird, bevor die erwartete Anzahl von Bytes gelesen wurde. |
| ObjectDisposedException | Wird ausgelöst, wenn das Objekt bereits verworfen wurde. |

## Hinweise

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methode [`Extract`](../../lhaarchiveentry/extract/) zum Dekomprimieren.

## Beispiele

Das folgende Beispiel extrahiert ein Archiv und dekomprimiert dann den ersten Eintrag in einen `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LhaArchive archive = new LhaArchive("sample.lzh"))
{
    archive.Entries[0].Extract(extracted);
}
```

### Siehe auch

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)


