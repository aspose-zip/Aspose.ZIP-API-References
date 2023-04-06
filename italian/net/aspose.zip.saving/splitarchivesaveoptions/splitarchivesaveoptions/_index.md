---
title: SplitArchiveSaveOptions.SplitArchiveSaveOptions
second_title: Riferimento API Aspose.ZIP per .NET
description: SplitArchiveSaveOptions costruttore. Crea unistanza delle impostazioni per il salvataggio di un archivio zip multivolume.
type: docs
weight: 10
url: /it/net/aspose.zip.saving/splitarchivesaveoptions/splitarchivesaveoptions/
---
## SplitArchiveSaveOptions constructor

Crea un'istanza delle impostazioni per il salvataggio di un archivio zip multivolume.

```csharp
public SplitArchiveSaveOptions(string fileName, uint segmentSize)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | String | Nome per volumi. Può essere con o senza estensione .zip. |
| segmentSize | UInt32 | Dimensione del volume. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentOutOfRangeException | La dimensione del segmento è inferiore a 65536 byte. |

### Osservazioni

Alcuni volumi potrebbero essere inferiori a*segmentSize*. Nella maggior parte dei casi l'ultimo segmento sarà inferiore, ma raramente potrebbero esserlo anche i segmenti regolari.

I nomi dei file saranno i seguenti:*fileName* .z01,*fileName* .z02, ...,*fileName* .z(n-1),*fileName*.cerniera lampo.

### Guarda anche

* class [SplitArchiveSaveOptions](../)
* spazio dei nomi [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* assemblea [Aspose.Zip](../../../)


