---
title: "クラス ZstandardArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Zstandard.ZstandardArchive クラス。 このクラスは Zstandard アーカイブファイルを表します。 Zstandard アーカイブを作成するために使用します。"
type: docs
weight: 1620
url: /ja/net/aspose.zip.zstandard/zstandardarchive/
---
## ZstandardArchive class

このクラスは Zstandard アーカイブ ファイルを表します。Zstandard アーカイブの作成に使用します。

```csharp
public class ZstandardArchive : IArchive, IArchiveFileEntry
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [ZstandardArchive](zstandardarchive/#constructor)() | `ZstandardArchive` クラスの新しいインスタンスを初期化し、圧縮用に準備します。 |
| [ZstandardArchive](zstandardarchive/#constructor_1)(Stream, ZstandardLoadOptions) | `ZstandardArchive` クラスの新しいインスタンスを初期化し、解凍用に準備します。 |
| [ZstandardArchive](zstandardarchive/#constructor_2)(string, ZstandardLoadOptions) | `ZstandardArchive` クラスの新しいインスタンスを初期化します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Dispose](../../aspose.zip.zstandard/zstandardarchive/dispose/)() | アンマネージド リソースの解放、リリース、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [Extract](../../aspose.zip.zstandard/zstandardarchive/extract/#extract_1)(Stream) | 提供されたストリームへアーカイブを抽出します。 |
| [Extract](../../aspose.zip.zstandard/zstandardarchive/extract/#extract)(string) | パスで指定されたファイルへアーカイブを抽出します。 |
| [ExtractToDirectory](../../aspose.zip.zstandard/zstandardarchive/extracttodirectory/)(string) | 提供されたディレクトリにアーカイブの内容を抽出します。 |
| [Open](../../aspose.zip.zstandard/zstandardarchive/open/)() | 抽出用にアーカイブを開き、アーカイブ内容のストリームを提供します。 |
| [Save](../../aspose.zip.zstandard/zstandardarchive/save/#save)(FileInfo, ZstandardSaveOptions) | アーカイブを指定された宛先ファイルに保存します。 |
| [Save](../../aspose.zip.zstandard/zstandardarchive/save/#save_1)(Stream, ZstandardSaveOptions) | アーカイブを指定されたストリームに保存します。 |
| [Save](../../aspose.zip.zstandard/zstandardarchive/save/#save_2)(string, ZstandardSaveOptions) | アーカイブを指定された宛先ファイルに保存します。 |
| [SetSource](../../aspose.zip.zstandard/zstandardarchive/setsource/#setsource)(FileInfo) | アーカイブ内で圧縮される内容を設定します。 |
| [SetSource](../../aspose.zip.zstandard/zstandardarchive/setsource/#setsource_1)(Stream) | アーカイブ内で圧縮される内容を設定します。 |
| [SetSource](../../aspose.zip.zstandard/zstandardarchive/setsource/#setsource_2)(string) | アーカイブ内で圧縮される内容を設定します。 |

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Zstandard](../../aspose.zip.zstandard/)
* assembly [Aspose.Zip](../../)


