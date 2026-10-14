---
title: "LhaLoadOptions"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Επιλογές με τις οποίες το αρχείο φορτώνεται από ένα συμπιεσμένο αρχείο."
type: docs
weight: 78
url: /el/java/com.aspose.zip/lhaloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LhaLoadOptions
```

Επιλογές με τις οποίες το αρχείο φορτώνεται από ένα συμπιεσμένο αρχείο.

Στο .NET Framework 4.0 και άνω, μπορεί να χρησιμοποιηθεί για την ακύρωση της εξαγωγής.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [LhaLoadOptions()](#LhaLoadOptions--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Ορίζει μια σημαία ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής. |
### LhaLoadOptions() {#LhaLoadOptions--}
```
public LhaLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Ορίζει μια σημαία ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής.

Ακύρωση εξαγωγής αρχείου LHA μετά από κάποιο χρονικό διάστημα.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
LhaLoadOptions options = new LhaLoadOptions();
options.setCancellationFlag(cf);
try (LhaArchive a = new LhaArchive("big.lha", options)) {
try {
a.getEntries().get(0).extract("data.bin");
} catch (OperationCanceledException e) {
System.out.println("Η εξαγωγή ακυρώθηκε μετά από 60 δευτερόλεπτα");
}
}
}
 
```

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

