---
title: "クラス XarFileEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Xar.XarFileEntry クラス。xar アーカイブ内のファイルエントリを表します。"
type: docs
weight: 1470
url: /ja/net/aspose.zip.xar/xarfileentry/
---
## XarFileEntry class

xar アーカイブ内のファイル エントリを表します。

```csharp
public sealed class XarFileEntry : XarEntry, IArchiveFileEntry
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [CreationTime](../../aspose.zip.xar/xarentry/creationtime/) { get; } | ファイルまたはディレクトリの作成時刻を取得します。 |
| [FullPath](../../aspose.zip.xar/xarentry/fullpath/) { get; } | アーカイブ内のエントリのフルパスを取得します。 |
| [IsDirectory](../../aspose.zip.xar/xarentry/isdirectory/) { get; } | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [LastAccessTime](../../aspose.zip.xar/xarentry/lastaccesstime/) { get; } | ファイルまたはディレクトリの最終アクセス時刻を取得します。 |
| [Length](../../aspose.zip.xar/xarfileentry/length/) { get; } | エントリの長さ（バイト単位）を取得します。 |
| [ModificationTime](../../aspose.zip.xar/xarentry/modificationtime/) { get; } | ファイルまたはディレクトリの更新日時を取得します。 |
| [Name](../../aspose.zip.xar/xarentry/name/) { get; } | アーカイブ内エントリの名前を取得します。 |
| [Parent](../../aspose.zip.xar/xarentry/parent/) { get; } | エントリが属する親ディレクトリを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract_1)(Stream) | エントリを提供されたストリームに抽出します。 |
| [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract)(string) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [Open](../../aspose.zip.xar/xarfileentry/open/)() | エントリを抽出用に開き、エントリの内容を含むストリームを提供します。 |
| override [ToString](../../aspose.zip.xar/xarentry/tostring/)() |  |

## イベント

| 名前 | 説明 |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.xar/xarfileentry/compressionprogressed/) | 生ストリームの一部が圧縮されたときに発生します。 |

### 関連項目

* class [XarEntry](../xarentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Xar](../../aspose.zip.xar/)
* assembly [Aspose.Zip](../../)


