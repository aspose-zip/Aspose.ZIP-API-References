---
title: "SevenZipLZMA2CompressionSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "7z アーカイブ内の LZMA2 圧縮方式の設定。"
type: docs
weight: 114
url: /ja/java/com.aspose.zip/sevenziplzma2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMA2CompressionSettings extends SevenZipCompressionSettings
```

7z アーカイブ内の LZMA2 圧縮方式の設定。

LZMA2 は圧縮された LZMA データと非圧縮データの複数のランをサポートします。

詳しくは: [Lempel\\u2013Ziv\\u2013Markov\_chain\_algorithm][Lempel_u2013Ziv_u2013Markov_chain_algorithm]


[Lempel_u2013Ziv_u2013Markov_chain_algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [SevenZipLZMA2CompressionSettings()](#SevenZipLZMA2CompressionSettings--) | 7z アーカイブ内の LZMA2 圧縮方式の設定をインスタンス化します。 |
| [SevenZipLZMA2CompressionSettings(int dictionarySize)](#SevenZipLZMA2CompressionSettings-int-) | 7z アーカイブ内の LZMA2 圧縮方式の設定をインスタンス化します。 |
| [SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)](#SevenZipLZMA2CompressionSettings-int-int-) | 7z アーカイブ内の LZMA2 圧縮方式の設定をインスタンス化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | 圧縮スレッド数を取得します。 |
| [getDictionarySize()](#getDictionarySize--) | 辞書（履歴バッファ）サイズは、最近処理された非圧縮データがメモリに保持されるバイト数を示します。 |
| [getFastBytes()](#getFastBytes--) | LZMA2 コンプレッサーで使用される高速バイト数の制御番号を取得します。 |
| [getMethod()](#getMethod--) | 圧縮または解凍の方式を取得します。 |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | 圧縮スレッド数を設定します。 |
### SevenZipLZMA2CompressionSettings() {#SevenZipLZMA2CompressionSettings--}
```
public SevenZipLZMA2CompressionSettings()
```


7z アーカイブ内の LZMA2 圧縮方式の設定をインスタンス化します。

### SevenZipLZMA2CompressionSettings(int dictionarySize) {#SevenZipLZMA2CompressionSettings-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize)
```


7z アーカイブ内の LZMA2 圧縮方式の設定をインスタンス化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | dictionarySize | int | 履歴バッファのサイズは 4096 から 1073741824 の間でなければなりません。 |

辞書が大きいほど、通常は圧縮率が向上しますが、非圧縮データより大きい辞書は RAM の無駄です。 |

### SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes) {#SevenZipLZMA2CompressionSettings-int-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)
```


7z アーカイブ内の LZMA2 圧縮方式の設定をインスタンス化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | dictionarySize | int | 履歴バッファのサイズは 4096 から 1073741824 の間でなければなりません。 |

辞書が大きいほど、通常は圧縮率が向上しますが、非圧縮データより大きい辞書は RAM の無駄です。 |
| fastBytes | int | LZMA2 圧縮器が使用する高速バイト数を制御します。高速バイト数を増やすと、圧縮速度を犠牲にして圧縮率を向上させることができます。 |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


圧縮スレッド数を取得します。値が 1 より大きい場合、マルチスレッド圧縮が使用されます。

**Returns:**
int - 圧縮スレッド数
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


辞書（履歴バッファ）サイズは、最近処理された非圧縮データがメモリに保持されるバイト数を示します。

**Returns:**
int - 辞書（履歴バッファ）サイズ
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


LZMA2 コンプレッサーで使用される高速バイト数の制御番号を取得します。

**Returns:**
int - LZMA2 圧縮器が使用する高速バイト数の制御番号
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


圧縮または解凍の方式を取得します。

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method.
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


圧縮スレッド数を設定します。値が 1 より大きい場合、マルチスレッド圧縮が使用されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | 値 | int | 圧縮スレッド数。 |

この数値を CPU コア数以上に設定しないでください。 |

