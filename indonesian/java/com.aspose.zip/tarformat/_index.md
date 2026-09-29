---
title: "TarFormat"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Enumerasi dengan format yang didukung dari ."
type: docs
weight: 169
url: /id/java/com.aspose.zip/tarformat/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum TarFormat extends Enum<TarFormat>
```

Enumerasi dengan format yang didukung dari [TarArchive](../../com.aspose.zip/tararchive).
## Fields

| Field | Deskripsi |
| --- | --- |
| [Gnu](#Gnu) | GNU tar didasarkan pada draf awal POSIX.1. |
| [Pax](#Pax) | Format didefinisikan dalam standar POSIX.1-2001. |
| [UsTar](#UsTar) | Format memperluas blok header dari format v7. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Gnu {#Gnu}
```
public static final TarFormat Gnu
```


GNU tar didasarkan pada draf awal POSIX.1. Format ini diimplementasikan sebagai format tar default di banyak sistem Linux.

### Pax {#Pax}
```
public static final TarFormat Pax
```


Format didefinisikan dalam standar POSIX.1-2001.

### UsTar {#UsTar}
```
public static final TarFormat UsTar
```


Format memperluas blok header dari format v7. Banyak tersebar dan didukung dalam banyak utilitas untuk Windows.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static TarFormat valueOf(String name)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String |  |

**Returns:**
[TarFormat](../../com.aspose.zip/tarformat)
### values() {#values--}
```
public static TarFormat[] values()
```




**Returns:**
com.aspose.zip.TarFormat[]
