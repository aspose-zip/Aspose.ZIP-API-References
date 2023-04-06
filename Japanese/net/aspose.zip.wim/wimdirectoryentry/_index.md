---
title: Class WimDirectoryEntry
second_title: Aspose.ZIP for .NET API リファレンス
description: Aspose.Zip.Wim.WimDirectoryEntry クラス. wim アーカイブ内の単一のディレクトリを表します
type: docs
weight: 770
url: /ja/net/aspose.zip.wim/wimdirectoryentry/
---
## WimDirectoryEntry class

wim アーカイブ内の単一のディレクトリを表します。

```csharp
public sealed class WimDirectoryEntry : WimEntry
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [AllEntries](../../aspose.zip.wim/wimdirectoryentry/allentries/) { get; } | のすべてのエントリを取得します[`WimEntry`](../wimentry/)ディレクトリを再帰的に構成する型. |
| [AlternateDataStreams](../../aspose.zip.wim/wimentry/alternatedatastreams/) { get; } | ファイルまたはディレクトリの代替データ ストリームの名前を取得します。 |
| [Archive](../../aspose.zip.wim/wimentry/archive/) { get; } | エントリが属するアーカイブを取得します。 |
| [ChangeTime](../../aspose.zip.wim/wimentry/changetime/) { get; } | ファイルまたはディレクトリが最後に変更された時刻を取得します。 |
| [CreationTime](../../aspose.zip.wim/wimentry/creationtime/) { get; } | ファイルまたはディレクトリの作成時刻を取得します。 |
| [Directories](../../aspose.zip.wim/wimdirectoryentry/directories/) { get; } | のエントリを取得します`WimDirectoryEntry`ディレクトリを構成する型. |
| [FileAttributes](../../aspose.zip.wim/wimentry/fileattributes/) { get; } | ファイルまたはディレクトリの属性を取得します。 |
| [Files](../../aspose.zip.wim/wimdirectoryentry/files/) { get; } | のエントリを取得します[`WimFileEntry`](../wimfileentry/)ディレクトリを構成する型. |
| [FilesAndDirectories](../../aspose.zip.wim/wimdirectoryentry/filesanddirectories/) { get; } | のエントリを取得します[`WimEntry`](../wimentry/)ディレクトリを構成する型. |
| [FullPath](../../aspose.zip.wim/wimentry/fullpath/) { get; } | 画像内のエントリのフル パスを取得します。 |
| [HardLink](../../aspose.zip.wim/wimentry/hardlink/) { get; } | ファイルまたはディレクトリのハードリンク ID を取得します。 |
| [HasHardLinks](../../aspose.zip.wim/wimentry/hashardlinks/) { get; } | ファイルまたはディレクトリが他の名前で知られているかどうかを取得します. |
| [Image](../../aspose.zip.wim/wimentry/image/) { get; } | エントリが属するイメージを取得します。 |
| [IsDirectory](../../aspose.zip.wim/wimentry/isdirectory/) { get; } | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [LastAccessTime](../../aspose.zip.wim/wimentry/lastaccesstime/) { get; } | ファイルまたはディレクトリの最終アクセス時刻を取得します。 |
| [LastWriteTime](../../aspose.zip.wim/wimentry/lastwritetime/) { get; } | ファイルまたはディレクトリの変更時刻を取得します。 |
| [Name](../../aspose.zip.wim/wimentry/name/) { get; } | 画像内のエントリの名前を取得します. |
| [Parent](../../aspose.zip.wim/wimentry/parent/) { get; } | エントリが属する親ディレクトリを取得します。 |
| [ShortName](../../aspose.zip.wim/wimentry/shortname/) { get; } | 画像内のエントリの短い名前を取得します. |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [ExtractToDirectory](../../aspose.zip.wim/wimdirectoryentry/extracttodirectory/)(string) | 現在のディレクトリ内のすべてのファイルを、指定されたディレクトリに抽出します。 |
| override [ToString](../../aspose.zip.wim/wimentry/tostring/)() |  |

### 関連項目

* class [WimEntry](../wimentry/)
* 名前空間 [Aspose.Zip.Wim](../../aspose.zip.wim/)
* 組み立て [Aspose.Zip](../../)


