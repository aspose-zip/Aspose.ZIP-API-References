---
title: "TarFormat"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Enumeratie met ondersteunde formaten van ."
type: docs
weight: 169
url: /nl/java/com.aspose.zip/tarformat/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum TarFormat extends Enum<TarFormat>
```

Enumeratie met ondersteunde formaten van [TarArchive](../../com.aspose.zip/tararchive).
## Velden

| Veld | Beschrijving |
| --- | --- |
| [Gnu](#Gnu) | GNU tar is gebaseerd op het vroege concept van POSIX.1. |
| [Pax](#Pax) | Formaat gedefinieerd in de POSIX.1-2001-standaard. |
| [UsTar](#UsTar) | Formaat breidt het headerblok uit van het v7-formaat. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Gnu {#Gnu}
```
public static final TarFormat Gnu
```


GNU tar is gebaseerd op het vroege concept van POSIX.1. Dit formaat wordt geïmplementeerd als standaard tar-formaat in veel Linux-systemen.

### Pax {#Pax}
```
public static final TarFormat Pax
```


Formaat gedefinieerd in de POSIX.1-2001-standaard.

### UsTar {#UsTar}
```
public static final TarFormat UsTar
```


Formaat breidt het headerblok uit van het v7-formaat. Veelgebruikt en ondersteund in veel hulpprogramma's voor Windows.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static TarFormat valueOf(String name)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String |  |

**Returns:**
[TarFormat](../../com.aspose.zip/tarformat)
### values() {#values--}
```
public static TarFormat[] values()
```




**Returns:**
com.aspose.zip.TarFormat[]
