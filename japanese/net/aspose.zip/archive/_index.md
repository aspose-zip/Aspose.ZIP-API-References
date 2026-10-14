---
title: "クラス Archive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Archive クラス。このクラスはZIPアーカイブファイルを表します。ZIPアーカイブの作成、抽出、または更新に使用します。"
type: docs
weight: 160
url: /ja/net/aspose.zip/archive/
---
## Archive class

このクラスは zip アーカイブファイルを表します。zip アーカイブの作成、抽出、または更新に使用します。

```csharp
public class Archive : IArchive
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [Archive](archive/#constructor)(ArchiveEntrySettings) | `Archive` クラスの新しいインスタンスを、エントリのオプション設定とともに初期化します。 |
| [Archive](archive/#constructor_1)(Stream, ArchiveLoadOptions, ArchiveEntrySettings) | `Archive` クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを作成します。 |
| [Archive](archive/#constructor_2)(string, ArchiveLoadOptions, ArchiveEntrySettings) | `Archive` クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを作成します。 |
| [Archive](archive/#constructor_3)(string, string[], ArchiveLoadOptions) | マルチボリュームZIPアーカイブから `Archive` クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを作成します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Comment](../../aspose.zip/archive/comment/) { get; } | アーカイブ全体のコメントを取得します。 |
| [Entries](../../aspose.zip/archive/entries/) { get; } | アーカイブを構成する [`ArchiveEntry`](../archiveentry/) 型のエントリを取得します。 |
| [NewEntrySettings](../../aspose.zip/archive/newentrysettings/) { get; } | 新しく追加された [`ArchiveEntry`](../archiveentry/) アイテムに使用される圧縮および暗号化設定。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries)(DirectoryInfo, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries_1)(string, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry)(string, Func&lt;Stream&gt;, ArchiveEntrySettings) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_2)(string, Stream, ArchiveEntrySettings) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_1)(string, FileInfo, bool, ArchiveEntrySettings) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_3)(string, Stream, ArchiveEntrySettings, FileSystemInfo) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_4)(string, string, bool, ArchiveEntrySettings) | アーカイブ内に単一のエントリを作成します。 |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry)(ArchiveEntry) | エントリリストから特定のエントリの最初の出現を削除します。 |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry_1)(int) | インデックスでエントリリストからエントリを削除します。 |
| [Dispose](../../aspose.zip/archive/dispose/)() | アンマネージド リソースの解放、リリース、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [ExtractToDirectory](../../aspose.zip/archive/extracttodirectory/)(string) | アーカイブ内のすべてのファイルを指定されたディレクトリに抽出します。 |
| [Save](../../aspose.zip/archive/save/#save)(Stream, ArchiveSaveOptions) | アーカイブを指定されたストリームに保存します。 |
| [Save](../../aspose.zip/archive/save/#save_1)(string, ArchiveSaveOptions) | アーカイブを指定された宛先ファイルに保存します。 |
| [SaveSplit](../../aspose.zip/archive/savesplit/#savesplit)(IVolumeStreamProvider, SplitArchiveSaveOptions) | ボリュームプロバイダーが提供するストリームにマルチボリューム アーカイブを保存します。 |
| [SaveSplit](../../aspose.zip/archive/savesplit/#savesplit_1)(string, SplitArchiveSaveOptions) | 指定された宛先ディレクトリにマルチボリューム アーカイブを保存します。 |

### 関連項目

* interface [IArchive](../iarchive/)
* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)


