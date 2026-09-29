---
title: "AppleArchiveEntrySettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "エントリを構成するために使用される設定です。"
type: docs
weight: 18
url: /ja/java/com.aspose.zip/applearchiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class AppleArchiveEntrySettings
```

エントリを構成するために使用される設定です [AppleArchive](../../com.aspose.zip/applearchive) の内部で。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)](#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-) | [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | 構成された Apple Archive ペイロードに適用される圧縮設定を取得します。 |
| [getIncludeCrc32Checksum()](#getIncludeCrc32Checksum--) | 構成されたファイルエントリに CRC32 チェックサムフィールドが含まれるかどうかを示す値を取得します。 |
| [setIncludeCrc32Checksum(boolean value)](#setIncludeCrc32Checksum-boolean-) | 構成されたファイルエントリに CRC32 チェックサムフィールドが含まれるかどうかを示す値を設定します。 |
### AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings) {#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-}
```
public AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)
```


[AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| compressionSettings | [AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) | 構成された Apple Archive ペイロードに適用される圧縮設定。 |

### getCompressionSettings() {#getCompressionSettings--}
```
public final AppleCompressionSettings getCompressionSettings()
```


構成された Apple Archive ペイロードに適用される圧縮設定を取得します。

**Returns:**
[AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) - compression settings applied to the composed Apple Archive payload.
### getIncludeCrc32Checksum() {#getIncludeCrc32Checksum--}
```
public final boolean getIncludeCrc32Checksum()
```


構成されたファイルエントリに CRC32 チェックサムフィールドが含まれるかどうかを示す値を取得します。

**Returns:**
boolean - 構成されたファイルエントリに CRC32 チェックサムフィールドが含まれるかどうかを示す値。
### setIncludeCrc32Checksum(boolean value) {#setIncludeCrc32Checksum-boolean-}
```
public final void setIncludeCrc32Checksum(boolean value)
```


構成されたファイルエントリに CRC32 チェックサムフィールドが含まれるかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 構成されたファイルエントリに CRC32 チェックサムフィールドが含まれるかどうかを示す値。 |

