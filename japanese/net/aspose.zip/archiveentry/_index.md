---
title: "クラス ArchiveEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.ArchiveEntry クラス。アーカイブ内の単一ファイルを表します"
type: docs
weight: 170
url: /ja/net/aspose.zip/archiveentry/
---
## ArchiveEntry class

アーカイブ内の単一ファイルを表します。

```csharp
public abstract class ArchiveEntry : IArchiveFileEntry
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | アーカイブ内エントリのコメントを取得します。 |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | 圧縮されたファイルのサイズを取得します。 |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | 圧縮または解凍の設定を取得します。 |
| [DataSource](../../aspose.zip/archiveentry/datasource/) { get; } | エントリがアーカイブに追加された場合のソースで、抽出されたものではありません。 |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | 最終更新日時を取得または設定します。 |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | アーカイブ内エントリの名前を取得します。 |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | 元のファイルのサイズを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/#extract_1)(Stream, string) | エントリを提供されたストリームに抽出します。 |
| [Extract](../../aspose.zip/archiveentry/extract/#extract)(string, string) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [Open](../../aspose.zip/archiveentry/open/)(string) | エントリを抽出用に開き、解凍されたエントリ内容を含むストリームを提供します。 |

## イベント

| 名前 | 説明 |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | 生ストリームの一部が圧縮されたときに発生します。 |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | 生ストリームの一部が抽出されたときに発生します。 |

## 備考

`ArchiveEntry` インスタンスを [`ArchiveEntryEncrypted`](../archiveentryencrypted/) にキャストして、エントリが暗号化されているかどうかを判断します。

### 関連項目

* interface [IArchiveFileEntry](../iarchivefileentry/)
* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)


