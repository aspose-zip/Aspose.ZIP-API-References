---
title: Class XarFileEntry
second_title: Aspose.ZIP for .NET API リファレンス
description: Aspose.Zip.Xar.XarFileEntry クラス. xar アーカイブ内のファイル エントリを表します
type: docs
weight: 840
url: /ja/net/aspose.zip.xar/xarfileentry/
---
## XarFileEntry class

xar アーカイブ内のファイル エントリを表します。

```csharp
public abstract class XarFileEntry : XarEntry, IArchiveFileEntry
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [CreationTime](../../aspose.zip.xar/xarentry/creationtime/) { get; } | ファイルまたはディレクトリの作成時刻を取得します。 |
| [FullPath](../../aspose.zip.xar/xarentry/fullpath/) { get; } | アーカイブ内のエントリのフル パスを取得します。 |
| [IsDirectory](../../aspose.zip.xar/xarentry/isdirectory/) { get; } | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [LastAccessTime](../../aspose.zip.xar/xarentry/lastaccesstime/) { get; } | ファイルまたはディレクトリの最終アクセス時刻を取得します。 |
| [LastWriteTime](../../aspose.zip.xar/xarentry/lastwritetime/) { get; } | ファイルまたはディレクトリの変更時刻を取得します。 |
| abstract [Length](../../aspose.zip.xar/xarfileentry/length/) { get; } | エントリの長さをバイト単位で取得します。 |
| [Name](../../aspose.zip.xar/xarentry/name/) { get; } | アーカイブ内のエントリの名前を取得します。 |
| [Parent](../../aspose.zip.xar/xarentry/parent/) { get; } | エントリが属する親ディレクトリを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract_1)(Stream) | 提供されたストリームにエントリを抽出します。 |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract)(string) | 提供されたパスによってファイルシステムへのエントリを抽出します. |
| abstract [Open](../../aspose.zip.xar/xarfileentry/open/)() | エントリを抽出用に開き、ストリームにエントリ コンテンツを提供します。 |
| override [ToString](../../aspose.zip.xar/xarentry/tostring/)() |  |

### 関連項目

* class [XarEntry](../xarentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* 名前空間 [Aspose.Zip.Xar](../../aspose.zip.xar/)
* 組み立て [Aspose.Zip](../../)


