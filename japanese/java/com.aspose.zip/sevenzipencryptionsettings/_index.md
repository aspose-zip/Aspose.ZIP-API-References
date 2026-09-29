---
title: "SevenZipEncryptionSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "複数の 7z 暗号化方式の設定の基底クラス。"
type: docs
weight: 112
url: /ja/java/com.aspose.zip/sevenzipencryptionsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class SevenZipEncryptionSettings
```

複数の 7z 暗号化方式の設定の基底クラス。

AES-256 は 7z アーカイブで使用できる唯一の暗号化方式です。そのため、[SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) が唯一の実装です。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getEncryptHeader()](#getEncryptHeader--) | ヘッダー暗号化を示す値を取得します。 |
| [getPassword()](#getPassword--) | 暗号化または復号化のためのパスワードを取得します。 |
| [setEncryptHeader(boolean value)](#setEncryptHeader-boolean-) | ヘッダー暗号化を示す値を設定します。 |
| [setPassword(String value)](#setPassword-java.lang.String-) | 暗号化または復号化のためのパスワードを設定します。 |
### getEncryptHeader() {#getEncryptHeader--}
```
public final boolean getEncryptHeader()
```


ヘッダー暗号化を示す値を取得します。

この設定は 7-Zip ツールの `-mhe=on` スイッチと同等です。現在、ヘッダー圧縮とは互換性がありません。

**Returns:**
boolean - ヘッダー暗号化を示す値
### getPassword() {#getPassword--}
```
public final String getPassword()
```


暗号化または復号化のためのパスワードを取得します。

**Returns:**
java.lang.String - 暗号化または復号化のためのパスワード
### setEncryptHeader(boolean value) {#setEncryptHeader-boolean-}
```
public final void setEncryptHeader(boolean value)
```


ヘッダー暗号化を示す値を設定します。

この設定は 7-Zip ツールの `-mhe=on` スイッチと同等です。現在、ヘッダー圧縮とは互換性がありません。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | ヘッダー暗号化を示す値 |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


暗号化または復号化のためのパスワードを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 暗号化または復号化のためのパスワード |

