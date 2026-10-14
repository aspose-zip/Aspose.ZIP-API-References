---
title: "クラス SevenZipArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.SevenZip.SevenZipArchive クラス。このクラスは 7z アーカイブファイルを表します。7z アーカイブの作成と抽出に使用します。"
type: docs
weight: 1190
url: /ja/net/aspose.zip.sevenzip/sevenziparchive/
---
## SevenZipArchive class

このクラスは 7z アーカイブファイルを表します。7z アーカイブの作成と抽出に使用します。

```csharp
public class SevenZipArchive : IArchive
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [SevenZipArchive](sevenziparchive/#constructor)(SevenZipEntrySettings) | `SevenZipArchive` クラスの新しいインスタンスを、エントリのオプション設定とともに初期化します。 |
| [SevenZipArchive](sevenziparchive/#constructor_1)(Stream, SevenZipLoadOptions) | `SevenZipArchive` クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。 |
| [SevenZipArchive](sevenziparchive/#constructor_2)(Stream, string) | `SevenZipArchive` クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。 |
| [SevenZipArchive](sevenziparchive/#constructor_3)(string, SevenZipLoadOptions) | `SevenZipArchive` クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。 |
| [SevenZipArchive](sevenziparchive/#constructor_4)(string, string) | `SevenZipArchive` クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。 |
| [SevenZipArchive](sevenziparchive/#constructor_5)(string[], string) | マルチボリューム 7z アーカイブから `SevenZipArchive` クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Entries](../../aspose.zip.sevenzip/sevenziparchive/entries/) { get; } | アーカイブを構成する [`SevenZipArchiveEntry`](../sevenziparchiveentry/) 型のエントリを取得します。 |
| [NewEntrySettings](../../aspose.zip.sevenzip/sevenziparchive/newentrysettings/) { get; } | 新しく追加された [`SevenZipArchiveEntry`](../sevenziparchiveentry/) アイテムに使用される圧縮および暗号化設定です。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries)(DirectoryInfo, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries_1)(string, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry)(string, Func&lt;Stream&gt;, SevenZipEntrySettings) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_2)(string, Stream, SevenZipEntrySettings) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_1)(string, FileInfo, bool, SevenZipEntrySettings) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_3)(string, Stream, SevenZipEntrySettings, FileSystemInfo) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_4)(string, string, bool, SevenZipEntrySettings) | アーカイブ内に単一のエントリを作成します。 |
| [Dispose](../../aspose.zip.sevenzip/sevenziparchive/dispose/)() | アンマネージド リソースの解放、リリース、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [ExtractToDirectory](../../aspose.zip.sevenzip/sevenziparchive/extracttodirectory/)(string, string) | アーカイブ内のすべてのファイルを指定されたディレクトリに抽出します。 |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save)(Stream, SevenZipArchiveSaveOptions) | 提供されたストリームに 7z アーカイブを保存します。 |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save_1)(string, SevenZipArchiveSaveOptions) | 提供された宛先ファイルにアーカイブを保存します。 |
| [SaveSplit](../../aspose.zip.sevenzip/sevenziparchive/savesplit/)(string, SplitSevenZipArchiveSaveOptions) | 指定された宛先ディレクトリにマルチボリューム アーカイブを保存します。 |

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* assembly [Aspose.Zip](../../)


