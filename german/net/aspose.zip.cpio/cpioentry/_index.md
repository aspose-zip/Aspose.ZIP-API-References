---
title: Class CpioEntry
second_title: Aspose.ZIP für .NET-API-Referenz
description: Aspose.Zip.Cpio.CpioEntry klas. Stellt eine einzelne Datei im cpioArchiv dar.
type: docs
weight: 170
url: /de/net/aspose.zip.cpio/cpioentry/
---
## CpioEntry class

Stellt eine einzelne Datei im cpio-Archiv dar.

```csharp
public sealed class CpioEntry : IArchiveFileEntry
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [IsDirectory](../../aspose.zip.cpio/cpioentry/isdirectory/) { get; } | Ruft einen Wert ab, der angibt, ob der Eintrag ein Verzeichnis darstellt. |
| [LastWriteTimeUtc](../../aspose.zip.cpio/cpioentry/lastwritetimeutc/) { get; } | Ruft die letzte Schreibzeit ab. |
| [Length](../../aspose.zip.cpio/cpioentry/length/) { get; } | Liefert die Länge des Eintrags in Bytes. |
| [Name](../../aspose.zip.cpio/cpioentry/name/) { get; } | Ruft den Namen des Eintrags im Archiv ab. |
| [Parent](../../aspose.zip.cpio/cpioentry/parent/) { get; } | Ruft das Archiv ab, zu dem der Eintrag gehört. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Extract](../../aspose.zip.cpio/cpioentry/extract/#extract_1)(Stream) | Extrahiert den Eintrag zum bereitgestellten Stream. |
| [Extract](../../aspose.zip.cpio/cpioentry/extract/#extract)(string) | Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad. |
| [Open](../../aspose.zip.cpio/cpioentry/open/)() | Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit Eintragsinhalt bereit. |
| override [ToString](../../aspose.zip.cpio/cpioentry/tostring/)() |  |

### Siehe auch

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namensraum [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* Montage [Aspose.Zip](../../)


