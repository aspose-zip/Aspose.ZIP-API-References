---
title: "TarFormat"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Απαρίθμηση με υποστηριζόμενες μορφές του ."
type: docs
weight: 169
url: /el/java/com.aspose.zip/tarformat/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum TarFormat extends Enum<TarFormat>
```

Απαρίθμηση με υποστηριζόμενες μορφές του [TarArchive](../../com.aspose.zip/tararchive).
## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
| [Gnu](#Gnu) | Το GNU tar βασίζεται στο πρώιμο προσχέδιο του POSIX.1. |
| [Pax](#Pax) | Μορφή ορισμένη στο πρότυπο POSIX.1-2001. |
| [UsTar](#UsTar) | Η μορφή επεκτείνει το μπλοκ κεφαλίδας από τη μορφή v7. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Gnu {#Gnu}
```
public static final TarFormat Gnu
```


Το GNU tar βασίζεται στο πρώιμο προσχέδιο του POSIX.1. Αυτή η μορφή υλοποιείται ως προεπιλεγμένη μορφή tar σε πολλά συστήματα Linux.

### Pax {#Pax}
```
public static final TarFormat Pax
```


Μορφή ορισμένη στο πρότυπο POSIX.1-2001.

### UsTar {#UsTar}
```
public static final TarFormat UsTar
```


Η μορφή επεκτείνει το μπλοκ κεφαλίδας από τη μορφή v7. Είναι διαδεδομένη και υποστηρίζεται σε πολλές βοηθητικές εφαρμογές για Windows.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static TarFormat valueOf(String name)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String |  |

**Returns:**
[TarFormat](../../com.aspose.zip/tarformat)
### values() {#values--}
```
public static TarFormat[] values()
```




**Returns:**
com.aspose.zip.TarFormat[]
