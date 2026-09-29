---
title: "XzCheckType"
second_title: "Aspose.ZIP for Java API 参考"
description: "该枚举定义了 xz 存档的校验和计算方法。"
type: docs
weight: 170
url: /zh/java/com.aspose.zip/xzchecktype/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum XzCheckType extends Enum<XzCheckType>
```

该枚举定义了 xz 存档的校验和计算方法。
## 字段

| 字段 | 描述 |
| --- | --- |
| [Crc32](#Crc32) | 校验和将使用 CRC32 算法计算。 |
| [Crc64](#Crc64) | 校验和将使用 CRC64 算法计算。 |
| [None](#None) | 将不会计算校验和。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Crc32 {#Crc32}
```
public static final XzCheckType Crc32
```


校验和将使用 CRC32 算法计算。

### Crc64 {#Crc64}
```
public static final XzCheckType Crc64
```


校验和将使用 CRC64 算法计算。

### None {#None}
```
public static final XzCheckType None
```


将不会计算校验和。

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static XzCheckType valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[XzCheckType](../../com.aspose.zip/xzchecktype)
### values() {#values--}
```
public static XzCheckType[] values()
```




**Returns:**
com.aspose.zip.XzCheckType[]
