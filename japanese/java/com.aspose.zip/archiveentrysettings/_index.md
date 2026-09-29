---
title: "ArchiveEntrySettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "エントリを圧縮または解凍するために使用される設定です。"
type: docs
weight: 30
url: /ja/java/com.aspose.zip/archiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveEntrySettings
```

エントリを圧縮または解凍するために使用される設定です。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ArchiveEntrySettings()](#ArchiveEntrySettings--) | 新しい [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) クラスのインスタンスを初期化します。 |
| [ArchiveEntrySettings(CompressionSettings compressionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-) | 新しい [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) クラスのインスタンスを初期化します。 |
| [ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-) | 新しい [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getComment()](#getComment--) | ZIP アーカイブ内のエントリのコメントを取得します。 |
| [getCompressionSettings()](#getCompressionSettings--) | 圧縮または解凍ルーチンの設定を取得します。 |
| [getEncryptionSettings()](#getEncryptionSettings--) | 暗号化または復号化の設定を取得します。 |
| [setComment(String value)](#setComment-java.lang.String-) | ZIP アーカイブ内のエントリのコメント。 |
### ArchiveEntrySettings() {#ArchiveEntrySettings--}
```
public ArchiveEntrySettings()
```


新しい [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) クラスのインスタンスを初期化します。

### ArchiveEntrySettings(CompressionSettings compressionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings)
```


新しい [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | 圧縮の設定です。デフォルトのデフレート設定の場合は null を渡してください。 |

以下のいずれかにできます：

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |

### ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)
```


新しい [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | 圧縮の設定です。デフォルトのデフレート設定の場合は null を渡してください。 |

以下のいずれかにできます：

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |
|  | encryptionSettings | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | 暗号化の設定です。暗号化または復号が不要な場合は null を渡してください。 |

以下のいずれかにできます：

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) |

### getComment() {#getComment--}
```
public final String getComment()
```


ZIP アーカイブ内のエントリのコメントを取得します。

**Returns:**
java.lang.String - ZIP アーカイブ内のエントリに対するコメントです。
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


圧縮または解凍ルーチンの設定を取得します。

以下のいずれかにできます：

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings)

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression routine.
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final EncryptionSettings getEncryptionSettings()
```


暗号化または復号化の設定を取得します。特定のエントリの設定は異なる場合があります。

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - settings for encryption or decryption. Settings of particular entry may vary.
### setComment(String value) {#setComment-java.lang.String-}
```
public final void setComment(String value)
```


ZIP アーカイブ内のエントリのコメント。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String |  |

