---
title: "XzCheckType"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "L'énumération définit l'approche de calcul du checksum pour l'archive xz."
type: docs
weight: 170
url: /fr/java/com.aspose.zip/xzchecktype/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum XzCheckType extends Enum<XzCheckType>
```

L'énumération définit l'approche de calcul du checksum pour l'archive xz.
## Champs

| Champ | Description |
| --- | --- |
| [Crc32](#Crc32) | La somme de contrôle sera calculée à l'aide de l'algorithme CRC32. |
| [Crc64](#Crc64) | La somme de contrôle sera calculée à l'aide de l'algorithme CRC64. |
| [None](#None) | La somme de contrôle ne sera pas calculée. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Crc32 {#Crc32}
```
public static final XzCheckType Crc32
```


La somme de contrôle sera calculée à l'aide de l'algorithme CRC32.

### Crc64 {#Crc64}
```
public static final XzCheckType Crc64
```


La somme de contrôle sera calculée à l'aide de l'algorithme CRC64.

### None {#None}
```
public static final XzCheckType None
```


La somme de contrôle ne sera pas calculée.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static XzCheckType valueOf(String name)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String |  |

**Returns:**
[XzCheckType](../../com.aspose.zip/xzchecktype)
### values() {#values--}
```
public static XzCheckType[] values()
```




**Returns:**
com.aspose.zip.XzCheckType[]
