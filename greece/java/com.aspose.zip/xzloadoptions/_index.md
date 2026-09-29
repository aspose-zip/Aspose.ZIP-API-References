---
title: "XzLoadOptions"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Επιλογές για τη φόρτωση ."
type: docs
weight: 152
url: /el/java/com.aspose.zip/xzloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class XzLoadOptions
```

Επιλογές για τη φόρτωση του [XzArchive](../../com.aspose.zip/xzarchive).

Στο .NET Framework 4.0 και άνω, μπορεί να χρησιμοποιηθεί για την ακύρωση της εξαγωγής.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [XzLoadOptions()](#XzLoadOptions--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Ορίζει μια σημαία ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής. |
### XzLoadOptions() {#XzLoadOptions--}
```
public XzLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Ορίζει μια σημαία ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής.

Ακύρωση εξαγωγής αρχείου lzip μετά από κάποιο χρονικό διάστημα.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
XzLoadOptions options = new XzLoadOptions();
options.setCancellationFlag(cf);
try (XzArchive a = new XzArchive("big.xz", options)) {
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

