---
title: "XarLoadOptions"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Επιλογές με τις οποίες το αρχείο XAR φορτώνεται από ένα συμπιεσμένο αρχείο."
type: docs
weight: 142
url: /el/java/com.aspose.zip/xarloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class XarLoadOptions
```

Επιλογές με τις οποίες το αρχείο XAR φορτώνεται από ένα συμπιεσμένο αρχείο.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [XarLoadOptions()](#XarLoadOptions--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getEntryExtractionProgressed()](#getEntryExtractionProgressed--) | Λαμβάνει ένα συμβάν που ενεργοποιείται όταν έχουν εξαχθεί κάποια bytes. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Ορίζει μια σημαία ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής. |
| [setEntryExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Ορίζει ένα συμβάν που ενεργοποιείται όταν έχουν εξαχθεί κάποια bytes. |
### XarLoadOptions() {#XarLoadOptions--}
```
public XarLoadOptions()
```


### getEntryExtractionProgressed() {#getEntryExtractionProgressed--}
```
public final Event<ProgressEventArgs> getEntryExtractionProgressed()
```


Λαμβάνει ένα συμβάν που ενεργοποιείται όταν έχουν εξαχθεί κάποια bytes.

```

``````

XarLoadOptions loadOptions = new XarLoadOptions();
loadOptions.setEntryExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / ((XarFileEntry)sender).getLength());
});
XarArchive archive = new XarArchive("archive.xar", loadOptions);
 
```

Event sender is the [XarFileEntry](../../com.aspose.zip/xarfileentry) instance which extraction is progressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel XAR archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         XarLoadOptions options = new XarLoadOptions();
         options.setCancellationFlag(cf);
         try (XarArchive a = new XarArchive("big.xar", options)) {
             try {
                 ((XarFileEntry) a.getEntries().get(0)).extract("data.bin");
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

### setEntryExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setEntryExtractionProgressed(Event<ProgressEventArgs> value)
```


Ορίζει ένα συμβάν που ενεργοποιείται όταν έχουν εξαχθεί κάποια bytes.

```

``````

XarLoadOptions loadOptions = new XarLoadOptions();
loadOptions.setEntryExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / ((XarFileEntry)sender).getLength());
});
XarArchive archive = new XarArchive("archive.xar", loadOptions);
 
```

Event sender is the [XarFileEntry](../../com.aspose.zip/xarfileentry) instance which extraction is progressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when some bytes have been extracted |

