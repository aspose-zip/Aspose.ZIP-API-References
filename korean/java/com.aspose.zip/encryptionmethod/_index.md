---
title: "EncryptionMethod"
second_title: "Aspose.ZIP for Java API 참조"
description: "ZIP 아카이브와 함께 암호화/복호화 방법을 사용할 수 있습니다."
type: docs
weight: 165
url: /ko/java/com.aspose.zip/encryptionmethod/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum EncryptionMethod extends Enum<EncryptionMethod>
```

ZIP 아카이브와 함께 암호화/복호화 방법을 사용할 수 있습니다.
## 필드

| 필드 | 설명 |
| --- | --- |
| [AES128](#AES128) | 키 길이가 128비트인 고급 암호화 표준. |
| [AES192](#AES192) | 키 길이가 192비트인 고급 암호화 표준. |
| [AES256](#AES256) | 키 길이가 256비트인 고급 암호화 표준. |
| [Traditional](#Traditional) | 전통적인 PKWARE 암호화. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### AES128 {#AES128}
```
public static final EncryptionMethod AES128
```


키 길이가 128비트인 고급 암호화 표준.

### AES192 {#AES192}
```
public static final EncryptionMethod AES192
```


키 길이가 192비트인 고급 암호화 표준.

### AES256 {#AES256}
```
public static final EncryptionMethod AES256
```


키 길이가 256비트인 고급 암호화 표준.

### Traditional {#Traditional}
```
public static final EncryptionMethod Traditional
```


전통적인 PKWARE 암호화.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static EncryptionMethod valueOf(String name)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 이름 | java.lang.String |  |

**Returns:**
[EncryptionMethod](../../com.aspose.zip/encryptionmethod)
### values() {#values--}
```
public static EncryptionMethod[] values()
```




**Returns:**
com.aspose.zip.EncryptionMethod[]
