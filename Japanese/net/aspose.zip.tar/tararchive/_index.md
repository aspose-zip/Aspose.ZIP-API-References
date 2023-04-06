---
title: Class TarArchive
second_title: Aspose.ZIP for .NET API リファレンス
description: Aspose.Zip.Tar.TarArchive クラス. このクラスは tar アーカイブ ファイルを表します tar アーカイブの作成抽出または更新に使用します
type: docs
weight: 730
url: /ja/net/aspose.zip.tar/tararchive/
---
## TarArchive class

このクラスは tar アーカイブ ファイルを表します。 tar アーカイブの作成、抽出、または更新に使用します。

```csharp
public class TarArchive : IArchive
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [TarArchive](tararchive/#constructor)() | の新しいインスタンスを初期化します`TarArchive`class. |
| [TarArchive](tararchive/#constructor_1)(Stream) | の新しいインスタンスを初期化します[`Archive`](../../aspose.zip/archive/)クラスと構成エントリのリストは、アーカイブから抽出できます。 |
| [TarArchive](tararchive/#constructor_2)(string) | の新しいインスタンスを初期化します`TarArchive`クラスと構成エントリのリストは、アーカイブから抽出できます。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries/) { get; } | のエントリを取得します[`TarEntry`](../tarentry/)アーカイブを構成するタイプ. |

## メソッド

| 名前 | 説明 |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip)(Stream) | 提供された gzip アーカイブを抽出して構成します`TarArchive`抽出されたデータから. |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip_1)(string) | 提供された gzip アーカイブを抽出して構成します`TarArchive`抽出されたデータから. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip)(Stream) | 提供された lzip アーカイブを抽出して構成します`TarArchive`抽出されたデータから. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip_1)(string) | 提供された lzip アーカイブを抽出して構成します`TarArchive`抽出されたデータから. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz)(Stream) | 提供された xz 形式のアーカイブを抽出し、構成します`TarArchive`抽出されたデータから. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz_1)(string) | 提供された xz 形式のアーカイブを抽出し、構成します`TarArchive`抽出されたデータから. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz)(Stream) | 提供された Z 形式のアーカイブを抽出し、構成します`TarArchive`抽出されたデータから. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz_1)(string) | 提供された Z 形式のアーカイブを抽出し、構成します`TarArchive`抽出されたデータから. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries)(DirectoryInfo, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries_1)(string, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry)(string, FileInfo, bool) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_1)(string, Stream, FileSystemInfo) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_2)(string, string, bool) | アーカイブ内に単一のエントリを作成します。 |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry_1)(int) | インデックスによってエントリ リストからエントリを削除します。 |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry)(TarEntry) | エントリ リストから特定のエントリの最初の出現を削除します。 |
| [Dispose](../../aspose.zip.tar/tararchive/dispose/)() | アンマネージ リソースの解放、解放、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory/)(string) | アーカイブ内のすべてのファイルを指定されたディレクトリに抽出します。 |
| [Save](../../aspose.zip.tar/tararchive/save/#save)(Stream, TarFormat?) | 提供されたストリームにアーカイブを保存します。 |
| [Save](../../aspose.zip.tar/tararchive/save/#save_1)(string, TarFormat?) | 指定された宛先ファイルにアーカイブを保存します。 |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped)(Stream, TarFormat?) | gzip 圧縮でアーカイブをストリームに保存します。 |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped_1)(string, TarFormat?) | アーカイブを gzip 圧縮のパスでファイルに保存します。 |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped)(Stream, TarFormat?) | アーカイブを lzip 圧縮でストリームに保存します。 |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped_1)(string, TarFormat?) | アーカイブを lzip 圧縮のパスでファイルに保存します。 |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | xz 圧縮でアーカイブをストリームに保存します。 |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed_1)(string, TarFormat?, XzArchiveSettings) | xz 圧縮でパスごとにアーカイブをパスに保存します。 |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed)(Stream, TarFormat?) | アーカイブを Z 圧縮でストリームに保存します。 |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed_1)(string, TarFormat?) | アーカイブを Z 圧縮でパスごとにパスに保存します。 |

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* 名前空間 [Aspose.Zip.Tar](../../aspose.zip.tar/)
* 組み立て [Aspose.Zip](../../)


