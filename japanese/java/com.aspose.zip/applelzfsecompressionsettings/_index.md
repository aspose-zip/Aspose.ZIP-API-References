---
title: "AppleLzfseCompressionSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "Apple Archive の .aar ファイル内での LZFSE 圧縮設定。"
type: docs
weight: 22
url: /ja/java/com.aspose.zip/applelzfsecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLzfseCompressionSettings extends AppleCompressionSettings
```

Apple Archive (.aar) ファイル内の LZFSE 圧縮の設定です。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [AppleLzfseCompressionSettings(int blockSize)](#AppleLzfseCompressionSettings-int-) | 新しい [AppleLzfseCompressionSettings](../../com.aspose.zip/applelzfsecompressionsettings) クラスのインスタンスを初期化します。 |
| [AppleLzfseCompressionSettings()](#AppleLzfseCompressionSettings--) | デフォルトパラメーターで新しい [AppleLzfseCompressionSettings](../../com.aspose.zip/applelzfsecompressionsettings) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | 圧縮前の各データブロックのサイズを取得します。 |
### AppleLzfseCompressionSettings(int blockSize) {#AppleLzfseCompressionSettings-int-}
```
public AppleLzfseCompressionSettings(int blockSize)
```


新しい [AppleLzfseCompressionSettings](../../com.aspose.zip/applelzfsecompressionsettings) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| blockSize | int | 圧縮前の各データブロックのサイズです。 |

### AppleLzfseCompressionSettings() {#AppleLzfseCompressionSettings--}
```
public AppleLzfseCompressionSettings()
```


デフォルトパラメーターで新しい [AppleLzfseCompressionSettings](../../com.aspose.zip/applelzfsecompressionsettings) クラスのインスタンスを初期化します。

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


圧縮前の各データブロックのサイズを取得します。

値: デフォルト値は 4 MiB です。

**Returns:**
int - 圧縮前の各データブロックのサイズ。
