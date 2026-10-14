---
title: "SevenZipArchiveEntry.CompressionProgressed"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SevenZipArchiveEntry イベント。生ストリームの一部が圧縮されたときに発生します"
type: docs
weight: 70
url: /ja/net/aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/
---
## SevenZipArchiveEntry.CompressionProgressed event

生ストリームの一部が圧縮されたときに発生します。

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## 備考

イベント送信者は [`SevenZipArchiveEntry`](../) インスタンスです。

LZMA2 エントリに対して、ソリッドモードおよびマルチスレッドモードでは呼び出されません。

## 例

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### 関連項目

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [SevenZipArchiveEntry](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* assembly [Aspose.Zip](../../../)


