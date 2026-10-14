---
title: "EncryptionMethod"
second_title: "Aspose.ZIP for Java API 参考"
description: "加密/解密方法可用于 ZIP 存档。"
type: docs
weight: 165
url: /zh/java/com.aspose.zip/encryptionmethod/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum EncryptionMethod extends Enum<EncryptionMethod>
```

加密/解密方法可用于 ZIP 存档。
## 字段

| 字段 | 描述 |
| --- | --- |
| [AES128](#AES128) | 高级加密标准，密钥长度为 128 位。 |
| [AES192](#AES192) | 具有 192 位密钥长度的高级加密标准。 |
| [AES256](#AES256) | 具有 256 位密钥长度的高级加密标准。 |
| [Traditional](#Traditional) | 传统 PKWARE 加密。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### AES128 {#AES128}
```
public static final EncryptionMethod AES128
```


高级加密标准，密钥长度为 128 位。

### AES192 {#AES192}
```
public static final EncryptionMethod AES192
```


具有 192 位密钥长度的高级加密标准。

### AES256 {#AES256}
```
public static final EncryptionMethod AES256
```


具有 256 位密钥长度的高级加密标准。

### Traditional {#Traditional}
```
public static final EncryptionMethod Traditional
```


传统 PKWARE 加密。

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static EncryptionMethod valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[EncryptionMethod](../../com.aspose.zip/encryptionmethod)
### values() {#values--}
```
public static EncryptionMethod[] values()
```




**Returns:**
com.aspose.zip.EncryptionMethod[]
