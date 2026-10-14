---
title: "ZstandardLoadOptions"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Επιλογές με τις οποίες  φορτώνεται από ένα συμπιεσμένο αρχείο."
type: docs
weight: 158
url: /el/java/com.aspose.zip/zstandardloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZstandardLoadOptions
```

Επιλογές με τις οποίες το [ZstandardArchive](../../com.aspose.zip/zstandardarchive) φορτώνεται από ένα συμπιεσμένο αρχείο. Περιέχει το συμβάν που ενεργοποιείται κατά την εξαγωγή.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ZstandardLoadOptions()](#ZstandardLoadOptions--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getExtractionProgressed()](#getExtractionProgressed--) | Λαμβάνει ένα συμβάν που ενεργοποιείται όταν έχουν εξαχθεί κάποια bytes. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Ορίζει μια σημαία ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Ορίζει ένα συμβάν που ενεργοποιείται όταν έχουν εξαχθεί κάποια bytes. |
### ZstandardLoadOptions() {#ZstandardLoadOptions--}
```
public ZstandardLoadOptions()
```


### getExtractionProgressed() {#getExtractionProgressed--}
```
public Event<ProgressEventArgs> getExtractionProgressed()
```


Λαμβάνει ένα συμβάν που ενεργοποιείται όταν έχουν εξαχθεί κάποια bytes.

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

Η ακύρωση συνήθως οδηγεί σε μη εξαγόμενα κάποια δεδομένα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | μια σημαία ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής. |

### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setExtractionProgressed(Event<ProgressEventArgs> value)
```


Ορίζει ένα συμβάν που ενεργοποιείται όταν έχουν εξαχθεί κάποια bytes.

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

