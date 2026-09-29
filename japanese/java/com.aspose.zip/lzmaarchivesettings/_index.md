---
title: "LzmaArchiveSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "lzma アーカイブの設定。"
type: docs
weight: 87
url: /ja/java/com.aspose.zip/lzmaarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzmaArchiveSettings
```

lzma アーカイブの設定。

Lempel–Ziv–Markov 連鎖アルゴリズム (LZMA) は、ロスレスデータ圧縮を実行するために使用されるアルゴリズムです。このアルゴリズムは、LZ77 アルゴリズムにやや似た辞書圧縮方式を使用し、高い圧縮率と可変の圧縮辞書サイズを特徴とします。

詳細はこちら: [Lempel\u2013Ziv\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [LzmaArchiveSettings()](#LzmaArchiveSettings--) | デフォルトの辞書サイズ 16 メガバイト、ファストバイト数 32、リテラルコンテキストビット数 3 を持つ [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | 生ストリームの一部が圧縮されたときに発生するイベントを取得します。 |
| [getDictionarySize()](#getDictionarySize--) | 辞書（履歴バッファ）サイズは、最近処理された非圧縮データがメモリに保持されるバイト数を示します。 |
| [getLiteralContextBits()](#getLiteralContextBits--) | リテラルコンテキストビット数を取得します。 |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | LZMA アルゴリズムで高速マッチ検索に使用されるバイト数を取得します。 |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | 生ストリームの一部が圧縮されたときに発生するイベントを設定します。 |
| [setDictionarySize(int value)](#setDictionarySize-int-) | 辞書（履歴バッファ）サイズは、最近処理された非圧縮データがメモリに保持されるバイト数を示します。 |
| [setLiteralContextBits(int value)](#setLiteralContextBits-int-) | リテラルコンテキストビット数を設定します。 |
| [setNumberOfFastBytes(int value)](#setNumberOfFastBytes-int-) | LZMA アルゴリズムで高速マッチ検索に使用されるバイト数を設定します。 |
### LzmaArchiveSettings() {#LzmaArchiveSettings--}
```
public LzmaArchiveSettings()
```


デフォルトの辞書サイズ 16 メガバイト、ファストバイト数 32、リテラルコンテキストビット数 3 を持つ [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) クラスの新しいインスタンスを初期化します。

```

``````

LzmaArchiveSettings settings = new LzmaArchiveSettings();
settings.setDictionarySize(1048576);
try (LzmaArchive archive = new LzmaArchive(settings)) {
archive.setSource("data.bin");
archive.save(lzmaFile);
}
 
```



### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Gets an event that is raised when a portion of raw stream compressed.

```

``````

    lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```



**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Dictionary (history buffer) のサイズは、最近処理された非圧縮データがメモリに保持されるバイト数を示します。設定されていない場合、エントリサイズに応じて自動的に選択されます。

辞書が大きいほど、通常は圧縮率が向上しますが、非圧縮データよりも大きな辞書は RAM の無駄になります。LZMA アーカイブの辞書サイズは、2 のべき乗 (2^n) または 2 のべき乗の 3 倍 (3\*2^n) のいずれかでなければなりません。

**Returns:**
int - Dictionary (history buffer) のサイズ。
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


リテラルコンテキストビット数を取得します。

Literal Context Bits は、前の非圧縮バイトの上位ビットが次のリテラルバイトのビットを予測するために使用されるビット数を定義します。0 から 8 の範囲で指定する必要があります。

**Returns:**
int - リテラルコンテキストビットの数。
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


LZMA アルゴリズムで高速マッチ検索に使用されるバイト数を取得します。

値を大きくすると、圧縮器がより長い一致を検索できるようになり、圧縮率がわずかに向上する可能性がありますが、圧縮速度が低下します。

**Returns:**
int - LZMA アルゴリズムで高速一致検索に使用されるバイト数。
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


生ストリームの一部が圧縮されたときに発生するイベントを設定します。

```

``````

lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when a portion of raw stream compressed |

### setDictionarySize(int value) {#setDictionarySize-int-}
```
public final void setDictionarySize(int value)
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory. If not set, will be chosen accordingly to entry size.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM. The disctionary size of LZMA archive must be either a power of two (2^n) or three times a power of two (3\*2^n).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | Dictionary (history buffer) size. |

### setLiteralContextBits(int value) {#setLiteralContextBits-int-}
```
public final void setLiteralContextBits(int value)
```


Sets the number of literal context bits.

Literal Context Bits define how many of the most significant bits of the previous uncompressed byte are used to predict the bits of the next literal byte. Must be from 0 to 8.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of literal context bits. |

### setNumberOfFastBytes(int value) {#setNumberOfFastBytes-int-}
```
public final void setNumberOfFastBytes(int value)
```


Sets the number of bytes used for fast match searching in the LZMA algorithm.

A higher value allows the compressor to search longer matches, which can improve the compression ratio slightly but slows down compression.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of bytes used for fast match searching in the LZMA algorithm. |

