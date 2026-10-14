---
title: "クラス AlzEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Alz.AlzEntry クラス。すべてのメタデータを含む ALZ アーカイブ内のファイルエントリを表します"
type: docs
weight: 30
url: /ja/net/aspose.zip.alz/alzentry/
---
## AlzEntry class

ALZ アーカイブ内のファイル エントリをすべてのメタデータとともに表します。

```csharp
public abstract class AlzEntry : IArchiveFileEntry
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [CompressedSize](../../aspose.zip.alz/alzentry/compressedsize/) { get; } | ファイルデータの圧縮サイズ（バイト単位）。 |
| [IsDirectory](../../aspose.zip.alz/alzentry/isdirectory/) { get; } | このエントリがディレクトリを表す場合は true を返します。 |
| [Length](../../aspose.zip.alz/alzentry/length/) { get; } |  |
| [Name](../../aspose.zip.alz/alzentry/name/) { get; } | ファイル名（パスなし）。 |
| [UncompressedSize](../../aspose.zip.alz/alzentry/uncompressedsize/) { get; } | ファイルデータの非圧縮サイズ（バイト単位）。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract_1)(Stream, string) | エントリを提供されたストリームに抽出します。 |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract)(string, string) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | エントリを抽出用に開き、解凍されたエントリ内容を含むストリームを提供します。 |

### 関連項目

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


