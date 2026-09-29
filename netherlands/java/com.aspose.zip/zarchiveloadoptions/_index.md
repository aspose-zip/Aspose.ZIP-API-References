---
title: "ZArchiveLoadOptions"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Opties waarmee  wordt geladen uit een gecomprimeerd bestand."
type: docs
weight: 154
url: /nl/java/com.aspose.zip/zarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZArchiveLoadOptions
```

Opties waarmee [ZArchive](../../com.aspose.zip/zarchive) wordt geladen vanuit een gecomprimeerd bestand. Bevat een gebeurtenis die wordt opgewekt bij het uitpakken.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ZArchiveLoadOptions()](#ZArchiveLoadOptions--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getExtractionProgressed()](#getExtractionProgressed--) | Haalt een gebeurtenis op die wordt geactiveerd wanneer enkele bytes zijn geëxtraheerd. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Stelt een annuleringsvlag in die wordt gebruikt om de extractie‑bewerking te annuleren. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Stelt een gebeurtenis in die wordt geactiveerd wanneer enkele bytes zijn geëxtraheerd. |
### ZArchiveLoadOptions() {#ZArchiveLoadOptions--}
```
public ZArchiveLoadOptions()
```


### getExtractionProgressed() {#getExtractionProgressed--}
```
public Event<ProgressEventArgs> getExtractionProgressed()
```


Haalt een gebeurtenis op die wordt geactiveerd wanneer enkele bytes zijn geëxtraheerd.

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

Annulering resulteert meestal in het niet extraheren van sommige gegevens.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | een annuleringsvlag die wordt gebruikt om de extractie‑operatie te annuleren. |

### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setExtractionProgressed(Event<ProgressEventArgs> value)
```


Stelt een gebeurtenis in die wordt geactiveerd wanneer enkele bytes zijn geëxtraheerd.

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

