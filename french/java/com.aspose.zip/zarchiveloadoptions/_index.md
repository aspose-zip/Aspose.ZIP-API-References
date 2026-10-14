---
title: "ZArchiveLoadOptions"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Options avec lesquelles  est chargé depuis un fichier compressé."
type: docs
weight: 154
url: /fr/java/com.aspose.zip/zarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZArchiveLoadOptions
```

Options avec lesquelles [ZArchive](../../com.aspose.zip/zarchive) est chargé à partir d'un fichier compressé. Contient l'événement déclenché lors de l'extraction.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ZArchiveLoadOptions()](#ZArchiveLoadOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getExtractionProgressed()](#getExtractionProgressed--) | Obtient un événement qui est déclenché lorsque des octets ont été extraits. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Définit un drapeau d'annulation utilisé pour annuler l'opération d'extraction. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Définit un événement qui est déclenché lorsque des octets ont été extraits. |
### ZArchiveLoadOptions() {#ZArchiveLoadOptions--}
```
public ZArchiveLoadOptions()
```


### getExtractionProgressed() {#getExtractionProgressed--}
```
public Event<ProgressEventArgs> getExtractionProgressed()
```


Obtient un événement qui est déclenché lorsque des octets ont été extraits.

```

``````

long length = 10_000_000;
ZArchiveLoadOptions loadOptions = new ZArchiveLoadOptions();
loadOptions.setExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / length);
});
ZArchive archive = new ZArchive("archive.z", loadOptions);
 
```

Event sender is the [ZArchive](../../com.aspose.zip/zarchive) instance which extraction is progressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel Z archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         ZArchiveLoadOptions options = new ZArchiveLoadOptions();
         options.setCancellationFlag(cf);
         try (ZArchive a = new ZArchive("big.z", options)) {
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

long length = 10_000_000;
ZArchiveLoadOptions loadOptions = new ZArchiveLoadOptions();
loadOptions.setExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / length);
});
ZArchive archive = new ZArchive("archive.z", loadOptions);
 
```

Event sender is the [ZArchive](../../com.aspose.zip/zarchive) instance which extraction is progressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when some bytes have been extracted |

