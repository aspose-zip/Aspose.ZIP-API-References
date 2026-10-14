---
title: "クラス XarDirectoryEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Xar.XarDirectoryEntry クラス。xar アーカイブ内のディレクトリエントリを表します"
type: docs
weight: 1450
url: /ja/net/aspose.zip.xar/xardirectoryentry/
---
## XarDirectoryEntry class

xar アーカイブ内のディレクトリ エントリを表します。

```csharp
public sealed class XarDirectoryEntry : XarEntry
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [AllEntries](../../aspose.zip.xar/xardirectoryentry/allentries/) { get; } | ディレクトリを構成するすべての [`XarEntry`](../xarentry/) タイプのエントリを再帰的に取得します。 |
| [CreationTime](../../aspose.zip.xar/xarentry/creationtime/) { get; } | ファイルまたはディレクトリの作成時刻を取得します。 |
| [Directories](../../aspose.zip.xar/xardirectoryentry/directories/) { get; } | `XarDirectoryEntry` タイプのエントリを取得し、ディレクトリを構成します。 |
| [Files](../../aspose.zip.xar/xardirectoryentry/files/) { get; } | ディレクトリを構成する [`XarFileEntry`](../xarfileentry/) タイプのエントリを取得します。 |
| [FilesAndDirectories](../../aspose.zip.xar/xardirectoryentry/filesanddirectories/) { get; } | ディレクトリを構成する [`XarEntry`](../xarentry/) タイプのエントリを取得します。 |
| [FullPath](../../aspose.zip.xar/xarentry/fullpath/) { get; } | アーカイブ内のエントリのフルパスを取得します。 |
| [IsDirectory](../../aspose.zip.xar/xarentry/isdirectory/) { get; } | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [LastAccessTime](../../aspose.zip.xar/xarentry/lastaccesstime/) { get; } | ファイルまたはディレクトリの最終アクセス時刻を取得します。 |
| [ModificationTime](../../aspose.zip.xar/xarentry/modificationtime/) { get; } | ファイルまたはディレクトリの更新日時を取得します。 |
| [Name](../../aspose.zip.xar/xarentry/name/) { get; } | アーカイブ内エントリの名前を取得します。 |
| [Parent](../../aspose.zip.xar/xarentry/parent/) { get; } | エントリが属する親ディレクトリを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [ExtractToDirectory](../../aspose.zip.xar/xardirectoryentry/extracttodirectory/)(string) | 現在のディレクトリ内のすべてのファイルを、指定されたディレクトリへ抽出します。 |
| override [ToString](../../aspose.zip.xar/xarentry/tostring/)() |  |

### 関連項目

* class [XarEntry](../xarentry/)
* namespace [Aspose.Zip.Xar](../../aspose.zip.xar/)
* assembly [Aspose.Zip](../../)


