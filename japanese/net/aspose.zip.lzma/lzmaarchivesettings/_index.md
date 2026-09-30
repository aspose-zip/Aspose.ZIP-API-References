---
title: "クラス LzmaArchiveSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.LZMA.LzmaArchiveSettings クラス。lzma アーカイブの設定"
type: docs
weight: 620
url: /ja/net/aspose.zip.lzma/lzmaarchivesettings/
---
## LzmaArchiveSettings class

lzma アーカイブの設定です。

```csharp
public class LzmaArchiveSettings
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [LzmaArchiveSettings](lzmaarchivesettings/)() | `LzmaArchiveSettings` クラスの新しいインスタンスを初期化します（デフォルトの辞書サイズは 16 メガバイト、ファストバイト数は 32、リテラルコンテキストビットは 3 に設定）。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [DictionarySize](../../aspose.zip.lzma/lzmaarchivesettings/dictionarysize/) { get; set; } | 辞書（履歴バッファ）のサイズは、最近処理された非圧縮データがメモリに保持されるバイト数を示します。設定されていない場合、エントリサイズに応じて自動的に選択されます。 |
| [LiteralContextBits](../../aspose.zip.lzma/lzmaarchivesettings/literalcontextbits/) { get; set; } | リテラルコンテキストビット数を取得または設定します。 |
| [NumberOfFastBytes](../../aspose.zip.lzma/lzmaarchivesettings/numberoffastbytes/) { get; set; } | LZMA アルゴリズムで高速マッチ検索に使用されるバイト数を取得または設定します。 |

## イベント

| 名前 | 説明 |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.lzma/lzmaarchivesettings/compressionprogressed/) | 生ストリームの一部が圧縮されたときに発生します。 |

## 備考

Lempel–Ziv–Markov 連鎖アルゴリズム（LZMA）は、ロスレスデータ圧縮を行うアルゴリズムです。このアルゴリズムは LZ77 アルゴリズムにやや似た辞書圧縮方式を使用し、高い圧縮率と可変の圧縮辞書サイズを特徴とします。

詳しくは: [Lempel–Ziv–Markov 連鎖アルゴリズム](https://en.wikipedia.org/wiki/Lempel–Ziv–Markov_chain_algorithm)

### 関連項目

* namespace [Aspose.Zip.LZMA](../../aspose.zip.lzma/)
* assembly [Aspose.Zip](../../)


