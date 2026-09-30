---
title: "クラス CpioEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Cpio.CpioEntry クラス。cpio アーカイブ内の単一ファイルを表します"
type: docs
weight: 420
url: /ja/net/aspose.zip.cpio/cpioentry/
---
## CpioEntry class

cpio アーカイブ内の単一ファイルを表します。

```csharp
public sealed class CpioEntry : IArchiveFileEntry
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [IsDirectory](../../aspose.zip.cpio/cpioentry/isdirectory/) { get; } | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [LastWriteTimeUtc](../../aspose.zip.cpio/cpioentry/lastwritetimeutc/) { get; } | 最後の書き込み時刻を取得します。 |
| [Length](../../aspose.zip.cpio/cpioentry/length/) { get; } | エントリの長さ（バイト単位）を取得します。 |
| [Name](../../aspose.zip.cpio/cpioentry/name/) { get; } | アーカイブ内エントリの名前を取得します。 |
| [Parent](../../aspose.zip.cpio/cpioentry/parent/) { get; } | エントリが属するアーカイブを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Extract](../../aspose.zip.cpio/cpioentry/extract/#extract_1)(Stream) | エントリを提供されたストリームに抽出します。 |
| [Extract](../../aspose.zip.cpio/cpioentry/extract/#extract)(string) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [Open](../../aspose.zip.cpio/cpioentry/open/)() | エントリを抽出用に開き、エントリの内容を含むストリームを提供します。 |
| override [ToString](../../aspose.zip.cpio/cpioentry/tostring/)() |  |

### 関連項目

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* assembly [Aspose.Zip](../../)


