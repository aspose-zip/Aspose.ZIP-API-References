---
title: "クラス TarArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Tar.TarArchive クラス。このクラスは tar アーカイブ ファイルを表します。tar アーカイブの作成、抽出、または更新に使用します。"
type: docs
weight: 1270
url: /ja/net/aspose.zip.tar/tararchive/
---
## TarArchive class

このクラスは tar アーカイブファイルを表します。tar アーカイブの作成、抽出、または更新に使用します。

```csharp
public class TarArchive : IArchive
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [TarArchive](tararchive/#constructor)() | `TarArchive` クラスの新しいインスタンスを初期化します。 |
| [TarArchive](tararchive/#constructor_1)(Stream, TarLoadOptions) | `TarArchive` クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリ リストを作成します。 |
| [TarArchive](tararchive/#constructor_2)(string, TarLoadOptions) | `TarArchive` クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリ リストを作成します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries/) { get; } | アーカイブを構成する [`TarEntry`](../tarentry/) 型のエントリを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip)(Stream) | 提供された gzip アーカイブを展開し、抽出されたデータから `TarArchive` を作成します。 |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip_1)(string) | 提供された gzip アーカイブを展開し、抽出されたデータから `TarArchive` を作成します。 |
| static [FromLZ4](../../aspose.zip.tar/tararchive/fromlz4/#fromlz4)(Stream) | 提供された LZ4 アーカイブを展開し、抽出されたデータから `TarArchive` を作成します。 |
| static [FromLZ4](../../aspose.zip.tar/tararchive/fromlz4/#fromlz4_1)(string) | 提供された LZ4 アーカイブを展開し、抽出されたデータから `TarArchive` を作成します。 |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip)(Stream) | 提供された lzip アーカイブを展開し、抽出されたデータから `TarArchive` を作成します。 |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip_1)(string) | 提供された lzip アーカイブを展開し、抽出されたデータから `TarArchive` を作成します。 |
| static [FromLZMA](../../aspose.zip.tar/tararchive/fromlzma/#fromlzma)(Stream) | 提供された LZMA アーカイブを展開し、抽出されたデータから `TarArchive` を作成します。 |
| static [FromLZMA](../../aspose.zip.tar/tararchive/fromlzma/#fromlzma_1)(string) | 提供された LZMA アーカイブを展開し、抽出されたデータから `TarArchive` を作成します。 |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz)(Stream) | 提供された xz 形式のアーカイブを展開し、抽出されたデータから `TarArchive` を作成します。 |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz_1)(string) | 提供された xz 形式のアーカイブを展開し、抽出されたデータから `TarArchive` を作成します。 |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz)(Stream) | 提供された Z 形式のアーカイブを展開し、抽出されたデータから `TarArchive` を作成します。 |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz_1)(string) | 提供された Z 形式のアーカイブを展開し、抽出されたデータから `TarArchive` を作成します。 |
| static [FromZstandard](../../aspose.zip.tar/tararchive/fromzstandard/#fromzstandard)(Stream) | 提供された Zstandard アーカイブを展開し、抽出されたデータから `TarArchive` を作成します。 |
| static [FromZstandard](../../aspose.zip.tar/tararchive/fromzstandard/#fromzstandard_1)(string) | 提供された Zstandard アーカイブを展開し、抽出されたデータから `TarArchive` を作成します。 |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries)(DirectoryInfo, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries_1)(string, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry)(string, FileInfo, bool) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_1)(string, Stream, FileSystemInfo) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_2)(string, string, bool) | アーカイブ内に単一のエントリを作成します。 |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry_1)(int) | インデックスでエントリリストからエントリを削除します。 |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry)(TarEntry) | エントリ リストから特定のエントリの最初の出現を削除します。 |
| [Dispose](../../aspose.zip.tar/tararchive/dispose/)() | アンマネージド リソースの解放、リリース、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory/)(string) | アーカイブ内のすべてのファイルを指定されたディレクトリに抽出します。 |
| [Save](../../aspose.zip.tar/tararchive/save/#save)(Stream, TarFormat?) | アーカイブを指定されたストリームに保存します。 |
| [Save](../../aspose.zip.tar/tararchive/save/#save_1)(string, TarFormat?) | 提供された宛先ファイルにアーカイブを保存します。 |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped)(Stream, TarFormat?) | gzip 圧縮でアーカイブをストリームに保存します。 |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped_1)(string, TarFormat?) | gzip 圧縮でパスで指定されたファイルにアーカイブを保存します。 |
| [SaveLZ4Compressed](../../aspose.zip.tar/tararchive/savelz4compressed/#savelz4compressed)(Stream, TarFormat?) | LZ4 圧縮でアーカイブをストリームに保存します。 |
| [SaveLZ4Compressed](../../aspose.zip.tar/tararchive/savelz4compressed/#savelz4compressed_1)(string, TarFormat?) | LZ4 圧縮でパスで指定されたファイルにアーカイブを保存します。 |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped)(Stream, TarFormat?) | lzip 圧縮でアーカイブをストリームに保存します。 |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped_1)(string, TarFormat?) | lzip 圧縮でパスで指定されたファイルにアーカイブを保存します。 |
| [SaveLZMACompressed](../../aspose.zip.tar/tararchive/savelzmacompressed/#savelzmacompressed)(Stream, TarFormat?) | LZMA 圧縮でアーカイブをストリームに保存します。 |
| [SaveLZMACompressed](../../aspose.zip.tar/tararchive/savelzmacompressed/#savelzmacompressed_1)(string, TarFormat?) | lzma 圧縮でパスで指定されたファイルにアーカイブを保存します。 |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | xz 圧縮でアーカイブをストリームに保存します。 |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed_1)(string, TarFormat?, XzArchiveSettings) | xz 圧縮でパスで指定されたパスにアーカイブを保存します。 |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed)(Stream, TarFormat?) | Z 圧縮でアーカイブをストリームに保存します。 |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed_1)(string, TarFormat?) | Z 圧縮でパスで指定されたパスにアーカイブを保存します。 |
| [SaveZstandard](../../aspose.zip.tar/tararchive/savezstandard/#savezstandard)(Stream, TarFormat?) | Zstandard 圧縮を使用してストリームにアーカイブを保存します。 |
| [SaveZstandard](../../aspose.zip.tar/tararchive/savezstandard/#savezstandard_1)(string, TarFormat?) | Zstandard 圧縮を使用してパスで指定されたファイルにアーカイブを保存します。 |

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Tar](../../aspose.zip.tar/)
* assembly [Aspose.Zip](../../)


