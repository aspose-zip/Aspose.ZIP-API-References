---
title: Class SevenZipArchiveEntryPlain
second_title: Aspose.ZIP for .NET API リファレンス
description: Aspose.Zip.SevenZip.SevenZipArchiveEntryPlain クラス. 暗号化せずに圧縮するか復号化せずに解凍する必要がある SevenZip エントリ
type: docs
weight: 690
url: /ja/net/aspose.zip.sevenzip/sevenziparchiveentryplain/
---
## SevenZipArchiveEntryPlain class

暗号化せずに圧縮するか、復号化せずに解凍する必要がある SevenZip エントリ。

```csharp
public class SevenZipArchiveEntryPlain : SevenZipArchiveEntry
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | 圧縮ファイルのサイズを取得します。 |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | 圧縮または解凍の設定を取得します。 |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | エントリがディレクトリを表すかどうかを示す値を取得します。 |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | 最終更新日時を取得します。 |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | アーカイブ内のエントリの名前を取得します。 |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | 元のファイルのサイズを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/)(Stream, string) | 提供されたストリームにエントリを抽出します。 |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/)(string, string) | 提供されたパスによってファイルシステムへのエントリを抽出します. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | エントリを抽出用に開き、ストリームにエントリ コンテンツを提供します。 |

## イベント

| 名前 | 説明 |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | raw ストリームの一部が圧縮されたときに発生します。 |

### 関連項目

* class [SevenZipArchiveEntry](../sevenziparchiveentry/)
* 名前空間 [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* 組み立て [Aspose.Zip](../../)


