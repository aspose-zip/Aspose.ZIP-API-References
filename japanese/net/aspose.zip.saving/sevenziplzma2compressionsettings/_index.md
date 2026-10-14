---
title: "クラス SevenZipLZMA2CompressionSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Saving.SevenZipLZMA2CompressionSettings クラス。7z アーカイブ内の LZMA2 圧縮方式の設定"
type: docs
weight: 1080
url: /ja/net/aspose.zip.saving/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings class

7z アーカイブ内の LZMA2 圧縮方式の設定。

```csharp
public class SevenZipLZMA2CompressionSettings : SevenZipCompressionSettings
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [SevenZipLZMA2CompressionSettings](sevenziplzma2compressionsettings/#constructor)(int) | 7z アーカイブ内の LZMA2 圧縮方式の設定をインスタンス化します。 |
| [SevenZipLZMA2CompressionSettings](sevenziplzma2compressionsettings/#constructor_1)(int, int) | 7z アーカイブ内の LZMA2 圧縮方式の設定をインスタンス化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [CompressionThreads](../../aspose.zip.saving/sevenziplzma2compressionsettings/compressionthreads/) { get; set; } | 圧縮スレッド数を取得または設定します。値が 1 より大きい場合、マルチスレッド圧縮が使用されます。 |
| [DictionarySize](../../aspose.zip.saving/sevenziplzma2compressionsettings/dictionarysize/) { get; } | 辞書（履歴バッファ）サイズは、最近処理された非圧縮データがメモリに保持されるバイト数を示します。 |
| [FastBytes](../../aspose.zip.saving/sevenziplzma2compressionsettings/fastbytes/) { get; } | LZMA2 コンプレッサーで使用される高速バイト数の制御番号を取得します。 |
| override [Method](../../aspose.zip.saving/sevenziplzma2compressionsettings/method/) { get; } | 圧縮または解凍の方法を取得します。 |

## 備考

LZMA2 は圧縮された LZMA データと非圧縮データの複数のランをサポートします。

詳しくは: [Lempel–Ziv–Markov 連鎖アルゴリズム](https://en.wikipedia.org/wiki/Lempel–Ziv–Markov_chain_algorithm)

### 関連項目

* class [SevenZipCompressionSettings](../sevenzipcompressionsettings/)
* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


