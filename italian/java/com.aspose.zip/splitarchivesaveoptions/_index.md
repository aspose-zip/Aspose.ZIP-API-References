---
title: "SplitArchiveSaveOptions"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Opzioni per salvare un archivio ZIP multivolume."
type: docs
weight: 122
url: /it/java/com.aspose.zip/splitarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitArchiveSaveOptions
```

Opzioni per salvare un archivio ZIP multivolume.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SplitArchiveSaveOptions(String fileName, long segmentSize)](#SplitArchiveSaveOptions-java.lang.String-long-) | Istanzia le impostazioni per salvare un archivio ZIP multivolume. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Ottiene il commento opzionale per il file Zip. |
| [getCloseEntrySource()](#getCloseEntrySource--) | Ottiene un valore che indica se le sorgenti delle voci devono essere chiuse subito dopo che una voce è stata compressa. |
| [getEncoding()](#getEncoding--) | Ottiene la codifica per convertire i nomi dei file e altre stringhe in byte. |
| [getEventsBag()](#getEventsBag--) | Ottiene il contenitore degli eventi generati durante il salvataggio dell'archivio. |
| [getFileName()](#getFileName--) | Ottiene il nome dei segmenti senza estensione. |
| [getSegmentSize()](#getSegmentSize--) | Ottiene la dimensione del segmento. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Imposta il commento opzionale per il file Zip. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | Imposta un valore che indica se le sorgenti delle voci devono essere chiuse subito dopo che una voce è stata compressa. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Imposta la codifica per convertire i nomi dei file e altre stringhe in byte. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | Imposta il contenitore degli eventi generati durante il salvataggio dell'archivio. |
### SplitArchiveSaveOptions(String fileName, long segmentSize) {#SplitArchiveSaveOptions-java.lang.String-long-}
```
public SplitArchiveSaveOptions(String fileName, long segmentSize)
```


Istanzia le impostazioni per salvare un archivio ZIP multivolume.

Alcuni volumi possono essere inferiori a `segmentSize`. Nella maggior parte dei casi, l'ultimo segmento sarà più piccolo, ma raramente i segmenti regolari potrebbero esserlo.

I nomi dei file saranno i seguenti: `fileName`.z01, `fileName`.z02, ..., `fileName`.z(n-1), `fileName`.zip.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Nome per i volumi. Può includere o meno l'estensione .zip. |
| segmentSize | long | Dimensione del volume. |

### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Ottiene il commento opzionale per il file Zip.

**Returns:**
java.lang.String - commento opzionale per il file Zip.
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


Ottiene un valore che indica se le sorgenti delle voci devono essere chiuse subito dopo che una voce è stata compressa.

**Returns:**
boolean - un valore che indica se le sorgenti delle voci devono essere chiuse subito dopo che una voce è stata compressa.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Ottiene la codifica per convertire i nomi dei file e altre stringhe in byte.

Se non impostato, verrà utilizzata la code page 437.

**Returns:**
java.nio.charset.Charset - codifica per convertire i nomi dei file e altre stringhe in byte.
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


Ottiene il contenitore degli eventi generati durante il salvataggio dell'archivio.

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getFileName() {#getFileName--}
```
public final String getFileName()
```


Ottiene il nome dei segmenti senza estensione.

**Returns:**
java.lang.String - il nome dei segmenti senza estensione.
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Ottiene la dimensione del segmento.

**Returns:**
long - la dimensione del segmento.
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


Imposta il commento opzionale per il file Zip.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | commento opzionale per il file Zip. |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


Imposta un valore che indica se le sorgenti delle voci devono essere chiuse subito dopo che una voce è stata compressa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se le sorgenti delle voci devono essere chiuse subito dopo che una voce è stata compressa. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Imposta la codifica per convertire i nomi dei file e altre stringhe in byte.

Se non impostato, verrà utilizzata la code page 437.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.nio.charset.Charset | codifica per convertire i nomi dei file e altre stringhe in byte. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


Imposta il contenitore degli eventi generati durante il salvataggio dell'archivio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | contenitore degli eventi generati durante il salvataggio dell'archivio. |

