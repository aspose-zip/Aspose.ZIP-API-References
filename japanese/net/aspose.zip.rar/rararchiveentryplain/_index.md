---
title: "クラス RarArchiveEntryPlain"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Rar.RarArchiveEntryPlain クラス。復号せずに展開する必要がある Rar エントリ"
type: docs
weight: 820
url: /ja/net/aspose.zip.rar/rararchiveentryplain/
---
## RarArchiveEntryPlain class

復号せずに解凍する必要がある Rar エントリです。

```csharp
public sealed class RarArchiveEntryPlain : RarArchiveEntry
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [CompressedSize](../../aspose.zip.rar/rararchiveentry/compressedsize/) { get; } | 圧縮ファイルのサイズを取得します。 |
| [CreationTime](../../aspose.zip.rar/rararchiveentry/creationtime/) { get; } | 作成日時を取得します。 |
| [IsDirectory](../../aspose.zip.rar/rararchiveentry/isdirectory/) { get; } | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [LastAccessTime](../../aspose.zip.rar/rararchiveentry/lastaccesstime/) { get; } | 最終アクセス日時を取得します。 |
| [ModificationTime](../../aspose.zip.rar/rararchiveentry/modificationtime/) { get; } | 最終更新日時を取得します。 |
| [Name](../../aspose.zip.rar/rararchiveentry/name/) { get; } | アーカイブ内エントリの名前を取得します。 |
| [UncompressedSize](../../aspose.zip.rar/rararchiveentry/uncompressedsize/) { get; } | 元のファイルのサイズを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/)(Stream, string) | エントリを提供されたストリームに抽出します。 |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/)(string, string) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [Open](../../aspose.zip.rar/rararchiveentry/open/)(string) | エントリを抽出用に開き、解凍されたエントリ内容を含むストリームを提供します。 |

## イベント

| 名前 | 説明 |
| --- | --- |
| event [ExtractionProgressed](../../aspose.zip.rar/rararchiveentry/extractionprogressed/) | 生ストリームの一部が抽出されたときに発生します。 |

### 関連項目

* class [RarArchiveEntry](../rararchiveentry/)
* namespace [Aspose.Zip.Rar](../../aspose.zip.rar/)
* assembly [Aspose.Zip](../../)


