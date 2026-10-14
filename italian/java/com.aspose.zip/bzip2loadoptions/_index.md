---
title: "Bzip2LoadOptions"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Opzioni per il caricamento ."
type: docs
weight: 42
url: /it/java/com.aspose.zip/bzip2loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class Bzip2LoadOptions
```

Opzioni per il caricamento di [Bzip2Archive](../../com.aspose.zip/bzip2archive). Contiene l'evento generato durante l'estrazione.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Bzip2LoadOptions()](#Bzip2LoadOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getExtractionProgressed()](#getExtractionProgressed--) | Ottiene un evento che viene generato quando alcuni byte sono stati estratti. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Imposta un flag di cancellazione usato per annullare l'operazione di estrazione. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Imposta un evento che viene generato quando alcuni byte sono stati estratti. |
### Bzip2LoadOptions() {#Bzip2LoadOptions--}
```
public Bzip2LoadOptions()
```


### getExtractionProgressed() {#getExtractionProgressed--}
```
public Event<ProgressEventArgs> getExtractionProgressed()
```


Ottiene un evento che viene generato quando alcuni byte sono stati estratti.

```

``````

int[] percent = { 0 };
long originalFileLength = 10_000_000;

Bzip2LoadOptions loadOptions = new Bzip2LoadOptions();
loadOptions.setExtractionProgressed((sender, args) -> {
percent[0] = (int)((100 * (double)args.getProceededBytes()) / originalFileLength);
});
 
```

Event sender is the [Bzip2Archive](../../com.aspose.zip/bzip2archive) instance which extraction is progressed. The `ProgressEventArgs.getProceededBytes()`([ProgressEventArgs.getProceededBytes()](../../com.aspose.zip/progresseventargs\#getProceededBytes--)) is the number of bytes after extraction.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel Bzip2 archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         Bzip2LoadOptions options = new Bzip2LoadOptions();
         options.setCancellationFlag(cf);
         try (Bzip2Archive a = new Bzip2Archive("big.bz2", options)) {
             try {
                 a.extract("data.bin");
             } catch (OperationCanceledException e) {
                 System.out.println("Extraction was cancelled after 60 seconds");
             }
         }
     }
 
```

La cancellazione di solito comporta che alcuni dati non vengano estratti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | un flag di cancellazione utilizzato per annullare l'operazione di estrazione. |

### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setExtractionProgressed(Event<ProgressEventArgs> value)
```


Imposta un evento che viene generato quando alcuni byte sono stati estratti.

```

``````

int[] percent = { 0 };
long originalFileLength = 10_000_000;

Bzip2LoadOptions loadOptions = new Bzip2LoadOptions();
loadOptions.setExtractionProgressed((sender, args) -> {
percent[0] = (int)((100 * (double)args.getProceededBytes()) / originalFileLength);
});
 
```

Event sender is the [Bzip2Archive](../../com.aspose.zip/bzip2archive) instance which extraction is progressed. The `ProgressEventArgs.getProceededBytes()`([ProgressEventArgs.getProceededBytes()](../../com.aspose.zip/progresseventargs\#getProceededBytes--)) is the number of bytes after extraction.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when some bytes have been extracted |

