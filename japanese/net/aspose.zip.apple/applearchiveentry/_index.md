---
title: "クラス AppleArchiveEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Apple.AppleArchiveEntry クラス。AppleArchive 内のファイルシステムエントリを表します。"
type: docs
weight: 70
url: /ja/net/aspose.zip.apple/applearchiveentry/
---
## AppleArchiveEntry class

[`AppleArchive`](../applearchive/) 内のファイルシステムエントリを表します。

```csharp
public sealed class AppleArchiveEntry : IArchiveFileEntry
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [IsDirectory](../../aspose.zip.apple/applearchiveentry/isdirectory/) { get; } | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [IsSymbolicLink](../../aspose.zip.apple/applearchiveentry/issymboliclink/) { get; } | エントリがシンボリックリンクを表すかどうかを示す値を取得します。 |
| [Length](../../aspose.zip.apple/applearchiveentry/length/) { get; } | エントリの非圧縮長さ（バイト単位）を取得します。 |
| [Name](../../aspose.zip.apple/applearchiveentry/name/) { get; } | アーカイブ内のエントリのパスを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract_1)(Stream) | エントリを提供されたストリームに抽出します。 |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract)(string) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [Open](../../aspose.zip.apple/applearchiveentry/open/)() | エントリを抽出用に開き、エントリの内容を含むストリームを提供します。 |

## 備考

このクラスのインスタンスは、既存の Apple Archive から解析された通常ファイル、ディレクトリ、またはシンボリックリンク、あるいは作成中のアーカイブに追加されたファイルやディレクトリを表すことができます。

### 関連項目

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


