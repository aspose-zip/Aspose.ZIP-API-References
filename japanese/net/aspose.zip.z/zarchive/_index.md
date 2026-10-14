---
title: "クラス ZArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Z.ZArchive クラス。このクラスは Z 圧縮アーカイブファイルを表します。Z アーカイブの作成または抽出に使用します。"
type: docs
weight: 1590
url: /ja/net/aspose.zip.z/zarchive/
---
## ZArchive class

このクラスは Z（圧縮）アーカイブ ファイルを表します。Z アーカイブの作成や抽出に使用してください。

```csharp
public class ZArchive : IArchive, IArchiveFileEntry
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [ZArchive](zarchive/#constructor)() | 圧縮用に準備された `ZArchive` クラスの新しいインスタンスを初期化します。 |
| [ZArchive](zarchive/#constructor_1)(Stream, ZArchiveLoadOptions) | 解凍用に準備された `ZArchive` クラスの新しいインスタンスを初期化します。 |
| [ZArchive](zarchive/#constructor_2)(string, ZArchiveLoadOptions) | 解凍用に準備された `ZArchive` クラスの新しいインスタンスを初期化します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Dispose](../../aspose.zip.z/zarchive/dispose/)() | アンマネージド リソースの解放、リリース、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [Extract](../../aspose.zip.z/zarchive/extract/#extract_1)(FileInfo) | Z アーカイブをファイルに抽出します。 |
| [Extract](../../aspose.zip.z/zarchive/extract/#extract_2)(Stream) | Z アーカイブをストリームに抽出します。 |
| [Extract](../../aspose.zip.z/zarchive/extract/#extract)(string) | パスで指定されたファイルに Z アーカイブを抽出します。 |
| [ExtractToDirectory](../../aspose.zip.z/zarchive/extracttodirectory/)(string) | 提供されたディレクトリにアーカイブの内容を抽出します。 |
| [Save](../../aspose.zip.z/zarchive/save/#save)(Stream, ZArchiveSaveOptions) | 提供されたストリームに xz アーカイブを保存します。 |
| [Save](../../aspose.zip.z/zarchive/save/#save_1)(string, ZArchiveSaveOptions) | 提供された宛先ファイルに Z アーカイブを保存します。 |
| [SetSource](../../aspose.zip.z/zarchive/setsource/#setsource)(FileInfo) | アーカイブ内で圧縮される内容を設定します。 |
| [SetSource](../../aspose.zip.z/zarchive/setsource/#setsource_1)(Stream) | アーカイブ内で圧縮される内容を設定します。 |
| [SetSource](../../aspose.zip.z/zarchive/setsource/#setsource_2)(string) | アーカイブ内で圧縮される内容を設定します。 |

## 備考

参照してください https://docs.fileformat.com/compression/z/

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Z](../../aspose.zip.z/)
* assembly [Aspose.Zip](../../)


