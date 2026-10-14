---
title: "Bzip2LoadOptions"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Options de chargement ."
type: docs
weight: 42
url: /fr/java/com.aspose.zip/bzip2loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class Bzip2LoadOptions
```

Options de chargement de [Bzip2Archive](../../com.aspose.zip/bzip2archive). Contient l'événement déclenché lors de l'extraction.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Bzip2LoadOptions()](#Bzip2LoadOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getExtractionProgressed()](#getExtractionProgressed--) | Obtient un événement qui est déclenché lorsque des octets ont été extraits. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Définit un drapeau d'annulation utilisé pour annuler l'opération d'extraction. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Définit un événement qui est déclenché lorsque des octets ont été extraits. |
### Bzip2LoadOptions() {#Bzip2LoadOptions--}
```
public Bzip2LoadOptions()
```


### getExtractionProgressed() {#getExtractionProgressed--}
```
public Event<ProgressEventArgs> getExtractionProgressed()
```


Obtient un événement qui est déclenché lorsque des octets ont été extraits.

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

L'annulation entraîne généralement que certaines données ne sont pas extraites.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | un indicateur d'annulation utilisé pour annuler l'opération d'extraction. |

### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setExtractionProgressed(Event<ProgressEventArgs> value)
```


Définit un événement qui est déclenché lorsque des octets ont été extraits.

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

