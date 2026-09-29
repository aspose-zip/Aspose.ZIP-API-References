---
title: "AlzArchiveLoadOptions"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "圧縮ファイルから ALZ アーカイブを読み込む際のオプションです。"
type: docs
weight: 12
url: /ja/java/com.aspose.zip/alzarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class AlzArchiveLoadOptions
```

圧縮ファイルから ALZ アーカイブを読み込む際のオプションです。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [AlzArchiveLoadOptions()](#AlzArchiveLoadOptions--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | エントリの復号に使用されるパスワードを取得します。 |
| [getEncoding()](#getEncoding--) | エントリ名に使用されるエンコーディングを取得します。 |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | ALZ エントリのチェックサム検証がスキップされるかどうかを取得します。 |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 抽出をキャンセルするために使用されるキャンセルフラグを設定します。 |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | エントリの復号に使用されるパスワードを設定します。 |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | エントリ名に使用されるエンコーディングを設定します。 |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | ALZ エントリのチェックサム検証をスキップするかどうかを設定します。 |
### AlzArchiveLoadOptions() {#AlzArchiveLoadOptions--}
```
public AlzArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public String getDecryptionPassword()
```


エントリの復号に使用されるパスワードを取得します。

**Returns:**
java.lang.String - エントリの復号に使用されるパスワード、設定されていない場合は `null`
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


エントリ名に使用されるエンコーディングを取得します。デフォルトは韓国 Windows コードページ 949 (CP949) です。ALZ アーカイブは歴史的にファイル名を韓国 Windows ANSI コードページで保存しています。

**Returns:**
java.nio.charset.Charset - エントリ名に使用されるエンコーディング
### getSkipChecksumVerification() {#getSkipChecksumVerification--}
```
public boolean getSkipChecksumVerification()
```


ALZ エントリのチェックサム検証がスキップされるかどうかを取得します。デフォルトは `false` です。

**Returns:**
boolean - チェックサム検証がスキップされるかどうか
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


抽出をキャンセルするために使用されるキャンセルフラグを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | キャンセルフラグ、またはキャンセルを無効にするための `null` |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public void setDecryptionPassword(String value)
```


エントリの復号に使用されるパスワードを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | エントリを復号化するために使用されるパスワード |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


エントリ名に使用されるエンコーディングを設定します。ALZ アーカイブは歴史的に韓国の Windows ANSI コードページを使用してファイル名を保存しています。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.nio.charset.Charset | エントリ名に使用されるエンコーディング |

### setSkipChecksumVerification(boolean value) {#setSkipChecksumVerification-boolean-}
```
public void setSkipChecksumVerification(boolean value)
```


ALZ エントリのチェックサム検証をスキップするかどうかを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | チェックサム検証がスキップされるかどうか |

