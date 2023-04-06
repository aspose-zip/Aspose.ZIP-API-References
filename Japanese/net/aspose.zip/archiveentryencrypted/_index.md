---
title: Class ArchiveEntryEncrypted
second_title: Aspose.ZIP for .NET API リファレンス
description: Aspose.Zip.ArchiveEntryEncrypted クラス. 暗号化で圧縮するか復号化で解凍する必要がある zip エントリ
type: docs
weight: 30
url: /ja/net/aspose.zip/archiveentryencrypted/
---
## ArchiveEntryEncrypted class

暗号化で圧縮するか、復号化で解凍する必要がある zip エントリ。

```csharp
public sealed class ArchiveEntryEncrypted : ArchiveEntry
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | アーカイブ内のエントリのコメントを取得します。 |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | 圧縮ファイルのサイズを取得します。 |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | 圧縮または解凍の設定を取得します。 |
| [EncryptionSettings](../../aspose.zip/archiveentryencrypted/encryptionsettings/) { get; } | 暗号化または復号化の設定を取得します。 |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | 最終変更日時を取得または設定します。 |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | アーカイブ内のエントリの名前を取得します。 |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | 元のファイルのサイズを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/)(Stream, string) | 提供されたストリームにエントリを抽出します。 |
| [Extract](../../aspose.zip/archiveentry/extract/)(string, string) | 提供されたパスによってファイルシステムへのエントリを抽出します. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | エントリを抽出用に開き、圧縮解除されたエントリ コンテンツを含むストリームを提供します。 |

## イベント

| 名前 | 説明 |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | raw ストリームの一部が圧縮されたときに発生します。 |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | raw ストリームの一部が抽出されたときに発生します。 |

### 関連項目

* class [ArchiveEntry](../archiveentry/)
* 名前空間 [Aspose.Zip](../../aspose.zip/)
* 組み立て [Aspose.Zip](../../)


