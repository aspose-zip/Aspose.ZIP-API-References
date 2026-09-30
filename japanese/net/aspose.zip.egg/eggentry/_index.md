---
title: "EggEntry クラス"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Egg.EggEntry クラス。EGG アーカイブ内のファイルエントリをすべてのメタデータと共に表します"
type: docs
weight: 470
url: /ja/net/aspose.zip.egg/eggentry/
---
## EggEntry class

すべてのメタデータを含む EGG アーカイブ内のファイルエントリを表します。

```csharp
public abstract class EggEntry : IArchiveFileEntry
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [CompressedSize](../../aspose.zip.egg/eggentry/compressedsize/) { get; } | エントリの圧縮サイズを取得します。 |
| [IsDirectory](../../aspose.zip.egg/eggentry/isdirectory/) { get; } | このエントリがディレクトリを表すかどうかを示す値を取得します。 |
| [Length](../../aspose.zip.egg/eggentry/length/) { get; } |  |
| [ModificationTime](../../aspose.zip.egg/eggentry/modificationtime/) { get; } | 最終更新日時を取得または設定します。 |
| [Name](../../aspose.zip.egg/eggentry/name/) { get; } | アーカイブ内のエントリ名を取得します。 |
| [UncompressedSize](../../aspose.zip.egg/eggentry/uncompressedsize/) { get; } | エントリの非圧縮サイズを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract_1)(Stream) | エントリを提供されたストリームに抽出します。 |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract)(string) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [Open](../../aspose.zip.egg/eggentry/open/)() | エントリを抽出用に開き、解凍されたエントリ内容を含むストリームを提供します。 |

### 関連項目

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Egg](../../aspose.zip.egg/)
* assembly [Aspose.Zip](../../)


