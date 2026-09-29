---
title: "LzxLoadOptions"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Επιλογές με τις οποίες το αρχείο φορτώνεται από ένα συμπιεσμένο αρχείο."
type: docs
weight: 91
url: /el/java/com.aspose.zip/lzxloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LzxLoadOptions
```

Επιλογές με τις οποίες το αρχείο φορτώνεται από ένα συμπιεσμένο αρχείο.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [LzxLoadOptions()](#LzxLoadOptions--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Ορίζει μια σημαία ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής. |
### LzxLoadOptions() {#LzxLoadOptions--}
```
public LzxLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Ορίζει μια σημαία ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής.

Ακύρωση εξαγωγής αρχείου ISO μετά από ορισμένο χρόνο.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
LzxLoadOptions options = new LzxLoadOptions();
options.setCancellationFlag(cf);
try (LzxArchive a = new LzxArchive("big.lzx", options)) {
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

