---
title: "SplitSevenZipArchiveSaveOptions"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Opzioni per salvare un archivio 7-zip multivolume."
type: docs
weight: 123
url: /it/java/com.aspose.zip/splitsevenziparchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitSevenZipArchiveSaveOptions
```

Opzioni per salvare un archivio 7-zip multivolume.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)](#SplitSevenZipArchiveSaveOptions-java.lang.String-long-) | Istanzia le impostazioni per salvare un archivio 7z multi-volume. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getFileName()](#getFileName--) | Ottiene il nome dei segmenti senza estensione. |
| [getSegmentSize()](#getSegmentSize--) | Ottiene la dimensione del segmento. |
### SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize) {#SplitSevenZipArchiveSaveOptions-java.lang.String-long-}
```
public SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)
```


Istanzia le impostazioni per salvare un archivio 7z multi-volume.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | fileName | java.lang.String | nome per i volumi. Può essere con o senza estensione .7z. |

I nomi dei file saranno i seguenti: `fileName`.7z.001, `fileName`.7z.002, ..., `fileName`.7z.(n). |
|  | segmentSize | long | dimensione del volume. |

Alcuni volumi possono essere inferiori a `segmentSize`. Nella maggior parte dei casi, l'ultimo segmento sarà più piccolo, ma raramente i segmenti regolari potrebbero esserlo. |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Ottiene il nome dei segmenti senza estensione.

**Returns:**
java.lang.String - il nome dei segmenti senza estensione
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Ottiene la dimensione del segmento.

**Returns:**
long - la dimensione del segmento.
