---
title: "クラス GzipArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Gzip.GzipArchive クラス。このクラスは gzip アーカイブファイルを表します。gzip アーカイブの作成または抽出に使用します。"
type: docs
weight: 510
url: /ja/net/aspose.zip.gzip/gziparchive/
---
## GzipArchive class

このクラスは gzip アーカイブファイルを表します。gzip アーカイブの作成または抽出に使用します。

```csharp
public class GzipArchive : IArchive, IArchiveFileEntry
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [GzipArchive](gziparchive/#constructor)() | `GzipArchive` クラスの新しいインスタンスを初期化し、圧縮用に準備します。 |
| [GzipArchive](gziparchive/#constructor_2)(Stream, bool) | `GzipArchive` クラスの新しいインスタンスを初期化し、解凍用に準備します。 |
| [GzipArchive](gziparchive/#constructor_1)(Stream, GzipLoadOptions) | `GzipArchive` クラスの新しいインスタンスを初期化し、解凍用に準備します。 |
| [GzipArchive](gziparchive/#constructor_4)(string, bool) | `GzipArchive` クラスの新しいインスタンスを初期化し、解凍用に準備します。 |
| [GzipArchive](gziparchive/#constructor_3)(string, GzipLoadOptions) | `GzipArchive` クラスの新しいインスタンスを初期化し、解凍用に準備します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Name](../../aspose.zip.gzip/gziparchive/name/) { get; } | 元のファイル名。 |
| [UncompressedSize](../../aspose.zip.gzip/gziparchive/uncompressedsize/) { get; } | 元のファイルのサイズを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Dispose](../../aspose.zip.gzip/gziparchive/dispose/)() | アンマネージド リソースの解放、リリース、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/#extract_1)(Stream) | 提供されたストリームへアーカイブを抽出します。 |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/#extract)(string) | パスで指定されたファイルへアーカイブを抽出します。 |
| [ExtractToDirectory](../../aspose.zip.gzip/gziparchive/extracttodirectory/)(string) | 提供されたディレクトリにアーカイブの内容を抽出します。 |
| [Open](../../aspose.zip.gzip/gziparchive/open/)() | 抽出用にアーカイブを開き、アーカイブ内容のストリームを提供します。 |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save)(Stream) | アーカイブを指定されたストリームに保存します。 |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save_1)(string) | アーカイブを指定された宛先ファイルに保存します。 |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_1)(FileInfo) | アーカイブ内で圧縮される内容を設定します。 |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_2)(Stream) | アーカイブ内で圧縮される内容を設定します。 |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_3)(string) | アーカイブ内で圧縮される内容を設定します。 |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource)(TarArchive) | アーカイブ内で圧縮される内容を設定します。 |

## 備考

Gzip 圧縮アルゴリズムは DEFLATE アルゴリズムに基づいており、LZ77 とハフマン符号化の組み合わせです。

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Gzip](../../aspose.zip.gzip/)
* assembly [Aspose.Zip](../../)


