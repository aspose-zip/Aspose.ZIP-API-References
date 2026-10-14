---
title: "TarFormat"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Desteklenen biçimlerin listesi ."
type: docs
weight: 169
url: /tr/java/com.aspose.zip/tarformat/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum TarFormat extends Enum<TarFormat>
```

Desteklenen biçimlerin listesi [TarArchive](../../com.aspose.zip/tararchive).
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [Gnu](#Gnu) | GNU tar, POSIX.1'in erken taslağına dayanır. |
| [Pax](#Pax) | Biçim, POSIX.1-2001 standardında tanımlanmıştır. |
| [UsTar](#UsTar) | Biçim, v7 biçiminden gelen başlık bloğunu genişletir. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Gnu {#Gnu}
```
public static final TarFormat Gnu
```


GNU tar, POSIX.1'in erken taslağına dayanır. Bu biçim, birçok Linux sisteminde varsayılan tar biçimi olarak uygulanır.

### Pax {#Pax}
```
public static final TarFormat Pax
```


Biçim, POSIX.1-2001 standardında tanımlanmıştır.

### UsTar {#UsTar}
```
public static final TarFormat UsTar
```


Biçim, v7 biçiminden gelen başlık bloğunu genişletir. Windows için birçok yardımcı programda yaygın ve desteklenir.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static TarFormat valueOf(String name)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

**Returns:**
[TarFormat](../../com.aspose.zip/tarformat)
### values() {#values--}
```
public static TarFormat[] values()
```




**Returns:**
com.aspose.zip.TarFormat[]
