---
title: "GzipLoadOptions"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Opzioni per il caricamento ."
type: docs
weight: 70
url: /it/java/com.aspose.zip/gziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GzipLoadOptions
```

Opzioni per il caricamento [GzipArchive](../../com.aspose.zip/gziparchive).

Nel .NET Framework 4.0 e versioni successive, può essere usato per annullare l'estrazione.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [GzipLoadOptions()](#GzipLoadOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getParseHeader()](#getParseHeader--) | Restituisce il valore che indica se analizzare l'intestazione del flusso per determinare le proprietà, incluso il nome. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Imposta un flag di cancellazione usato per annullare l'operazione di estrazione. |
| [setParseHeader(boolean value)](#setParseHeader-boolean-) | Imposta il valore che indica se analizzare l'intestazione del flusso per determinare le proprietà, incluso il nome. |
### GzipLoadOptions() {#GzipLoadOptions--}
```
public GzipLoadOptions()
```


### getParseHeader() {#getParseHeader--}
```
public final boolean getParseHeader()
```


Restituisce il valore che indica se analizzare l'intestazione del flusso per determinare le proprietà, incluso il nome. Ha senso solo per flussi ricercabili.

**Returns:**
boolean - il valore che indica se analizzare l'intestazione del flusso per determinare le proprietà, incluso il nome.
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Imposta un flag di cancellazione usato per annullare l'operazione di estrazione.

Annulla l'estrazione dell'archivio gzip dopo un certo periodo di tempo.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
GzipLoadOptions options = new GzipLoadOptions();
options.setCancellationFlag(cf);
try (GzipArchive a = new GzipArchive("big.gz", options)) {
try {
a.extract("data.bin");
} catch (OperationCanceledException e) {
System.out.println("L'estrazione è stata annullata dopo 60 secondi");
}
}
}
 
```

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

### setParseHeader(boolean value) {#setParseHeader-boolean-}
```
public final void setParseHeader(boolean value)
```


Sets the value indicating whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | the value indicating whether to parse stream header to figure out properties, including name. |

