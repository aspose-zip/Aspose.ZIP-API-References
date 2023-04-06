---
title: Class SevenZipArchive
second_title: Aspose.ZIP for .NET API リファレンス
description: Aspose.Zip.SevenZip.SevenZipArchive クラス. このクラスは 7z アーカイブ ファイルを表しますこれを使用して7z アーカイブを構成および抽出します
type: docs
weight: 660
url: /ja/net/aspose.zip.sevenzip/sevenziparchive/
---
## SevenZipArchive class

このクラスは 7z アーカイブ ファイルを表します。これを使用して、7z アーカイブを構成および抽出します。

```csharp
public class SevenZipArchive : IArchive
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [SevenZipArchive](sevenziparchive/#constructor)(SevenZipEntrySettings) | の新しいインスタンスを初期化します`SevenZipArchive`エントリのオプション設定を持つクラス. |
| [SevenZipArchive](sevenziparchive/#constructor_1)(Stream) | の新しいインスタンスを初期化します`SevenZipArchive`クラスと構成エントリのリストは、アーカイブから抽出できます。 |
| [SevenZipArchive](sevenziparchive/#constructor_2)(string) | の新しいインスタンスを初期化します`SevenZipArchive`クラスと構成エントリのリストは、アーカイブから抽出できます。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Entries](../../aspose.zip.sevenzip/sevenziparchive/entries/) { get; } | のエントリを取得します[`SevenZipArchiveEntry`](../sevenziparchiveentry/)アーカイブを構成するタイプ. |
| [NewEntrySettings](../../aspose.zip.sevenzip/sevenziparchive/newentrysettings/) { get; } | 新たに追加された圧縮と暗号化の設定[`SevenZipArchiveEntry`](../sevenziparchiveentry/)items. |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries)(DirectoryInfo, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries_1)(string, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_1)(string, Stream, SevenZipEntrySettings) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry)(string, FileInfo, bool, SevenZipEntrySettings) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_2)(string, Stream, SevenZipEntrySettings, FileSystemInfo) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_3)(string, string, bool, SevenZipEntrySettings) | アーカイブ内に単一のエントリを作成します。 |
| [Dispose](../../aspose.zip.sevenzip/sevenziparchive/dispose/)() | アンマネージ リソースの解放、解放、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [ExtractToDirectory](../../aspose.zip.sevenzip/sevenziparchive/extracttodirectory/)(string, string) | アーカイブ内のすべてのファイルを指定されたディレクトリに抽出します。 |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save)(Stream) | 提供されたストリームに 7z アーカイブを保存します。 |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save_1)(string) | 指定された宛先ファイルにアーカイブを保存します。 |
| [SaveSplit](../../aspose.zip.sevenzip/sevenziparchive/savesplit/)(string, SplitSevenZipArchiveSaveOptions) | 指定された宛先ディレクトリにマルチボリューム アーカイブを保存します。 |

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* 名前空間 [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* 組み立て [Aspose.Zip](../../)


