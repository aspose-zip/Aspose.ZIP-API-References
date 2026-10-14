---
title: "ZstandardLoadOptions"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Optionen, mit denen  aus einer komprimierten Datei geladen wird."
type: docs
weight: 158
url: /de/java/com.aspose.zip/zstandardloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZstandardLoadOptions
```

Optionen, mit denen [ZstandardArchive](../../com.aspose.zip/zstandardarchive) aus einer komprimierten Datei geladen wird. Enthält ein Ereignis, das bei der Extraktion ausgelöst wird.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ZstandardLoadOptions()](#ZstandardLoadOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getExtractionProgressed()](#getExtractionProgressed--) | Gibt ein Ereignis zurück, das ausgelöst wird, wenn einige Bytes extrahiert wurden. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Setzt ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Setzt ein Ereignis, das ausgelöst wird, wenn einige Bytes extrahiert wurden. |
### ZstandardLoadOptions() {#ZstandardLoadOptions--}
```
public ZstandardLoadOptions()
```


### getExtractionProgressed() {#getExtractionProgressed--}
```
public Event<ProgressEventArgs> getExtractionProgressed()
```


Gibt ein Ereignis zurück, das ausgelöst wird, wenn einige Bytes extrahiert wurden.

```

``````

long length = 10_000_000;
ZStandardLoadOptions loadOptions = new ZStandardLoadOptions();
loadOptions.setExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / length);
});
ZstandardArchive archive = new ZstandardArchive("archive.zst", loadOptions);
 
```

Event sender is the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) instance which extraction is progressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel Zstandard archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         ZstandardLoadOptions options = new ZstandardLoadOptions();
         options.setCancellationFlag(cf);
         try (ZstandardArchive a = new ZstandardArchive("big.zstd", options)) {
             try {
                 a.extract("data.bin");
             } catch (OperationCanceledException e) {
                 System.out.println("Extraction was cancelled after 60 seconds");
             }
         }
     }
 
```

Ein Abbruch führt meistens dazu, dass einige Daten nicht extrahiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | Ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen. |

### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setExtractionProgressed(Event<ProgressEventArgs> value)
```


Setzt ein Ereignis, das ausgelöst wird, wenn einige Bytes extrahiert wurden.

```

``````

long length = 10_000_000;
ZStandardLoadOptions loadOptions = new ZStandardLoadOptions();
loadOptions.setExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / length);
});
ZstandardArchive archive = new ZstandardArchive("archive.zst", loadOptions);
 
```

Event sender is the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) instance which extraction is progressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when some bytes have been extracted |

