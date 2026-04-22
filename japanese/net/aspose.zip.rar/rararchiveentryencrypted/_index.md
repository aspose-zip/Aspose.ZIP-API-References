---
title: Class RarArchiveEntryEncrypted
second_title: Aspose.ZIP for .NET API リファレンス
description: Aspose.Zip.Rar.RarArchiveEntryEncrypted クラス. 復号化で解凍する必要がある zip エントリ.
type: docs
weight: 330
url: /ja/net/aspose.zip.rar/rararchiveentryencrypted/
---
## RarArchiveEntryEncrypted class

復号化で解凍する必要がある zip エントリ.

```csharp
public sealed class RarArchiveEntryEncrypted : RarArchiveEntry
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [CompressedSize](../../aspose.zip.rar/rararchiveentry/compressedsize/) { get; } | 圧縮ファイルのサイズを取得します。 |
| [CreationTime](../../aspose.zip.rar/rararchiveentry/creationtime/) { get; } | 作成日時を取得します。 |
| [IsDirectory](../../aspose.zip.rar/rararchiveentry/isdirectory/) { get; } | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [LastAccessTime](../../aspose.zip.rar/rararchiveentry/lastaccesstime/) { get; } | 最終アクセス日時を取得します。 |
| [ModificationTime](../../aspose.zip.rar/rararchiveentry/modificationtime/) { get; } | 最終更新日時を取得します。 |
| [Name](../../aspose.zip.rar/rararchiveentry/name/) { get; } | アーカイブ内のエントリの名前を取得します。 |
| [UncompressedSize](../../aspose.zip.rar/rararchiveentry/uncompressedsize/) { get; } | 元のファイルのサイズを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/)(Stream, string) | 提供されたストリームにエントリを抽出します。 |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/)(string, string) | 提供されたパスによってファイルシステムへのエントリを抽出します. |
| [Open](../../aspose.zip.rar/rararchiveentry/open/)(string) | エントリを抽出用に開き、圧縮解除されたエントリ コンテンツを含むストリームを提供します。 |

## イベント

| 名前 | 説明 |
| --- | --- |
| event [ExtractionProgressed](../../aspose.zip.rar/rararchiveentry/extractionprogressed/) | raw ストリームの一部が抽出されたときに発生します。 |

### 関連項目

* class [RarArchiveEntry](../rararchiveentry/)
* 名前空間 [Aspose.Zip.Rar](../../aspose.zip.rar/)
* 組み立て [Aspose.Zip](../../)


