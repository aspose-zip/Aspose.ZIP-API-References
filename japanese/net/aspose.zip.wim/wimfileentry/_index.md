---
title: "クラス WimFileEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Wim.WimFileEntry クラス。wim アーカイブ内の単一ファイルを表します"
type: docs
weight: 1360
url: /ja/net/aspose.zip.wim/wimfileentry/
---
## WimFileEntry class

wim アーカイブ内の単一ファイルを表します。

```csharp
public sealed class WimFileEntry : WimEntry, IArchiveFileEntry
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [AlternateDataStreams](../../aspose.zip.wim/wimentry/alternatedatastreams/) { get; } | ファイルまたはディレクトリの代替データストリームの名前を取得します。 |
| [Archive](../../aspose.zip.wim/wimentry/archive/) { get; } | エントリが属するアーカイブを取得します。 |
| [ChangeTime](../../aspose.zip.wim/wimentry/changetime/) { get; } | ファイルまたはディレクトリが最後に変更された時刻を取得します。 |
| [CreationTime](../../aspose.zip.wim/wimentry/creationtime/) { get; } | ファイルまたはディレクトリの作成時刻を取得します。 |
| [FileAttributes](../../aspose.zip.wim/wimentry/fileattributes/) { get; } | ファイルまたはディレクトリの属性を取得します。 |
| [FullPath](../../aspose.zip.wim/wimentry/fullpath/) { get; } | イメージ内のエントリのフルパスを取得します。 |
| [HardLink](../../aspose.zip.wim/wimentry/hardlink/) { get; } | ファイルまたはディレクトリのハードリンク ID を取得します。 |
| [HasHardLinks](../../aspose.zip.wim/wimentry/hashardlinks/) { get; } | ファイルまたはディレクトリが別名で知られているかどうかを取得します。 |
| [Image](../../aspose.zip.wim/wimentry/image/) { get; } | エントリが属するイメージを取得します。 |
| [IsDirectory](../../aspose.zip.wim/wimentry/isdirectory/) { get; } | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [LastAccessTime](../../aspose.zip.wim/wimentry/lastaccesstime/) { get; } | ファイルまたはディレクトリの最終アクセス時刻を取得します。 |
| [Length](../../aspose.zip.wim/wimfileentry/length/) { get; } | エントリの長さ（バイト単位）を取得します。 |
| [ModificationTime](../../aspose.zip.wim/wimentry/modificationtime/) { get; } | ファイルまたはディレクトリの更新日時を取得します。 |
| [Name](../../aspose.zip.wim/wimentry/name/) { get; } | イメージ内のエントリ名を取得します。 |
| [Parent](../../aspose.zip.wim/wimentry/parent/) { get; } | エントリが属する親ディレクトリを取得します。 |
| [ShortName](../../aspose.zip.wim/wimentry/shortname/) { get; } | イメージ内のエントリの短い名前を取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Extract](../../aspose.zip.wim/wimfileentry/extract/#extract_1)(Stream) | エントリを提供されたストリームに抽出します。 |
| [Extract](../../aspose.zip.wim/wimfileentry/extract/#extract)(string) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [Open](../../aspose.zip.wim/wimfileentry/open/)() | エントリを抽出用に開き、エントリの内容を含むストリームを提供します。 |
| override [ToString](../../aspose.zip.wim/wimentry/tostring/)() |  |

### 関連項目

* class [WimEntry](../wimentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Wim](../../aspose.zip.wim/)
* assembly [Aspose.Zip](../../)


