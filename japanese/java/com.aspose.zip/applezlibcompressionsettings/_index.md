---
title: "AppleZlibCompressionSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "Apple アーカイブ .aar ファイル内の Zlib 圧縮設定です。"
type: docs
weight: 25
url: /ja/java/com.aspose.zip/applezlibcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleZlibCompressionSettings extends AppleCompressionSettings
```

Apple Archive (.aar) ファイル内の Zlib 圧縮の設定です。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [AppleZlibCompressionSettings(int blockSize)](#AppleZlibCompressionSettings-int-) | 新しい [AppleZlibCompressionSettings](../../com.aspose.zip/applezlibcompressionsettings) クラスのインスタンスを初期化します。 |
| [AppleZlibCompressionSettings()](#AppleZlibCompressionSettings--) | デフォルトパラメータで新しい [AppleZlibCompressionSettings](../../com.aspose.zip/applezlibcompressionsettings) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | 圧縮前の各データブロックのサイズを取得します。 |
### AppleZlibCompressionSettings(int blockSize) {#AppleZlibCompressionSettings-int-}
```
public AppleZlibCompressionSettings(int blockSize)
```


新しい [AppleZlibCompressionSettings](../../com.aspose.zip/applezlibcompressionsettings) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| blockSize | int | 圧縮前の各データブロックのサイズです。 |

### AppleZlibCompressionSettings() {#AppleZlibCompressionSettings--}
```
public AppleZlibCompressionSettings()
```


デフォルトパラメータで新しい [AppleZlibCompressionSettings](../../com.aspose.zip/applezlibcompressionsettings) クラスのインスタンスを初期化します。

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


圧縮前の各データブロックのサイズを取得します。

値: デフォルト値は 4 MiB です。

**Returns:**
int - 圧縮前の各データブロックのサイズ。
