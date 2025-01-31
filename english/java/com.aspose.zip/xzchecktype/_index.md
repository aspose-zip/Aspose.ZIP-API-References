---
title: XzCheckType
second_title: Aspose.ZIP for Java API Reference
description: The enumeration defines checksum calculation approach for xz archive.
type: docs
weight: 130
url: /java/com.aspose.zip/xzchecktype/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum XzCheckType extends Enum<XzCheckType>
```

The enumeration defines checksum calculation approach for xz archive.
## Fields

| Field | Description |
| --- | --- |
| [Crc32](#Crc32) | Checksum will be calculated using CRC32 algorithm. |
| [Crc64](#Crc64) | Checksum will be calculated using CRC64 algorithm. |
| [None](#None) | Checksum will not be calculated. |
## Methods

| Method | Description |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Crc32 {#Crc32}
```
public static final XzCheckType Crc32
```


Checksum will be calculated using CRC32 algorithm.

### Crc64 {#Crc64}
```
public static final XzCheckType Crc64
```


Checksum will be calculated using CRC64 algorithm.

### None {#None}
```
public static final XzCheckType None
```


Checksum will not be calculated.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static XzCheckType valueOf(String name)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[XzCheckType](../../com.aspose.zip/xzchecktype)
### values() {#values--}
```
public static XzCheckType[] values()
```




**Returns:**
com.aspose.zip.XzCheckType[]
