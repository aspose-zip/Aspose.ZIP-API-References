---
title: "Klasse AppleArchiveEntry"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "Aspose.Zip.Apple.AppleArchiveEntry class. Stellt einen Dateisystemeintrag innerhalb eines AppleArchive dar"
type: docs
weight: 70
url: /de/net/aspose.zip.apple/applearchiveentry/
---
## AppleArchiveEntry class

Stellt einen Dateisystemeintrag innerhalb eines [`AppleArchive`](../applearchive/) dar.

```csharp
public sealed class AppleArchiveEntry : IArchiveFileEntry
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [IsDirectory](../../aspose.zip.apple/applearchiveentry/isdirectory/) { get; } | Gibt einen Wert zurück, der angibt, ob der Eintrag ein Verzeichnis darstellt. |
| [IsSymbolicLink](../../aspose.zip.apple/applearchiveentry/issymboliclink/) { get; } | Gibt einen Wert zurück, der angibt, ob der Eintrag einen symbolischen Link darstellt. |
| [Length](../../aspose.zip.apple/applearchiveentry/length/) { get; } | Gibt die unkomprimierte Länge des Eintrags in Bytes zurück. |
| [Name](../../aspose.zip.apple/applearchiveentry/name/) { get; } | Gibt den Pfad des Eintrags innerhalb des Archivs zurück. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract_1)(Stream) | Extrahiert den Eintrag in den bereitgestellten Stream. |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract)(string) | Extrahiert den Eintrag in das Dateisystem anhand des angegebenen Pfads. |
| [Open](../../aspose.zip.apple/applearchiveentry/open/)() | Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dem Eintragsinhalt bereit. |

## Hinweise

Eine Instanz dieser Klasse kann eine reguläre Datei, ein Verzeichnis oder einen symbolischen Link darstellen, die aus einem bestehenden Apple Archive geparst wurden, oder eine Datei bzw. ein Verzeichnis, das zu einem zu erstellenden Archiv hinzugefügt wird.

### Siehe auch

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


