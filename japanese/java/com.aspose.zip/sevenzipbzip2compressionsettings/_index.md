---
title: "SevenZipBZip2CompressionSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "7z アーカイブ内の BZip2 圧縮方式の設定。"
type: docs
weight: 109
url: /ja/java/com.aspose.zip/sevenzipbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipBZip2CompressionSettings extends SevenZipCompressionSettings
```

7z アーカイブ内の BZip2 圧縮方式の設定。

Bzip2 は Burrows-Wheeler ブロックソートテキスト圧縮アルゴリズムとハフマン符号化を使用してファイルを圧縮します。

詳しくは: [Bzip2][]


[Bzip2]: https://en.wikipedia.org/wiki/Bzip2
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [SevenZipBZip2CompressionSettings(int blockSize)](#SevenZipBZip2CompressionSettings-int-) | 新しい [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) クラスのインスタンスを初期化します。 |
| [SevenZipBZip2CompressionSettings()](#SevenZipBZip2CompressionSettings--) | デフォルトのブロックサイズ（9 百キロバイト）で [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | ブロックサイズ（百キロバイト単位）。 |
| [getMethod()](#getMethod--) | 圧縮または解凍の方式を取得します。 |
### SevenZipBZip2CompressionSettings(int blockSize) {#SevenZipBZip2CompressionSettings-int-}
```
public SevenZipBZip2CompressionSettings(int blockSize)
```


新しい [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| blockSize | int | ブロックサイズ（百キロバイト単位） |

### SevenZipBZip2CompressionSettings() {#SevenZipBZip2CompressionSettings--}
```
public SevenZipBZip2CompressionSettings()
```


デフォルトのブロックサイズ（9 百キロバイト）で [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) クラスの新しいインスタンスを初期化します。

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


ブロックサイズ（百キロバイト単位）。

**Returns:**
int - ブロックサイズ（百キロバイト単位）
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


圧縮または解凍の方式を取得します。

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
