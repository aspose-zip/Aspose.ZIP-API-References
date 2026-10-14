---
title: "LzmaCompressionSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "LZMA 圧縮方式の設定。"
type: docs
weight: 88
url: /ja/java/com.aspose.zip/lzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class LzmaCompressionSettings extends CompressionSettings
```

LZMA 圧縮方式の設定。

Lempel–Ziv–Markov 連鎖アルゴリズム (LZMA) は、ロスレスデータ圧縮を実行するために使用されるアルゴリズムです。このアルゴリズムは、LZ77 アルゴリズムにやや似た辞書圧縮方式を使用し、高い圧縮率と可変の圧縮辞書サイズを特徴とします。

詳細はこちら: [Lempel\u2013Ziv\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [LzmaCompressionSettings()](#LzmaCompressionSettings--) | デフォルトパラメータで [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) クラスの新しいインスタンスを初期化します。 |
| [LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#LzmaCompressionSettings-int-int-int-) | 指定された辞書サイズ、ファストバイト数、リテラルコンテキストビット数で [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) クラスの新しいインスタンスを初期化します。 |
| [LzmaCompressionSettings(int dictionarySize)](#LzmaCompressionSettings-int-) | 指定された辞書サイズ、デフォルトのファストバイト数（32）およびリテラルコンテキストビット数（3）で [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | 辞書（履歴バッファ）サイズは、最近処理された非圧縮データがメモリに保持されるバイト数を示します。 |
| [getLiteralContextBits()](#getLiteralContextBits--) | リテラルコンテキストビット数を取得します。 |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | LZMA アルゴリズムで高速マッチ検索に使用されるバイト数を取得します。 |
### LzmaCompressionSettings() {#LzmaCompressionSettings--}
```
public LzmaCompressionSettings()
```


デフォルトパラメータで [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) クラスの新しいインスタンスを初期化します。

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



### LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits) {#LzmaCompressionSettings-int-int-int-}
```
public LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)
```


Initializes a new instance of the [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) class with specified dictionary size, number of fast bytes and number of literal context bits.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824. |
| numberOfFastBytes | int | The number of bytes used for fast match searching in the LZMA algorithm. Can be in the range from 5 to 273. |
| literalContextBits | int | Sets the number of literal context bits (high bits of previous literal). It can be in range from 0 to 8. |

### LzmaCompressionSettings(int dictionarySize) {#LzmaCompressionSettings-int-}
```
public LzmaCompressionSettings(int dictionarySize)
```


Initializes a new instance of the [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) class with specified dictionary size, default number of fast bytes equal to 32 and number of literal context bits equal to 3.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824. |

### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM.

**Returns:**
int - how many bytes of the recently processed uncompressed data are kept in memory.
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


Gets the number of literal context bits.

Literal Context Bits define how many of the most significant bits of the previous uncompressed byte are used to predict the bits of the next literal byte. Must be from 0 to 8.

**Returns:**
int - the number of literal context bits.
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


Gets the number of bytes used for fast match searching in the LZMA algorithm.

A higher value allows the compressor to search longer matches, which can improve the compression ratio slightly but slows down compression.

**Returns:**
int - the number of bytes used for fast match searching in the LZMA algorithm.
