---
title: "クラス WimDirectoryEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Wim.WimDirectoryEntry クラス。wim アーカイブ内の単一ディレクトリを表します。"
type: docs
weight: 1340
url: /ja/net/aspose.zip.wim/wimdirectoryentry/
---
## WimDirectoryEntry class

wim アーカイブ内の単一ディレクトリを表します。

```csharp
public sealed class WimDirectoryEntry : WimEntry
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [AllEntries](../../aspose.zip.wim/wimdirectoryentry/allentries/) { get; } | ディレクトリを再帰的に構成する [`WimEntry`](../wimentry/) 型のすべてのエントリを取得します。 |
| [AlternateDataStreams](../../aspose.zip.wim/wimentry/alternatedatastreams/) { get; } | ファイルまたはディレクトリの代替データストリームの名前を取得します。 |
| [Archive](../../aspose.zip.wim/wimentry/archive/) { get; } | エントリが属するアーカイブを取得します。 |
| [ChangeTime](../../aspose.zip.wim/wimentry/changetime/) { get; } | ファイルまたはディレクトリが最後に変更された時刻を取得します。 |
| [CreationTime](../../aspose.zip.wim/wimentry/creationtime/) { get; } | ファイルまたはディレクトリの作成時刻を取得します。 |
| [Directories](../../aspose.zip.wim/wimdirectoryentry/directories/) { get; } | `WimDirectoryEntry` 型のエントリを取得し、ディレクトリを構成します。 |
| [FileAttributes](../../aspose.zip.wim/wimentry/fileattributes/) { get; } | ファイルまたはディレクトリの属性を取得します。 |
| [Files](../../aspose.zip.wim/wimdirectoryentry/files/) { get; } | ディレクトリを構成する [`WimFileEntry`](../wimfileentry/) 型のエントリを取得します。 |
| [FilesAndDirectories](../../aspose.zip.wim/wimdirectoryentry/filesanddirectories/) { get; } | ディレクトリを構成する [`WimEntry`](../wimentry/) 型のエントリを取得します。 |
| [FullPath](../../aspose.zip.wim/wimentry/fullpath/) { get; } | イメージ内のエントリのフルパスを取得します。 |
| [HardLink](../../aspose.zip.wim/wimentry/hardlink/) { get; } | ファイルまたはディレクトリのハードリンク ID を取得します。 |
| [HasHardLinks](../../aspose.zip.wim/wimentry/hashardlinks/) { get; } | ファイルまたはディレクトリが別名で知られているかどうかを取得します。 |
| [Image](../../aspose.zip.wim/wimentry/image/) { get; } | エントリが属するイメージを取得します。 |
| [IsDirectory](../../aspose.zip.wim/wimentry/isdirectory/) { get; } | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [LastAccessTime](../../aspose.zip.wim/wimentry/lastaccesstime/) { get; } | ファイルまたはディレクトリの最終アクセス時刻を取得します。 |
| [ModificationTime](../../aspose.zip.wim/wimentry/modificationtime/) { get; } | ファイルまたはディレクトリの更新日時を取得します。 |
| [Name](../../aspose.zip.wim/wimentry/name/) { get; } | イメージ内のエントリ名を取得します。 |
| [Parent](../../aspose.zip.wim/wimentry/parent/) { get; } | エントリが属する親ディレクトリを取得します。 |
| [ShortName](../../aspose.zip.wim/wimentry/shortname/) { get; } | イメージ内のエントリの短い名前を取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [ExtractToDirectory](../../aspose.zip.wim/wimdirectoryentry/extracttodirectory/)(string) | 現在のディレクトリ内のすべてのファイルを、指定されたディレクトリへ抽出します。 |
| override [ToString](../../aspose.zip.wim/wimentry/tostring/)() |  |

### 関連項目

* class [WimEntry](../wimentry/)
* namespace [Aspose.Zip.Wim](../../aspose.zip.wim/)
* assembly [Aspose.Zip](../../)


