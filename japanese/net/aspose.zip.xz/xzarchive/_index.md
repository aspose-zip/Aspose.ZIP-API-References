---
title: "クラス XzArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Xz.XzArchive クラス。このクラスは xz アーカイブ ファイルを表します。xz アーカイブの作成と抽出に使用します。"
type: docs
weight: 1580
url: /ja/net/aspose.zip.xz/xzarchive/
---
## XzArchive class

このクラスは xz アーカイブ ファイルを表します。xz アーカイブの作成および抽出に使用します。

```csharp
public class XzArchive : IArchive, IArchiveFileEntry
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [XzArchive](xzarchive/#constructor)(XzArchiveSettings) | `XzArchive` クラスの新しいインスタンスを初期化し、xz 形式でアーカイブを作成します。 |
| [XzArchive](xzarchive/#constructor_1)(Stream, XzLoadOptions) | 解凍用に準備された `XzArchive` クラスの新しいインスタンスを初期化します。 |
| [XzArchive](xzarchive/#constructor_2)(string, XzLoadOptions) | 解凍用に準備された `XzArchive` クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [UncompressedSize](../../aspose.zip.xz/xzarchive/uncompressedsize/) { get; } | ファイルデータの非圧縮サイズ（バイト単位）。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Dispose](../../aspose.zip.xz/xzarchive/dispose/)() | アンマネージド リソースの解放、リリース、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [Extract](../../aspose.zip.xz/xzarchive/extract/#extract_1)(FileInfo) | xz アーカイブをファイルに抽出します。 |
| [Extract](../../aspose.zip.xz/xzarchive/extract/#extract_2)(Stream) | xz アーカイブをストリームに抽出します。 |
| [Extract](../../aspose.zip.xz/xzarchive/extract/#extract)(string) | パスで指定されたファイルに xz アーカイブを抽出します。 |
| [ExtractToDirectory](../../aspose.zip.xz/xzarchive/extracttodirectory/)(string) | 提供されたディレクトリにアーカイブの内容を抽出します。 |
| [Save](../../aspose.zip.xz/xzarchive/save/#save)(Stream) | 提供されたストリームに xz アーカイブを保存します。 |
| [Save](../../aspose.zip.xz/xzarchive/save/#save_1)(string) | 指定された宛先ファイルに xz アーカイブを保存します。 |
| [SetSource](../../aspose.zip.xz/xzarchive/setsource/#setsource)(FileInfo) | アーカイブ内で圧縮される内容を設定します。 |
| [SetSource](../../aspose.zip.xz/xzarchive/setsource/#setsource_1)(Stream) | アーカイブ内で圧縮される内容を設定します。 |
| [SetSource](../../aspose.zip.xz/xzarchive/setsource/#setsource_2)(string) | アーカイブ内で圧縮される内容を設定します。 |

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Xz](../../aspose.zip.xz/)
* assembly [Aspose.Zip](../../)


