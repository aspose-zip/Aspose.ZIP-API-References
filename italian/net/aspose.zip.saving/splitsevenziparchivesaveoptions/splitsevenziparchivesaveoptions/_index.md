---
title: SplitSevenZipArchiveSaveOptions.SplitSevenZipArchiveSaveOptions
second_title: Riferimento API Aspose.ZIP per .NET
description: SplitSevenZipArchiveSaveOptions costruttore. Crea unistanza delle impostazioni per il salvataggio di un archivio 7z multivolume.
type: docs
weight: 10
url: /it/net/aspose.zip.saving/splitsevenziparchivesaveoptions/splitsevenziparchivesaveoptions/
---
## SplitSevenZipArchiveSaveOptions constructor

Crea un'istanza delle impostazioni per il salvataggio di un archivio 7z multivolume.

```csharp
public SplitSevenZipArchiveSaveOptions(string fileName, uint segmentSize)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | String | Nome per volumi. Può essere con o senza estensione .7z. |
| segmentSize | UInt32 | Dimensione del volume. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentOutOfRangeException | *segmentSize* è inferiore a 100. |

### Osservazioni

Alcuni volumi potrebbero essere inferiori a*segmentSize*. Nella maggior parte dei casi l'ultimo segmento sarà inferiore, ma raramente potrebbero esserlo anche i segmenti regolari.

I nomi dei file saranno i seguenti:*fileName* .7z.001,*fileName* .7z.002, ...,*fileName*.7z.(n).

### Guarda anche

* class [SplitSevenZipArchiveSaveOptions](../)
* spazio dei nomi [Aspose.Zip.Saving](../../splitsevenziparchivesaveoptions/)
* assemblea [Aspose.Zip](../../../)


