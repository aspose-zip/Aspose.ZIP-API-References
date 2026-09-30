---
title: "クラス LzipArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Lzip.LzipArchive クラス。このクラスは Lzip アーカイブ ファイルを表します。Lzip アーカイブの作成または抽出に使用します。"
type: docs
weight: 700
url: /ja/net/aspose.zip.lzip/lziparchive/
---
## LzipArchive class

このクラスは Lzip アーカイブ ファイルを表します。Lzip アーカイブの作成または抽出に使用します。

```csharp
public class LzipArchive : IArchive, IArchiveFileEntry
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [LzipArchive](lziparchive/#constructor)(LzipArchiveSettings) | `LzipArchive` の新しいインスタンスを初期化します。 |
| [LzipArchive](lziparchive/#constructor_1)(Stream, LzipLoadOptions) | 解凍用に準備された `LzipArchive` クラスの新しいインスタンスを初期化します。 |
| [LzipArchive](lziparchive/#constructor_2)(string, LzipLoadOptions) | 解凍用に準備された `LzipArchive` クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Settings](../../aspose.zip.lzip/lziparchive/settings/) { get; } | 特定の lzip アーカイブの設定を取得します。 |
| [UncompressedSize](../../aspose.zip.lzip/lziparchive/uncompressedsize/) { get; } | ファイルデータの非圧縮サイズ（バイト単位）。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Dispose](../../aspose.zip.lzip/lziparchive/dispose/)() | アンマネージド リソースの解放、リリース、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [Extract](../../aspose.zip.lzip/lziparchive/extract/#extract)(FileInfo) | lzip アーカイブをファイルに抽出します。 |
| [Extract](../../aspose.zip.lzip/lziparchive/extract/#extract_1)(Stream) | lzip アーカイブをストリームに抽出します。 |
| [Extract](../../aspose.zip.lzip/lziparchive/extract/#extract_2)(string) | パスで指定したファイルに lzip アーカイブを抽出します。 |
| [ExtractToDirectory](../../aspose.zip.lzip/lziparchive/extracttodirectory/)(string) | 提供されたディレクトリにアーカイブの内容を抽出します。 |
| [Save](../../aspose.zip.lzip/lziparchive/save/#save)(FileInfo) | 指定された宛先ファイルに lzip アーカイブを保存します。 |
| [Save](../../aspose.zip.lzip/lziparchive/save/#save_1)(Stream) | 指定されたストリームに lzip アーカイブを保存します。 |
| [Save](../../aspose.zip.lzip/lziparchive/save/#save_2)(string) | 指定された宛先ファイルに lzip アーカイブを保存します。 |
| [SetSource](../../aspose.zip.lzip/lziparchive/setsource/#setsource)(FileInfo) | アーカイブ内で圧縮される内容を設定します。 |
| [SetSource](../../aspose.zip.lzip/lziparchive/setsource/#setsource_1)(Stream) | アーカイブ内で圧縮される内容を設定します。 |
| [SetSource](../../aspose.zip.lzip/lziparchive/setsource/#setsource_2)(string) | アーカイブ内で圧縮される内容を設定します。 |

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Lzip](../../aspose.zip.lzip/)
* assembly [Aspose.Zip](../../)


