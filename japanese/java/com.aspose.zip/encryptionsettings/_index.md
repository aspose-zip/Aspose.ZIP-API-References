---
title: "EncryptionSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "複数の ZIP 暗号化方式の設定のための基底クラス。"
type: docs
weight: 60
url: /ja/java/com.aspose.zip/encryptionsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class EncryptionSettings
```

複数の ZIP 暗号化方式の設定のための基底クラス。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getMethod()](#getMethod--) | 暗号化アルゴリズムを取得します。 |
| [getPassword()](#getPassword--) | 暗号化または復号化のためのパスワードを取得します。 |
| [setPassword(String value)](#setPassword-java.lang.String-) | 暗号化または復号化のためのパスワードを設定します。 |
### getMethod() {#getMethod--}
```
public final EncryptionMethod getMethod()
```


暗号化アルゴリズムを取得します。

**Returns:**
[EncryptionMethod](../../com.aspose.zip/encryptionmethod) - the encryption algorithm.
### getPassword() {#getPassword--}
```
public final String getPassword()
```


暗号化または復号化のためのパスワードを取得します。

**Returns:**
java.lang.String - 暗号化または復号化のパスワード。
### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


暗号化または復号化のためのパスワードを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 暗号化または復号化のパスワード。 |

