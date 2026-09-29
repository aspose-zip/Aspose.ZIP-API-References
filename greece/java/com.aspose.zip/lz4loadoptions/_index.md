---
title: "Lz4LoadOptions"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Επιλογές για τη φόρτωση ."
type: docs
weight: 82
url: /el/java/com.aspose.zip/lz4loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class Lz4LoadOptions
```

Επιλογές για τη φόρτωση του [Lz4Archive](../../com.aspose.zip/lz4archive).
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Lz4LoadOptions()](#Lz4LoadOptions--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Ορίζει μια σημαία ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής. |
### Lz4LoadOptions() {#Lz4LoadOptions--}
```
public Lz4LoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Ορίζει μια σημαία ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής.

Ακυρώστε την εξαγωγή του αρχείου lz4 μετά από κάποιο χρονικό διάστημα.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
Lz4LoadOptions options = new Lz4LoadOptions();
options.setCancellationFlag(cf);
try (Lz4Archive a = new Lz4Archive("big.lz4", options)) {
try {
a.extract("data.bin");
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

