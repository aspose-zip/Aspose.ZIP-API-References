---
title: "AppleArchiveEntry.Open"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "AppleArchiveEntry-Methode. Öffnet den Eintrag zum Extrahieren und liefert einen Stream mit dem Eintragsinhalt"
type: docs
weight: 60
url: /de/net/aspose.zip.apple/applearchiveentry/open/
---
## AppleArchiveEntry.Open method

Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dem Eintragsinhalt bereit.

```csharp
public Stream Open()
```

### Rückgabewert

Ein lesbarer Stream, der die extrahierten Eintragsdaten enthält.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| NotSupportedException | Der Eintrag gehört zu einem solid Apple Archive oder verwendet ein nicht unterstütztes Kompressionsverfahren. |
| InvalidDataException | Die für den Eintrag gespeicherte Prüfsumme oder der Digest stimmt nicht mit den extrahierten Daten überein. |
| InvalidOperationException | Der Eintrag gehört zu einem für die Zusammensetzung vorbereiteten Archiv, oder die Eintragsdaten können nicht aus einem nicht durchsuchbaren Archivstream geöffnet werden. |
| ObjectDisposedException | Der Quellstream wurde freigegeben. |
| IOException | Ein I/O-Fehler ist aufgetreten. |

## Hinweise

Lesen Sie aus dem zurückgegebenen Stream, um den ursprünglichen Eintragsinhalt zu erhalten. Wenn das Archiv Prüfsummenfelder enthält, wird die Prüfsumme beim Lesen des zurückgegebenen Streams verifiziert.

### Siehe auch

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


