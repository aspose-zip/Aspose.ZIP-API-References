---
title: "クラス XarArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Xar.XarArchive クラス。このクラスは xar アーカイブファイルを表します"
type: docs
weight: 1420
url: /ja/net/aspose.zip.xar/xararchive/
---
## XarArchive class

このクラスは xar アーカイブ ファイルを表します。

```csharp
public class XarArchive : IArchive
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [XarArchive](xararchive/#constructor)(XarCompressionSettings) | `XarArchive` クラスの新しいインスタンスを初期化します。 |
| [XarArchive](xararchive/#constructor_1)(Stream, XarLoadOptions) | `XarArchive` クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。 |
| [XarArchive](xararchive/#constructor_2)(string, XarLoadOptions) | `XarArchive` クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Entries](../../aspose.zip.xar/xararchive/entries/) { get; } | アーカイブを構成する [`XarEntry`](../xarentry/) タイプのエントリを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [CreateEntries](../../aspose.zip.xar/xararchive/createentries/#createentries)(DirectoryInfo, bool, XarCompressionSettings) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntries](../../aspose.zip.xar/xararchive/createentries/#createentries_1)(string, bool, XarCompressionSettings) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntry](../../aspose.zip.xar/xararchive/createentry/#createentry_1)(string, Stream, XarCompressionSettings) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.xar/xararchive/createentry/#createentry)(string, FileInfo, bool, XarCompressionSettings) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.xar/xararchive/createentry/#createentry_2)(string, string, bool, XarCompressionSettings) | アーカイブ内に単一のエントリを作成します。 |
| [DeleteEntry](../../aspose.zip.xar/xararchive/deleteentry/)(XarEntry) | エントリ リストから特定のエントリの最初の出現を削除します。 |
| [Dispose](../../aspose.zip.xar/xararchive/dispose/)() | アンマネージド リソースの解放、リリース、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [ExtractToDirectory](../../aspose.zip.xar/xararchive/extracttodirectory/)(string) | アーカイブ内のすべてのファイルを指定されたディレクトリに抽出します。 |
| [Save](../../aspose.zip.xar/xararchive/save/#save)(Stream, XarSaveOptions) | アーカイブを指定されたストリームに保存します。 |
| [Save](../../aspose.zip.xar/xararchive/save/#save_1)(string, XarSaveOptions) | アーカイブを指定された宛先ファイルに保存します。 |

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Xar](../../aspose.zip.xar/)
* assembly [Aspose.Zip](../../)


