---
title: "Classe AlzEntry"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Aspose.Zip.Alz.AlzEntry classe. Rappresenta una voce di file in un archivio ALZ con tutti i suoi metadati"
type: docs
weight: 30
url: /it/net/aspose.zip.alz/alzentry/
---
## AlzEntry class

Rappresenta una voce di file in un archivio ALZ con tutti i suoi metadati.

```csharp
public abstract class AlzEntry : IArchiveFileEntry
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
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract_1)(Stream, string) | Estrae la voce nello stream fornito. |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract)(string, string) | Estrae la voce nel file system usando il percorso fornito. |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | Apre la voce per l'estrazione e fornisce uno stream con il contenuto decompresso della voce. |

### Vedi anche

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


