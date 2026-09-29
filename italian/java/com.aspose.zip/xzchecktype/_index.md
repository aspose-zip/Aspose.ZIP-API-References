---
title: "XzCheckType"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "L'enumerazione definisce l'approccio di calcolo del checksum per l'archivio xz."
type: docs
weight: 170
url: /it/java/com.aspose.zip/xzchecktype/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum XzCheckType extends Enum<XzCheckType>
```

L'enumerazione definisce l'approccio di calcolo del checksum per l'archivio xz.
## Campi

| Campo | Descrizione |
| --- | --- |
| [Crc32](#Crc32) | Il checksum verrà calcolato usando l'algoritmo CRC32. |
| [Crc64](#Crc64) | Il checksum verrà calcolato usando l'algoritmo CRC64. |
| [None](#None) | Il checksum non verrà calcolato. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Crc32 {#Crc32}
```
public static final XzCheckType Crc32
```


Il checksum verrà calcolato usando l'algoritmo CRC32.

### Crc64 {#Crc64}
```
public static final XzCheckType Crc64
```


Il checksum verrà calcolato usando l'algoritmo CRC64.

### None {#None}
```
public static final XzCheckType None
```


Il checksum non verrà calcolato.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static XzCheckType valueOf(String name)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String |  |

**Returns:**
[XzCheckType](../../com.aspose.zip/xzchecktype)
### values() {#values--}
```
public static XzCheckType[] values()
```




**Returns:**
com.aspose.zip.XzCheckType[]
