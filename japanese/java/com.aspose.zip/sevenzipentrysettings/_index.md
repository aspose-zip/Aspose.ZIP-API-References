---
title: "SevenZipEntrySettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "7z エントリを圧縮または展開するために使用される設定。"
type: docs
weight: 113
url: /ja/java/com.aspose.zip/sevenzipentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipEntrySettings
```

7z エントリを圧縮または展開するために使用される設定。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [SevenZipEntrySettings()](#SevenZipEntrySettings--) | 新しい [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) クラスのインスタンスを初期化します。 |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-) | 新しい [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) クラスのインスタンスを初期化します。 |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-) | 新しい [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCompressHeader()](#getCompressHeader--) | アーカイブヘッダーを圧縮するかどうかを示す値を取得します。 |
| [getCompressionSettings()](#getCompressionSettings--) | 圧縮または解凍ルーチンの設定を取得します。 |
| [getEncryptionSettings()](#getEncryptionSettings--) | 暗号化または復号化の設定を取得します。 |
| [getSolid()](#getSolid--) | エントリを連結して単一のデータブロックとして扱うかどうかを示す値を取得します。 |
| [setCompressHeader(boolean value)](#setCompressHeader-boolean-) | アーカイブヘッダーを圧縮するかどうかを示す値を設定します。 |
| [setSolid(boolean value)](#setSolid-boolean-) | エントリを連結して単一のデータブロックとして扱うかどうかを示す値を設定します。 |
### SevenZipEntrySettings() {#SevenZipEntrySettings--}
```
public SevenZipEntrySettings()
```


新しい [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) クラスのインスタンスを初期化します。

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)
```


新しい [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | 圧縮の設定です。デフォルトの LZMA 設定を使用する場合は null を渡します。 |

以下のいずれかにできます：

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)
```


新しい [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | 圧縮の設定です。デフォルトの LZMA 設定を使用する場合は null を渡します。 |

以下のいずれかにできます：

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |
|  | encryptionSettings | [SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) | 暗号化の設定です。暗号化または復号化が不要な場合は null を渡します。 |

唯一の選択肢は次のとおりです：

 *  [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) |

### getCompressHeader() {#getCompressHeader--}
```
public final boolean getCompressHeader()
```


アーカイブヘッダーを圧縮するかどうかを示す値を取得します。

この設定は 7-Zip ツールの `-mhc=on` スイッチに相当します。現在、ヘッダー暗号化とは互換性がありません。

**Returns:**
boolean - アーカイブヘッダーを圧縮するかどうかを示す値
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


圧縮または解凍ルーチンの設定を取得します。

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression routine
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final SevenZipEncryptionSettings getEncryptionSettings()
```


暗号化または復号化の設定を取得します。特定のエントリの設定は異なる場合があります。

[SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) は 7z アーカイブの唯一のオプションです。

**Returns:**
[SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) - settings for encryption or decryption
### getSolid() {#getSolid--}
```
public final boolean getSolid()
```


エントリを連結して単一のデータブロックとして扱うかどうかを示す値を取得します。

次の例は、ディレクトリを暗号化せずに LZMA2 圧縮でソリッド 7z アーカイブに圧縮する方法を示しています。

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream(\"archive.7z\")) {
SevenZipEntrySettings settings = new SevenZipEntrySettings(new SevenZipLZMACompressionSettings());
settings.setSolid(true);
try (SevenZipArchive archive = new SevenZipArchive(settings)) {
archive.createEntries("C:\\Documents");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

Provide `SevenZipEntrySettings` for solid 7z archive on archive instantiation.

**Returns:**
boolean - value indicating whether to concatenate entries and treat them as a single data block.
### setCompressHeader(boolean value) {#setCompressHeader-boolean-}
```
public final void setCompressHeader(boolean value)
```


Sets value indicating whether to compress archive header.

This setting is equivalent `-mhc=on` switch of 7-Zip tool. Currently, it is incompatible with header encryption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to compress archive header |

### setSolid(boolean value) {#setSolid-boolean-}
```
public final void setSolid(boolean value)
```


Sets value indicating whether to concatenate entries and treat them as a single data block.

The following example shows how to compress a directory to solid 7z archive with LZMA2 compression without encryption.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         SevenZipEntrySettings settings = new SevenZipEntrySettings(new SevenZipLZMACompressionSettings());
         settings.setSolid(true);
         try (SevenZipArchive archive = new SevenZipArchive(settings)) {
             archive.createEntries("C:\\Documents");
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

アーカイブのインスタンス化時に、ソリッド 7z アーカイブ用の `SevenZipEntrySettings` を提供します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | エントリを連結して単一のデータブロックとして扱うかどうかを示す値。 |

