---
title: "クラス TarEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Tar.TarEntry クラス。tar アーカイブ内の単一ファイルを表します"
type: docs
weight: 1280
url: /ja/net/aspose.zip.tar/tarentry/
---
## TarEntry class

tar アーカイブ内の単一ファイルを表します。

```csharp
public class TarEntry : IArchiveFileEntry
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [IsDirectory](../../aspose.zip.tar/tarentry/isdirectory/) { get; } | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [Length](../../aspose.zip.tar/tarentry/length/) { get; } | エントリの長さをバイト単位で取得します。 |
| [ModificationTime](../../aspose.zip.tar/tarentry/modificationtime/) { get; } | ファイルまたはディレクトリの更新日時を取得します。 |
| [Name](../../aspose.zip.tar/tarentry/name/) { get; set; } | アーカイブ内のエントリの名前を取得または設定します。 |
| [UncompressedSize](../../aspose.zip.tar/tarentry/uncompressedsize/) { get; } | 元のファイルのサイズを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Extract](../../aspose.zip.tar/tarentry/extract/#extract_1)(Stream) | エントリを提供されたストリームに抽出します。 |
| [Extract](../../aspose.zip.tar/tarentry/extract/#extract)(string) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [Open](../../aspose.zip.tar/tarentry/open/)() | エントリを抽出用に開き、エントリの内容を含むストリームを提供します。 |

### 関連項目

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Tar](../../aspose.zip.tar/)
* assembly [Aspose.Zip](../../)


