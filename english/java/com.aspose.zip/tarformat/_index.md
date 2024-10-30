---
title: TarFormat
second_title: Aspose.ZIP for Java API Reference
description: Enumeration with supported formats of .
type: docs
weight: 124
url: /java/com.aspose.zip/tarformat/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum TarFormat extends Enum<TarFormat>
```

Enumeration with supported formats of [TarArchive](../../com.aspose.zip/tararchive).
## Fields

| Field | Description |
| --- | --- |
| [Gnu](#Gnu) | GNU tar is based on the early draft of POSIX.1. |
| [Pax](#Pax) | Format defined in POSIX.1-2001 standard. |
| [UsTar](#UsTar) | Format extends the header block from the v7 format. |
## Methods

| Method | Description |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Gnu {#Gnu}
```
public static final TarFormat Gnu
```


GNU tar is based on the early draft of POSIX.1. This format is implemented as default tar format in many Linux systems.

### Pax {#Pax}
```
public static final TarFormat Pax
```


Format defined in POSIX.1-2001 standard.

### UsTar {#UsTar}
```
public static final TarFormat UsTar
```


Format extends the header block from the v7 format. Widespread and supported in many utilities for Windows.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static TarFormat valueOf(String name)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[TarFormat](../../com.aspose.zip/tarformat)
### values() {#values--}
```
public static TarFormat[] values()
```




**Returns:**
com.aspose.zip.TarFormat[]
