---
title: "クラス CabArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Cab.CabArchive クラス。このクラスは CAB アーカイブ ファイルを表します。"
type: docs
weight: 310
url: /ja/net/aspose.zip.cab/cabarchive/
---
## CabArchive class

このクラスは CAB アーカイブ ファイルを表します。

```csharp
public class CabArchive : IArchive
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [CabArchive](cabarchive/#constructor)(CabEntrySettings) | 圧縮用に準備された `CabArchive` クラスの新しいインスタンスを初期化します。 |
| [CabArchive](cabarchive/#constructor_1)(Stream, CabLoadOptions) | 新しい `CabArchive` クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。 |
| [CabArchive](cabarchive/#constructor_2)(string, CabLoadOptions) | 新しい `CabArchive` クラスのインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Entries](../../aspose.zip.cab/cabarchive/entries/) { get; } | アーカイブを構成する [`CabEntry`](../cabentry/) 型のエントリを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [CreateEntries](../../aspose.zip.cab/cabarchive/createentries/#createentries)(DirectoryInfo, bool) | 指定されたディレクトリからすべてのファイルを再帰的にアーカイブに追加します。 |
| [CreateEntries](../../aspose.zip.cab/cabarchive/createentries/#createentries_1)(string, bool) | 指定されたディレクトリパスからすべてのファイルを再帰的にアーカイブに追加します。 |
| [CreateEntry](../../aspose.zip.cab/cabarchive/createentry/#createentry_1)(string, FileInfo, CabEntrySettings) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.cab/cabarchive/createentry/#createentry)(string, Func&lt;Stream&gt;, CabEntrySettings) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.cab/cabarchive/createentry/#createentry_2)(string, Stream, CabEntrySettings) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.cab/cabarchive/createentry/#createentry_3)(string, string, CabEntrySettings) | アーカイブ内に単一のエントリを作成します。 |
| [Dispose](../../aspose.zip.cab/cabarchive/dispose/)() | アンマネージド リソースの解放、リリース、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [ExtractToDirectory](../../aspose.zip.cab/cabarchive/extracttodirectory/)(string) | アーカイブ内のすべてのファイルを指定されたディレクトリに抽出します。 |
| [Save](../../aspose.zip.cab/cabarchive/save/#save)(Stream, CabSaveOptions) | アーカイブを指定されたストリームに保存します。 |
| [Save](../../aspose.zip.cab/cabarchive/save/#save_1)(string, CabSaveOptions) | アーカイブを指定された宛先ファイルに保存します。 |

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Cab](../../aspose.zip.cab/)
* assembly [Aspose.Zip](../../)


