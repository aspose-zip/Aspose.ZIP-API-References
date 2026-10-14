---
title: "AppleLz4CompressionSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: ".aar ファイル内の Apple アーカイブに対する LZ4 圧縮の設定。"
type: docs
weight: 21
url: /ja/java/com.aspose.zip/applelz4compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLz4CompressionSettings extends AppleCompressionSettings
```

Apple Archive (.aar) ファイル内の LZ4 圧縮の設定です。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [AppleLz4CompressionSettings(int blockSize)](#AppleLz4CompressionSettings-int-) | 新しい [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) クラスのインスタンスを初期化します。 |
| [AppleLz4CompressionSettings()](#AppleLz4CompressionSettings--) | デフォルトパラメーターで [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | `pbz4`/`bv41` ブロックそれぞれの圧縮サイズを取得します。 |
### AppleLz4CompressionSettings(int blockSize) {#AppleLz4CompressionSettings-int-}
```
public AppleLz4CompressionSettings(int blockSize)
```


新しい [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| blockSize | int | 各圧縮された `pbz4`/`bv41` ブロックのサイズです。 |

### AppleLz4CompressionSettings() {#AppleLz4CompressionSettings--}
```
public AppleLz4CompressionSettings()
```


デフォルトパラメーターで [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) クラスの新しいインスタンスを初期化します。

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


`pbz4`/`bv41` ブロックそれぞれの圧縮サイズを取得します。

値: デフォルト値は 4 MiB です。

**Returns:**
int - 各圧縮された `pbz4`/`bv41` ブロックのサイズ。
