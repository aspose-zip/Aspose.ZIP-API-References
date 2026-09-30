---
title: "クラス LzmaCompressionSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Saving.LzmaCompressionSettings クラス。ZIP アーカイブ内の LZMA 圧縮の設定です。"
type: docs
weight: 960
url: /ja/net/aspose.zip.saving/lzmacompressionsettings/
---
## LzmaCompressionSettings class

ZIP アーカイブ内の LZMA 圧縮の設定。

```csharp
public class LzmaCompressionSettings : CompressionSettings
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [LzmaCompressionSettings](lzmacompressionsettings/#constructor)() | `LzmaCompressionSettings` クラスの新しいインスタンスをデフォルト パラメーターで初期化します。 |
| [LzmaCompressionSettings](lzmacompressionsettings/#constructor_1)(int) | `LzmaCompressionSettings` クラスの新しいインスタンスを、指定された辞書サイズ、デフォルトの高速バイト数 32、リテラルコンテキストビット数 3 で初期化します。 |
| [LzmaCompressionSettings](lzmacompressionsettings/#constructor_2)(int, int, int) | `LzmaCompressionSettings` クラスの新しいインスタンスを、指定された辞書サイズ、ファストバイト数、リテラルコンテキストビット数で初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [DictionarySize](../../aspose.zip.saving/lzmacompressionsettings/dictionarysize/) { get; } | 辞書（履歴バッファ）サイズは、最近処理された非圧縮データがメモリに保持されるバイト数を示します。 |
| [LiteralContextBits](../../aspose.zip.saving/lzmacompressionsettings/literalcontextbits/) { get; } | リテラルコンテキストビット数を取得します。 |
| [NumberOfFastBytes](../../aspose.zip.saving/lzmacompressionsettings/numberoffastbytes/) { get; } | LZMA アルゴリズムで高速マッチ検索に使用されるバイト数を取得します。 |

## 備考

Lempel–Ziv–Markov 連鎖アルゴリズム（LZMA）は、ロスレスデータ圧縮を行うアルゴリズムです。このアルゴリズムは LZ77 アルゴリズムにやや似た辞書圧縮方式を使用し、高い圧縮率と可変の圧縮辞書サイズを特徴とします。

詳しくは: [Lempel–Ziv–Markov 連鎖アルゴリズム](https://en.wikipedia.org/wiki/Lempel–Ziv–Markov_chain_algorithm)

### 関連項目

* class [CompressionSettings](../compressionsettings/)
* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


