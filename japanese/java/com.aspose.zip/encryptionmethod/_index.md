---
title: "EncryptionMethod"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "ZIP アーカイブで暗号化/復号化メソッドを使用できます。"
type: docs
weight: 165
url: /ja/java/com.aspose.zip/encryptionmethod/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum EncryptionMethod extends Enum<EncryptionMethod>
```

ZIP アーカイブで暗号化/復号化メソッドを使用できます。
## フィールド

| フィールド | 説明 |
| --- | --- |
| [AES128](#AES128) | Advanced Encryption Standard のキー長 128 ビット。 |
| [AES192](#AES192) | Advanced Encryption Standard のキー長 192 ビット。 |
| [AES256](#AES256) | Advanced Encryption Standard のキー長 256 ビット。 |
| [Traditional](#Traditional) | 従来の PKWARE 暗号化。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### AES128 {#AES128}
```
public static final EncryptionMethod AES128
```


Advanced Encryption Standard のキー長 128 ビット。

### AES192 {#AES192}
```
public static final EncryptionMethod AES192
```


Advanced Encryption Standard のキー長 192 ビット。

### AES256 {#AES256}
```
public static final EncryptionMethod AES256
```


Advanced Encryption Standard のキー長 256 ビット。

### Traditional {#Traditional}
```
public static final EncryptionMethod Traditional
```


従来の PKWARE 暗号化。

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static EncryptionMethod valueOf(String name)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 名前 | java.lang.String |  |

**Returns:**
[EncryptionMethod](../../com.aspose.zip/encryptionmethod)
### values() {#values--}
```
public static EncryptionMethod[] values()
```




**Returns:**
com.aspose.zip.EncryptionMethod[]
