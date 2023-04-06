---
title: Class Archive
second_title: Aspose.ZIP for .NET API リファレンス
description: Aspose.Zip.Archive クラス. このクラスはzip アーカイブ ファイルを表しますこれを使用してzip アーカイブを作成抽出または更新します
type: docs
weight: 10
url: /ja/net/aspose.zip/archive/
---
## Archive class

このクラスは、zip アーカイブ ファイルを表します。これを使用して、zip アーカイブを作成、抽出、または更新します。

```csharp
public class Archive : IArchive
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [Archive](archive/#constructor)(ArchiveEntrySettings) | の新しいインスタンスを初期化します`Archive`エントリのオプション設定を持つクラス. |
| [Archive](archive/#constructor_1)(Stream, ArchiveLoadOptions, ArchiveEntrySettings) | の新しいインスタンスを初期化します`Archive`クラスと構成エントリのリストは、アーカイブから抽出できます。 |
| [Archive](archive/#constructor_2)(string, ArchiveLoadOptions, ArchiveEntrySettings) | の新しいインスタンスを初期化します`Archive`クラスと構成エントリのリストは、アーカイブから抽出できます。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Entries](../../aspose.zip/archive/entries/) { get; } | のエントリを取得します[`ArchiveEntry`](../archiveentry/)アーカイブを構成するタイプ. |
| [NewEntrySettings](../../aspose.zip/archive/newentrysettings/) { get; } | 新たに追加された圧縮と暗号化の設定[`ArchiveEntry`](../archiveentry/)items. |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries)(DirectoryInfo, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries_1)(string, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_1)(string, Stream, ArchiveEntrySettings) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry)(string, FileInfo, bool, ArchiveEntrySettings) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_2)(string, Stream, ArchiveEntrySettings, FileSystemInfo) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_3)(string, string, bool, ArchiveEntrySettings) | アーカイブ内に単一のエントリを作成します。 |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry)(ArchiveEntry) | エントリ リストから特定のエントリの最初の出現を削除します。 |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry_1)(int) | インデックスによってエントリ リストからエントリを削除します。 |
| [Dispose](../../aspose.zip/archive/dispose/)() | アンマネージ リソースの解放、解放、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [ExtractToDirectory](../../aspose.zip/archive/extracttodirectory/)(string) | アーカイブ内のすべてのファイルを指定されたディレクトリに抽出します。 |
| [Save](../../aspose.zip/archive/save/#save)(Stream, ArchiveSaveOptions) | 提供されたストリームにアーカイブを保存します。 |
| [Save](../../aspose.zip/archive/save/#save_1)(string, ArchiveSaveOptions) | 指定された宛先ファイルにアーカイブを保存します。 |
| [SaveSplit](../../aspose.zip/archive/savesplit/)(string, SplitArchiveSaveOptions) | 指定された宛先ディレクトリにマルチボリューム アーカイブを保存します。 |

### 関連項目

* interface [IArchive](../iarchive/)
* 名前空間 [Aspose.Zip](../../aspose.zip/)
* 組み立て [Aspose.Zip](../../)


