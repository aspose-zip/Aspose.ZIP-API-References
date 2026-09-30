---
title: "クラス CabEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Cab.CabEntry クラス。CAB アーカイブ内の単一ファイルを表します。"
type: docs
weight: 330
url: /ja/net/aspose.zip.cab/cabentry/
---
## CabEntry class

CAB アーカイブ内の単一ファイルを表します。

```csharp
public sealed class CabEntry : IArchiveFileEntry
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Length](../../aspose.zip.cab/cabentry/length/) { get; } | エントリの長さ（バイト単位）を取得します。 |
| [ModificationTime](../../aspose.zip.cab/cabentry/modificationtime/) { get; } | 最終更新日時を取得します。 |
| [Name](../../aspose.zip.cab/cabentry/name/) { get; } | アーカイブ内エントリの名前を取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Extract](../../aspose.zip.cab/cabentry/extract/#extract_1)(Stream) | エントリを提供されたストリームに抽出します。 |
| [Extract](../../aspose.zip.cab/cabentry/extract/#extract)(string) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [Open](../../aspose.zip.cab/cabentry/open/)() | エントリを抽出用に開き、エントリの内容を含むストリームを提供します。 |
| override [ToString](../../aspose.zip.cab/cabentry/tostring/)() |  |

### 関連項目

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Cab](../../aspose.zip.cab/)
* assembly [Aspose.Zip](../../)


