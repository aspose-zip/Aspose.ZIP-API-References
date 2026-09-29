---
title: "TarFormat"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Enumeración con formatos compatibles de ."
type: docs
weight: 169
url: /es/java/com.aspose.zip/tarformat/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum TarFormat extends Enum<TarFormat>
```

Enumeración con formatos compatibles de [TarArchive](../../com.aspose.zip/tararchive).
## Campos

| Campo | Descripción |
| --- | --- |
| [Gnu](#Gnu) | GNU tar se basa en el borrador temprano de POSIX.1. |
| [Pax](#Pax) | Formato definido en la norma POSIX.1-2001. |
| [UsTar](#UsTar) | El formato amplía el bloque de encabezado del formato v7. |
## Métodos

| Método | Descripción |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Gnu {#Gnu}
```
public static final TarFormat Gnu
```


GNU tar se basa en el borrador temprano de POSIX.1. Este formato se implementa como el formato tar predeterminado en muchos sistemas Linux.

### Pax {#Pax}
```
public static final TarFormat Pax
```


Formato definido en la norma POSIX.1-2001.

### UsTar {#UsTar}
```
public static final TarFormat UsTar
```


El formato amplía el bloque de encabezado del formato v7. Está muy extendido y es compatible con muchas utilidades para Windows.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static TarFormat valueOf(String name)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String |  |

**Returns:**
[TarFormat](../../com.aspose.zip/tarformat)
### values() {#values--}
```
public static TarFormat[] values()
```




**Returns:**
com.aspose.zip.TarFormat[]
