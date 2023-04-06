---
title: Class CpioEntry
second_title: Aspose.ZIP for .NET API リファレンス
description: Aspose.Zip.Cpio.CpioEntry クラス. cpio アーカイブ内の単一ファイルを表します
type: docs
weight: 170
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
| [LastWriteTimeUtc](../../aspose.zip.cpio/cpioentry/lastwritetimeutc/) { get; } | 最終書き込み時刻を取得します。 |
| [Length](../../aspose.zip.cpio/cpioentry/length/) { get; } | エントリの長さをバイト単位で取得します。 |
| [Name](../../aspose.zip.cpio/cpioentry/name/) { get; } | アーカイブ内のエントリの名前を取得します。 |
| [Parent](../../aspose.zip.cpio/cpioentry/parent/) { get; } | エントリが属するアーカイブを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Extract](../../aspose.zip.cpio/cpioentry/extract/#extract_1)(Stream) | 提供されたストリームにエントリを抽出します。 |
| [Extract](../../aspose.zip.cpio/cpioentry/extract/#extract)(string) | 提供されたパスによってファイルシステムへのエントリを抽出します. |
| [Open](../../aspose.zip.cpio/cpioentry/open/)() | エントリを抽出用に開き、ストリームにエントリ コンテンツを提供します。 |
| override [ToString](../../aspose.zip.cpio/cpioentry/tostring/)() |  |

### 関連項目

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* 名前空間 [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* 組み立て [Aspose.Zip](../../)


