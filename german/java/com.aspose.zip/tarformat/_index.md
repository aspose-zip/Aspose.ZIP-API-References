---
title: "TarFormat"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Aufzählung der unterstützten Formate von ."
type: docs
weight: 169
url: /de/java/com.aspose.zip/tarformat/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum TarFormat extends Enum<TarFormat>
```

Aufzählung der unterstützten Formate von [TarArchive](../../com.aspose.zip/tararchive).
## Felder

| Feld | Beschreibung |
| --- | --- |
| [Gnu](#Gnu) | GNU tar basiert auf dem frühen Entwurf von POSIX.1. |
| [Pax](#Pax) | Format definiert im POSIX.1-2001-Standard. |
| [UsTar](#UsTar) | Format erweitert den Header-Block des v7-Formats. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Gnu {#Gnu}
```
public static final TarFormat Gnu
```


GNU tar basiert auf dem frühen Entwurf von POSIX.1. Dieses Format wird in vielen Linux-Systemen als Standard‑Tar‑Format implementiert.

### Pax {#Pax}
```
public static final TarFormat Pax
```


Format definiert im POSIX.1-2001-Standard.

### UsTar {#UsTar}
```
public static final TarFormat UsTar
```


Format erweitert den Header-Block des v7-Formats. Weit verbreitet und in vielen Dienstprogrammen für Windows unterstützt.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static TarFormat valueOf(String name)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[TarFormat](../../com.aspose.zip/tarformat)
### values() {#values--}
```
public static TarFormat[] values()
```




**Returns:**
com.aspose.zip.TarFormat[]
