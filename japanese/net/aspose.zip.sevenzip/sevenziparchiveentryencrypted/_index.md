---
title: "クラス SevenZipArchiveEntryEncrypted"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.SevenZip.SevenZipArchiveEntryEncrypted クラス。暗号化して圧縮するか、復号化して解凍する必要がある SevenZip アーカイブエントリです"
type: docs
weight: 1210
url: /ja/net/aspose.zip.sevenzip/sevenziparchiveentryencrypted/
---
## SevenZipArchiveEntryEncrypted class

暗号化して圧縮するか、復号化して解凍する必要がある SevenZip アーカイブエントリです。

```csharp
public class SevenZipArchiveEntryEncrypted : SevenZipArchiveEntry
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | 圧縮ファイルのサイズを取得します。 |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | 圧縮または解凍の設定を取得します。 |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | 最終更新日時を取得します。 |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | アーカイブ内エントリの名前を取得します。 |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | 元のファイルのサイズを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/)(Stream, string) | エントリを提供されたストリームに抽出します。 |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/)(string, string) | エントリを提供されたパスでファイルシステムに抽出します。 |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | エントリを抽出用に開き、エントリの内容を含むストリームを提供します。 |

## イベント

| 名前 | 説明 |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | 生ストリームの一部が圧縮されたときに発生します。 |

### 関連項目

* class [SevenZipArchiveEntry](../sevenziparchiveentry/)
* namespace [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* assembly [Aspose.Zip](../../)


