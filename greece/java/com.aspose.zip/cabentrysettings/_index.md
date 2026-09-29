---
title: "CabEntrySettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις που ελέγχουν πώς γράφεται μια καταχώρηση CAB."
type: docs
weight: 47
url: /el/java/com.aspose.zip/cabentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class CabEntrySettings
```

Ρυθμίσεις που ελέγχουν πώς γράφεται μια καταχώρηση CAB.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [CabEntrySettings(CabCompressionSettings compressionSettings)](#CabEntrySettings-com.aspose.zip.CabCompressionSettings-) | Αρχικοποιεί τις ρυθμίσεις με ένα συγκεκριμένο προφίλ συμπίεσης. |
| [CabEntrySettings()](#CabEntrySettings--) | Αρχικοποιεί τις ρυθμίσεις με την προεπιλεγμένη συμπίεση MSZip. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | Λαμβάνει τη διαμόρφωση συμπίεσης που εφαρμόζεται στην καταχώρηση. |
### CabEntrySettings(CabCompressionSettings compressionSettings) {#CabEntrySettings-com.aspose.zip.CabCompressionSettings-}
```
public CabEntrySettings(CabCompressionSettings compressionSettings)
```


Αρχικοποιεί τις ρυθμίσεις με ένα συγκεκριμένο προφίλ συμπίεσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | compressionSettings | [CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) | Ρυθμίσεις συμπίεσης προς χρήση. |

Μπορεί να είναι ένα από τα παρακάτω: |

### CabEntrySettings() {#CabEntrySettings--}
```
public CabEntrySettings()
```


Αρχικοποιεί τις ρυθμίσεις με την προεπιλεγμένη συμπίεση MSZip.

### getCompressionSettings() {#getCompressionSettings--}
```
public final CabCompressionSettings getCompressionSettings()
```


Λαμβάνει τη διαμόρφωση συμπίεσης που εφαρμόζεται στην καταχώρηση.

Μπορεί να είναι ένα από τα παρακάτω:

 *  

**Returns:**
[CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) - the compression configuration applied to the entry.
