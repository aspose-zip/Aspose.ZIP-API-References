---
title: "XzCheckType"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "この列挙は xz アーカイブのチェックサム計算方法を定義します。"
type: docs
weight: 170
url: /ja/java/com.aspose.zip/xzchecktype/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum XzCheckType extends Enum<XzCheckType>
```

この列挙は xz アーカイブのチェックサム計算方法を定義します。
## フィールド

| フィールド | 説明 |
| --- | --- |
| [Crc32](#Crc32) | チェックサムは CRC32 アルゴリズムを使用して計算されます。 |
| [Crc64](#Crc64) | チェックサムは CRC64 アルゴリズムを使用して計算されます。 |
| [None](#None) | チェックサムは計算されません。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Crc32 {#Crc32}
```
public static final XzCheckType Crc32
```


チェックサムは CRC32 アルゴリズムを使用して計算されます。

### Crc64 {#Crc64}
```
public static final XzCheckType Crc64
```


チェックサムは CRC64 アルゴリズムを使用して計算されます。

### None {#None}
```
public static final XzCheckType None
```


チェックサムは計算されません。

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static XzCheckType valueOf(String name)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 名前 | java.lang.String |  |

**Returns:**
[XzCheckType](../../com.aspose.zip/xzchecktype)
### values() {#values--}
```
public static XzCheckType[] values()
```




**Returns:**
com.aspose.zip.XzCheckType[]
