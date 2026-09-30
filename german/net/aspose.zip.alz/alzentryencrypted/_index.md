---
title: "Klasse AlzEntryEncrypted"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "Aspose.Zip.Alz.AlzEntryEncrypted Klasse. ALZ-Eintrag, der vor der Dekompression entschlüsselt werden muss"
type: docs
weight: 40
url: /de/net/aspose.zip.alz/alzentryencrypted/
---
## AlzEntryEncrypted class

ALZ-Eintrag, der vor der Dekompression entschlüsselt werden muss.

```csharp
public sealed class AlzEntryEncrypted : AlzEntry
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CompressedSize](../../aspose.zip.alz/alzentry/compressedsize/) { get; } | Komprimierte Größe der Dateidaten in Bytes. |
| [IsDirectory](../../aspose.zip.alz/alzentry/isdirectory/) { get; } | Gibt true zurück, wenn dieser Eintrag ein Verzeichnis darstellt. |
| [Length](../../aspose.zip.alz/alzentry/length/) { get; } |  |
| [Name](../../aspose.zip.alz/alzentry/name/) { get; } | Dateiname (ohne Pfad). |
| [UncompressedSize](../../aspose.zip.alz/alzentry/uncompressedsize/) { get; } | Unkomprimierte Größe der Dateidaten in Bytes. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Extract](../../aspose.zip.alz/alzentry/extract/)(Stream, string) | Extrahiert den Eintrag in den bereitgestellten Stream. |
| [Extract](../../aspose.zip.alz/alzentry/extract/)(string, string) | Extrahiert den Eintrag in das Dateisystem anhand des angegebenen Pfads. |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | Öffnet den Eintrag zum Extrahieren und liefert einen Stream mit dem dekomprimierten Eintragsinhalt. |

### Siehe auch

* class [AlzEntry](../alzentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


