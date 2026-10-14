---
title: "AppleArchiveEntry.Extract"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "AppleArchiveEntry-Methode. Extrahiert den Eintrag in das Dateisystem anhand des angegebenen Pfads"
type: docs
weight: 50
url: /de/net/aspose.zip.apple/applearchiveentry/extract/
---
## Extract(string) {#extract}

Extrahiert den Eintrag in das Dateisystem anhand des angegebenen Pfads.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | Der Pfad zur Zieldatei. Wenn die Datei bereits existiert, wird sie überschrieben. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| InvalidDataException | Die für den Eintrag gespeicherte Prüfsumme oder der Digest stimmt nicht mit den extrahierten Daten überein. |
| InvalidOperationException | Der Eintrag gehört zu einem für die Zusammensetzung vorbereiteten Archiv, oder die Eintragsdaten können nicht aus einem nicht durchsuchbaren Archivstream geöffnet werden. |
| NotSupportedException | Der Eintrag gehört zu einem solid Apple Archive oder verwendet ein nicht unterstütztes Kompressionsverfahren. |
| ObjectDisposedException | Der Quellstream wurde freigegeben. |
| IOException | Ein I/O-Fehler ist aufgetreten. |

### Siehe auch

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extrahiert den Eintrag in den bereitgestellten Stream.

```csharp
public void Extract(Stream destination)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ziel | Stream | Ziel-Stream. Muss beschreibbar sein. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *destination* ist `null`. |
| ArgumentException | *destination* unterstützt das Schreiben nicht. |
| InvalidDataException | Die für den Eintrag gespeicherte Prüfsumme oder der Digest stimmt nicht mit den extrahierten Daten überein. |
| InvalidOperationException | Der Eintrag gehört zu einem für die Zusammensetzung vorbereiteten Archiv, oder die Eintragsdaten können nicht aus einem nicht durchsuchbaren Archivstream geöffnet werden. |
| NotSupportedException | Der Eintrag gehört zu einem solid Apple Archive oder verwendet ein nicht unterstütztes Kompressionsverfahren. |
| ObjectDisposedException | Der Quellstream wurde freigegeben. |
| IOException | Ein I/O-Fehler ist aufgetreten. |

### Siehe auch

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


