---
title: "XzCheckType"
second_title: "Aspose.ZIP for Java API 참조"
description: "열거형은 xz 아카이브에 대한 체크섬 계산 방식을 정의합니다."
type: docs
weight: 170
url: /ko/java/com.aspose.zip/xzchecktype/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum XzCheckType extends Enum<XzCheckType>
```

열거형은 xz 아카이브에 대한 체크섬 계산 방식을 정의합니다.
## 필드

| 필드 | 설명 |
| --- | --- |
| [Crc32](#Crc32) | 체크섬은 CRC32 알고리즘을 사용하여 계산됩니다. |
| [Crc64](#Crc64) | 체크섬은 CRC64 알고리즘을 사용하여 계산됩니다. |
| [None](#None) | 체크섬이 계산되지 않습니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Crc32 {#Crc32}
```
public static final XzCheckType Crc32
```


체크섬은 CRC32 알고리즘을 사용하여 계산됩니다.

### Crc64 {#Crc64}
```
public static final XzCheckType Crc64
```


체크섬은 CRC64 알고리즘을 사용하여 계산됩니다.

### None {#None}
```
public static final XzCheckType None
```


체크섬이 계산되지 않습니다.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static XzCheckType valueOf(String name)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 이름 | java.lang.String |  |

**Returns:**
[XzCheckType](../../com.aspose.zip/xzchecktype)
### values() {#values--}
```
public static XzCheckType[] values()
```




**Returns:**
com.aspose.zip.XzCheckType[]
