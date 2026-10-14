---
title: "クラス AlzEntryEncrypted"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Alz.AlzEntryEncrypted クラス。解凍前に復号が必要な ALZ エントリ"
type: docs
weight: 40
url: /ja/net/aspose.zip.alz/alzentryencrypted/
---
## AlzEntryEncrypted class

解凍前に復号が必要な ALZ エントリ。

```csharp
public sealed class AlzEntryEncrypted : AlzEntry
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
| [Extract](../../aspose.zip.alz/alzentry/extract/)(Stream, string) | エントリを提供されたストリームに抽出します。 |
| [Extract](../../aspose.zip.alz/alzentry/extract/)(string, string) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | エントリを抽出用に開き、解凍されたエントリ内容を含むストリームを提供します。 |

### 関連項目

* class [AlzEntry](../alzentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


