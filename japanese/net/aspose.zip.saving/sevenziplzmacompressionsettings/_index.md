---
title: "クラス SevenZipLZMACompressionSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Saving.SevenZipLZMACompressionSettings クラス。7z アーカイブ内の LZMA 圧縮方式の設定"
type: docs
weight: 1090
url: /ja/net/aspose.zip.saving/sevenziplzmacompressionsettings/
---
## SevenZipLZMACompressionSettings class

7z アーカイブ内の LZMA 圧縮方式の設定。

```csharp
public class SevenZipLZMACompressionSettings : SevenZipCompressionSettings
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [SevenZipLZMACompressionSettings](sevenziplzmacompressionsettings/#constructor)() | `SevenZipLZMACompressionSettings` クラスの新しいインスタンスをデフォルトパラメーターで初期化します。 |
| [SevenZipLZMACompressionSettings](sevenziplzmacompressionsettings/#constructor_1)(int) | `SevenZipLZMACompressionSettings` クラスの新しいインスタンスを、指定された辞書サイズ、ファストバイト数を 32、リテラルコンテキストビット数を 3 に設定して初期化します。 |
| [SevenZipLZMACompressionSettings](sevenziplzmacompressionsettings/#constructor_2)(int, int, int) | `SevenZipLZMACompressionSettings` クラスの新しいインスタンスを、指定された辞書サイズ、ファストバイト数、リテラルコンテキストビット数で初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [DictionarySize](../../aspose.zip.saving/sevenziplzmacompressionsettings/dictionarysize/) { get; set; } | 辞書（履歴バッファ）サイズは、最近処理された非圧縮データがメモリに保持されるバイト数を示します。設定されていない場合、エントリサイズに応じて自動的に選択されます。サイズは 4096 から 1073741824 の間である必要があり、エントリサイズに基づく自動検出の場合は 0 を指定できます。 |
| [LiteralContextBits](../../aspose.zip.saving/sevenziplzmacompressionsettings/literalcontextbits/) { get; } | リテラルコンテキストビット数を取得します。 |
| override [Method](../../aspose.zip.saving/sevenziplzmacompressionsettings/method/) { get; } | 圧縮または解凍の方法を取得します。 |
| [NumberOfFastBytes](../../aspose.zip.saving/sevenziplzmacompressionsettings/numberoffastbytes/) { get; } | LZMA アルゴリズムで高速マッチ検索に使用されるバイト数を取得します。 |

## 備考

Lempel–Ziv–Markov 連鎖アルゴリズム（LZMA）は、ロスレスデータ圧縮を行うアルゴリズムです。このアルゴリズムは LZ77 アルゴリズムにやや似た辞書圧縮方式を使用し、高い圧縮率と可変の圧縮辞書サイズを特徴とします。

詳しくは: [Lempel–Ziv–Markov 連鎖アルゴリズム](https://en.wikipedia.org/wiki/Lempel–Ziv–Markov_chain_algorithm)

### 関連項目

* class [SevenZipCompressionSettings](../sevenzipcompressionsettings/)
* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


