---
title: Class GzipArchive
second_title: Aspose.ZIP for .NET API リファレンス
description: Aspose.Zip.Gzip.GzipArchive クラス. このクラスは gzip アーカイブ ファイルを表しますこれを使用してgzip アーカイブを作成または抽出します
type: docs
weight: 210
url: /ja/net/aspose.zip.gzip/gziparchive/
---
## GzipArchive class

このクラスは gzip アーカイブ ファイルを表します。これを使用して、gzip アーカイブを作成または抽出します。

```csharp
public class GzipArchive : IArchive, IArchiveFileEntry
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [GzipArchive](gziparchive/#constructor)() | の新しいインスタンスを初期化します`GzipArchive`圧縮用に準備されたクラス. |
| [GzipArchive](gziparchive/#constructor_1)(Stream, bool) | の新しいインスタンスを初期化します`GzipArchive`解凍用に準備されたクラス. |
| [GzipArchive](gziparchive/#constructor_2)(string, bool) | の新しいインスタンスを初期化します`GzipArchive`class. |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Name](../../aspose.zip.gzip/gziparchive/name/) { get; } | 元のファイル名. |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Dispose](../../aspose.zip.gzip/gziparchive/dispose/)() | アンマネージ リソースの解放、解放、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/)(Stream) | 提供されたストリームにアーカイブを抽出します。 |
| [Open](../../aspose.zip.gzip/gziparchive/open/)() | 抽出のためにアーカイブを開き、アーカイブ コンテンツを含むストリームを提供します。 |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save)(Stream) | 提供されたストリームにアーカイブを保存します。 |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save_1)(string) | 指定された宛先ファイルにアーカイブを保存します。 |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_1)(FileInfo) | アーカイブ内で圧縮するコンテンツを設定します。 |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_2)(Stream) | アーカイブ内で圧縮するコンテンツを設定します。 |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_3)(string) | アーカイブ内で圧縮するコンテンツを設定します。 |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource)(TarArchive) | アーカイブ内で圧縮するコンテンツを設定します。 |

### 備考

Gzip 圧縮アルゴリズムは、LZ77 とハフマン コーディングを組み合わせた DEFLATE アルゴリズムに基づいています。

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* 名前空間 [Aspose.Zip.Gzip](../../aspose.zip.gzip/)
* 組み立て [Aspose.Zip](../../)


