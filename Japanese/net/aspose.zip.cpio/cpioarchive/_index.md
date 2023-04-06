---
title: Class CpioArchive
second_title: Aspose.ZIP for .NET API リファレンス
description: Aspose.Zip.Cpio.CpioArchive クラス. このクラスはcpio アーカイブ ファイルを表します
type: docs
weight: 160
url: /ja/net/aspose.zip.cpio/cpioarchive/
---
## CpioArchive class

このクラスは、cpio アーカイブ ファイルを表します。

```csharp
public class CpioArchive : IArchive
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [CpioArchive](cpioarchive/#constructor)() | の新しいインスタンスを初期化します`CpioArchive`class. |
| [CpioArchive](cpioarchive/#constructor_1)(Stream) | の新しいインスタンスを初期化します`CpioArchive`クラスと構成エントリのリストは、アーカイブから抽出できます。 |
| [CpioArchive](cpioarchive/#constructor_2)(string) | の新しいインスタンスを初期化します`CpioArchive`クラスと構成エントリのリストは、アーカイブから抽出できます。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Entries](../../aspose.zip.cpio/cpioarchive/entries/) { get; } | のエントリを取得します[`CpioEntry`](../cpioentry/)アーカイブを構成するタイプ. |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries)(DirectoryInfo, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries_1)(string, bool) | 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。 |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_1)(string, Stream) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry)(string, FileInfo, bool) | アーカイブ内に単一のエントリを作成します。 |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_2)(string, string, bool) | アーカイブ内に単一のエントリを作成します。 |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry)(CpioEntry) | エントリ リストから特定のエントリの最初の出現を削除します。 |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry_1)(int) | インデックスによってエントリ リストからエントリを削除します。 |
| [Dispose](../../aspose.zip.cpio/cpioarchive/dispose/)() | アンマネージ リソースの解放、解放、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [ExtractToDirectory](../../aspose.zip.cpio/cpioarchive/extracttodirectory/)(string) | アーカイブ内のすべてのファイルを指定されたディレクトリに抽出します。 |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save)(Stream, CpioFormat) | 提供されたストリームにアーカイブを保存します。 |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save_1)(string, CpioFormat) | 指定された宛先ファイルにアーカイブを保存します。 |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped)(Stream, CpioFormat) | gzip 圧縮でアーカイブをストリームに保存します。 |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped_1)(string, CpioFormat) | アーカイブを gzip 圧縮のパスでファイルに保存します。 |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed)(Stream, CpioFormat, XzArchiveSettings) | xz 圧縮でアーカイブをストリームに保存します。 |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed_1)(string, CpioFormat, XzArchiveSettings) | xz 圧縮でパスごとにアーカイブをパスに保存します。 |

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* 名前空間 [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* 組み立て [Aspose.Zip](../../)


