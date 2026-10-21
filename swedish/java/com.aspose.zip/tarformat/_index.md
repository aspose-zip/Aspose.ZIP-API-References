---
title: "TarFormat"
second_title: "Aspose.ZIP för Java API-referens"
description: "Enumeration med stöd för format av ."
type: docs
weight: 169
url: /sv/java/com.aspose.zip/tarformat/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum TarFormat extends Enum<TarFormat>
```

Enumeration med stöd för format av [TarArchive](../../com.aspose.zip/tararchive).
## Fält

| Fält | Beskrivning |
| --- | --- |
| [Gnu](#Gnu) | GNU tar är baserad på det tidiga utkastet av POSIX.1. |
| [Pax](#Pax) | Format definierat i POSIX.1-2001-standarden. |
| [UsTar](#UsTar) | Formatet utökar headerblocket från v7-formatet. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Gnu {#Gnu}
```
public static final TarFormat Gnu
```


GNU tar är baserad på det tidiga utkastet av POSIX.1. Detta format implementeras som standard‑tar‑format i många Linux‑system.

### Pax {#Pax}
```
public static final TarFormat Pax
```


Format definierat i POSIX.1-2001-standarden.

### UsTar {#UsTar}
```
public static final TarFormat UsTar
```


Formatet utökar headerblocket från v7-formatet. Spritt och stöds i många verktyg för Windows.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static TarFormat valueOf(String name)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String |  |

**Returns:**
[TarFormat](../../com.aspose.zip/tarformat)
### values() {#values--}
```
public static TarFormat[] values()
```




**Returns:**
com.aspose.zip.TarFormat[]
