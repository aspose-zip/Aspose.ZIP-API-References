---
title: "AppleLzmaCompressionSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "Apple アーカイブ .aar ファイル内の LZMA 圧縮設定です。"
type: docs
weight: 23
url: /ja/java/com.aspose.zip/applelzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLzmaCompressionSettings extends AppleCompressionSettings
```

Apple Archive (.aar) ファイル内の LZMA 圧縮の設定です。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [AppleLzmaCompressionSettings(int blockSize)](#AppleLzmaCompressionSettings-int-) | 新しいインスタンスの [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) クラスを初期化します。 |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize)](#AppleLzmaCompressionSettings-int-int-) | 新しいインスタンスの [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) クラスを初期化します。 |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)](#AppleLzmaCompressionSettings-int-int-int-) | 新しいインスタンスの [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) クラスを初期化します。 |
| [AppleLzmaCompressionSettings()](#AppleLzmaCompressionSettings--) | デフォルト パラメーターを使用して、[AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | 圧縮前の各データブロックのサイズを取得します。 |
| [getDictionarySize()](#getDictionarySize--) | 圧縮に使用される辞書サイズを取得します。 |
| [getFastBytes()](#getFastBytes--) | 圧縮に使用される高速バイト数を取得します。 |
### AppleLzmaCompressionSettings(int blockSize) {#AppleLzmaCompressionSettings-int-}
```
public AppleLzmaCompressionSettings(int blockSize)
```


新しいインスタンスの [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) クラスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| blockSize | int | 圧縮前の各データブロックのサイズです。 |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize) {#AppleLzmaCompressionSettings-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize)
```


新しいインスタンスの [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) クラスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| blockSize | int | 圧縮前の各データブロックのサイズです。 |
| dictionarySize | int | 圧縮に使用される辞書サイズです。 |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes) {#AppleLzmaCompressionSettings-int-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)
```


新しいインスタンスの [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) クラスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| blockSize | int | 圧縮前の各データブロックのサイズです。 |
| dictionarySize | int | 圧縮に使用される辞書サイズです。 |
| fastBytes | int | 圧縮に使用される高速バイト数です。 |

### AppleLzmaCompressionSettings() {#AppleLzmaCompressionSettings--}
```
public AppleLzmaCompressionSettings()
```


デフォルト パラメーターを使用して、[AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) クラスの新しいインスタンスを初期化します。

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


圧縮前の各データブロックのサイズを取得します。

値: デフォルト値は 4 MiB です。

**Returns:**
int - 圧縮前の各データブロックのサイズ。
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


圧縮に使用される辞書サイズを取得します。

Value: デフォルト値は 8 MiB です。

**Returns:**
int - 圧縮に使用される辞書サイズ。
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


圧縮に使用される高速バイト数を取得します。

Value: デフォルト値は 32 です。

**Returns:**
int - 圧縮に使用される高速バイト数。
