---
title: "TarFormat"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Enumerazione con i formati supportati di ."
type: docs
weight: 169
url: /it/java/com.aspose.zip/tarformat/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum TarFormat extends Enum<TarFormat>
```

Enumerazione con i formati supportati di [TarArchive](../../com.aspose.zip/tararchive).
## Campi

| Campo | Descrizione |
| --- | --- |
| [Gnu](#Gnu) | GNU tar si basa sulla bozza iniziale di POSIX.1. |
| [Pax](#Pax) | Formato definito nello standard POSIX.1-2001. |
| [UsTar](#UsTar) | Il formato estende il blocco di intestazione del formato v7. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Gnu {#Gnu}
```
public static final TarFormat Gnu
```


GNU tar si basa sulla bozza iniziale di POSIX.1. Questo formato è implementato come formato tar predefinito in molti sistemi Linux.

### Pax {#Pax}
```
public static final TarFormat Pax
```


Formato definito nello standard POSIX.1-2001.

### UsTar {#UsTar}
```
public static final TarFormat UsTar
```


Il formato estende il blocco di intestazione del formato v7. Diffuso e supportato in molte utility per Windows.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static TarFormat valueOf(String name)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String |  |

**Returns:**
[TarFormat](../../com.aspose.zip/tarformat)
### values() {#values--}
```
public static TarFormat[] values()
```




**Returns:**
com.aspose.zip.TarFormat[]
