---
title: "AppleArchive.AppleArchive"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "AppleArchive-Konstruktor. Initialisiert eine neue Instanz der AppleArchive-Klasse mit Einstellungen, die für zusammengesetzte Einträge verwendet werden."
type: docs
weight: 10
url: /de/net/aspose.zip.apple/applearchive/applearchive/
---
## AppleArchive(AppleArchiveEntrySettings) {#constructor}

Initialisiert eine neue Instanz der [`AppleArchive`](../)-Klasse mit Einstellungen, die für zusammengesetzte Einträge verwendet werden.

```csharp
public AppleArchive(AppleArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| newEntrySettings | AppleArchiveEntrySettings | Einstellungen, die beim Erstellen eines neuen Apple Archive verwendet werden. |

### Siehe auch

* class [AppleArchiveEntrySettings](../../applearchiveentrysettings/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(Stream, AppleArchiveLoadOptions) {#constructor_1}

Initialisiert eine neue Instanz der [`AppleArchive`](../)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

```csharp
public AppleArchive(Stream sourceStream, AppleArchiveLoadOptions loadOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | Stream | Die Quelle des Archivs. |
| loadOptions | AppleArchiveLoadOptions | Optionen zum Laden eines vorhandenen Archivs. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *sourceStream* ist null. |
| ArgumentException | *sourceStream* ist nicht suchbar. |
| InvalidDataException | *sourceStream* ist kein gültiges Apple Archive. |
| EndOfStreamException | Der Stream endet unerwartet während des Parsens der Archiveinträge. |

## Hinweise

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methoden [`ExtractToDirectory`](../extracttodirectory/) und [`Open`](../../applearchiveentry/open/) zum Dekomprimieren.

### Siehe auch

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(string, AppleArchiveLoadOptions) {#constructor_2}

Initialisiert eine neue Instanz der [`AppleArchive`](../)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

```csharp
public AppleArchive(string path, AppleArchiveLoadOptions loadOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der vollständig qualifizierte oder relative Pfad zur Archivdatei. |
| loadOptions | AppleArchiveLoadOptions | Optionen zum Laden eines vorhandenen Archivs. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *path* ist null. |
| FileNotFoundException | Die Datei wurde nicht gefunden. |
| InvalidDataException | *path* ist kein gültiges Apple Archive. |
| EndOfStreamException | Der Stream endet unerwartet während des Parsens der Archiveinträge. |

## Hinweise

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methoden [`ExtractToDirectory`](../extracttodirectory/) und [`Open`](../../applearchiveentry/open/) zum Dekomprimieren.

### Siehe auch

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


