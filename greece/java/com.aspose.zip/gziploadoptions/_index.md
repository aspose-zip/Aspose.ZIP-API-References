---
title: "GzipLoadOptions"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Επιλογές για τη φόρτωση ."
type: docs
weight: 70
url: /el/java/com.aspose.zip/gziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GzipLoadOptions
```

Επιλογές για τη φόρτωση [GzipArchive](../../com.aspose.zip/gziparchive).

Στο .NET Framework 4.0 και άνω, μπορεί να χρησιμοποιηθεί για την ακύρωση της εξαγωγής.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [GzipLoadOptions()](#GzipLoadOptions--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getParseHeader()](#getParseHeader--) | Λαμβάνει την τιμή που υποδεικνύει εάν θα γίνει ανάλυση της κεφαλίδας της ροής για να προσδιοριστούν οι ιδιότητες, συμπεριλαμβανομένου του ονόματος. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Ορίζει μια σημαία ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής. |
| [setParseHeader(boolean value)](#setParseHeader-boolean-) | Ορίζει την τιμή που υποδεικνύει εάν θα γίνει ανάλυση της κεφαλίδας της ροής για να προσδιοριστούν οι ιδιότητες, συμπεριλαμβανομένου του ονόματος. |
### GzipLoadOptions() {#GzipLoadOptions--}
```
public GzipLoadOptions()
```


### getParseHeader() {#getParseHeader--}
```
public final boolean getParseHeader()
```


Λαμβάνει την τιμή που υποδεικνύει εάν θα γίνει ανάλυση της κεφαλίδας της ροής για να προσδιοριστούν οι ιδιότητες, συμπεριλαμβανομένου του ονόματος. Έχει νόημα μόνο για ροή με δυνατότητα αναζήτησης.

**Returns:**
boolean - η τιμή που υποδεικνύει εάν θα γίνει ανάλυση της κεφαλίδας της ροής για να προσδιοριστούν οι ιδιότητες, συμπεριλαμβανομένου του ονόματος.
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Ορίζει μια σημαία ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής.

Ακυρώστε την εξαγωγή του gzip αρχείου μετά από κάποιο χρονικό διάστημα.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
GzipLoadOptions options = new GzipLoadOptions();
options.setCancellationFlag(cf);
try (GzipArchive a = new GzipArchive("big.gz", options)) {
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

### setParseHeader(boolean value) {#setParseHeader-boolean-}
```
public final void setParseHeader(boolean value)
```


Sets the value indicating whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | the value indicating whether to parse stream header to figure out properties, including name. |

