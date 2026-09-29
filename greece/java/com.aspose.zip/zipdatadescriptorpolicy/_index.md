---
title: "ZipDataDescriptorPolicy"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Επιλογές για την παρουσία του Data Descriptor."
type: docs
weight: 171
url: /el/java/com.aspose.zip/zipdatadescriptorpolicy/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ZipDataDescriptorPolicy extends Enum<ZipDataDescriptorPolicy>
```

Επιλογές για την παρουσία του Data Descriptor.
## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
| [Always](#Always) | Το Data Descriptor είναι πάντα παρόν για όλες τις καταχωρήσεις zip. |
| [ForAllFileEntries](#ForAllFileEntries) | Το Data Descriptor υπάρχει μόνο για καταχωρήσεις με δεδομένα αρχείου· παραλείπεται για καταλόγους. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Always {#Always}
```
public static final ZipDataDescriptorPolicy Always
```


Το Data Descriptor είναι πάντα παρόν για όλες τις καταχωρήσεις zip.

### ForAllFileEntries {#ForAllFileEntries}
```
public static final ZipDataDescriptorPolicy ForAllFileEntries
```


Το Data Descriptor υπάρχει μόνο για καταχωρήσεις με δεδομένα αρχείου· παραλείπεται για καταλόγους. Η χρήση αυτής της επιλογής δεν συνιστάται.

Μπορεί να εφαρμοστεί μόνο σε μη κρυπτογραφημένα αρχεία.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ZipDataDescriptorPolicy valueOf(String name)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String |  |

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy)
### values() {#values--}
```
public static ZipDataDescriptorPolicy[] values()
```




**Returns:**
com.aspose.zip.ZipDataDescriptorPolicy[]
