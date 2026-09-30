---
title: "CpioArchive クラス"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Cpio.CpioArchive クラス。このクラスは cpio アーカイブファイルを表します"
type: docs
weight: 410
url: /ja/net/aspose.zip.cpio/cpioarchive/
---
## CpioArchive class

このクラスは cpio アーカイブ ファイルを表します。

```csharp
public class CpioArchive : IArchive
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [CpioArchive](cpioarchive/#constructor)() | `CpioArchive` クラスの新しいインスタンスを初期化します。 |
| [CpioArchive](cpioarchive/#constructor_1)(Stream) | `CpioArchive` クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。 |
| [CpioArchive](cpioarchive/#constructor_2)(string) | `CpioArchive` クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Entries](../../aspose.zip.cpio/cpioarchive/entries/) { get; } | アーカイブを構成する [`CpioEntry`](../cpioentry/) 型のエントリを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries)(DirectoryInfo, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries_1)(string, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_1)(string, Stream) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry)(string, FileInfo, bool) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_2)(string, string, bool) | アーカイブ内に単一のエントリを作成します。 |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry)(CpioEntry) | エントリ リストから特定のエントリの最初の出現を削除します。 |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry_1)(int) | インデックスでエントリリストからエントリを削除します。 |
| [Dispose](../../aspose.zip.cpio/cpioarchive/dispose/)() | アンマネージド リソースの解放、リリース、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [ExtractToDirectory](../../aspose.zip.cpio/cpioarchive/extracttodirectory/)(string) | アーカイブ内のすべてのファイルを指定されたディレクトリに抽出します。 |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save)(Stream, CpioFormat) | アーカイブを指定されたストリームに保存します。 |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save_1)(string, CpioFormat) | 提供された宛先ファイルにアーカイブを保存します。 |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped)(Stream, CpioFormat) | gzip 圧縮でアーカイブをストリームに保存します。 |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped_1)(string, CpioFormat) | gzip 圧縮でパスで指定されたファイルにアーカイブを保存します。 |
| [SaveLzipped](../../aspose.zip.cpio/cpioarchive/savelzipped/#savelzipped)(Stream, CpioFormat) | lzip 圧縮でアーカイブをストリームに保存します。 |
| [SaveLzipped](../../aspose.zip.cpio/cpioarchive/savelzipped/#savelzipped_1)(string, CpioFormat) | lzip 圧縮でパスで指定されたファイルにアーカイブを保存します。 |
| [SaveLZMACompressed](../../aspose.zip.cpio/cpioarchive/savelzmacompressed/#savelzmacompressed)(Stream, CpioFormat) | LZMA 圧縮でアーカイブをストリームに保存します。 |
| [SaveLZMACompressed](../../aspose.zip.cpio/cpioarchive/savelzmacompressed/#savelzmacompressed_1)(string, CpioFormat) | lzma 圧縮でパスで指定したファイルにアーカイブを保存します。 |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed)(Stream, CpioFormat, XzArchiveSettings) | xz 圧縮でアーカイブをストリームに保存します。 |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed_1)(string, CpioFormat, XzArchiveSettings) | xz 圧縮でパスで指定されたパスにアーカイブを保存します。 |
| [SaveZCompressed](../../aspose.zip.cpio/cpioarchive/savezcompressed/#savezcompressed)(Stream, CpioFormat) | Z 圧縮でアーカイブをストリームに保存します。 |
| [SaveZCompressed](../../aspose.zip.cpio/cpioarchive/savezcompressed/#savezcompressed_1)(string, CpioFormat) | Z 圧縮でパスで指定されたパスにアーカイブを保存します。 |
| [SaveZstandard](../../aspose.zip.cpio/cpioarchive/savezstandard/#savezstandard)(Stream, CpioFormat) | Zstandard 圧縮を使用してストリームにアーカイブを保存します。 |
| [SaveZstandard](../../aspose.zip.cpio/cpioarchive/savezstandard/#savezstandard_1)(string, CpioFormat) | Zstandard 圧縮を使用してパスで指定されたファイルにアーカイブを保存します。 |

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* assembly [Aspose.Zip](../../)


