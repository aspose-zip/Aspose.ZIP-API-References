---
title: "Classe AlzEntryEncrypted"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Aspose.Zip.Alz.AlzEntryEncrypted classe. Voce ALZ che deve essere decrittata prima della decompressione"
type: docs
weight: 40
url: /it/net/aspose.zip.alz/alzentryencrypted/
---
## AlzEntryEncrypted class

Voce ALZ che deve essere decrittata prima della decompressione.

```csharp
public sealed class AlzEntryEncrypted : AlzEntry
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CompressedSize](../../aspose.zip.alz/alzentry/compressedsize/) { get; } | Dimensione compressa dei dati del file in byte. |
| [IsDirectory](../../aspose.zip.alz/alzentry/isdirectory/) { get; } | Restituisce true se questa voce rappresenta una directory. |
| [Length](../../aspose.zip.alz/alzentry/length/) { get; } |  |
| [Name](../../aspose.zip.alz/alzentry/name/) { get; } | Nome file (senza percorso). |
| [UncompressedSize](../../aspose.zip.alz/alzentry/uncompressedsize/) { get; } | Dimensione decompresso dei dati del file in byte. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Extract](../../aspose.zip.alz/alzentry/extract/)(Stream, string) | Estrae la voce nello stream fornito. |
| [Extract](../../aspose.zip.alz/alzentry/extract/)(string, string) | Estrae la voce nel file system usando il percorso fornito. |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | Apre la voce per l'estrazione e fornisce uno stream con il contenuto decompresso della voce. |

### Vedi anche

* class [AlzEntry](../alzentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


