---
title: SevenZipArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP for .NET API リファレンス
description: SevenZipArchiveEntry イベント. raw ストリームの一部が圧縮されたときに発生します
type: docs
weight: 70
url: /ja/net/aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/
---
## SevenZipArchiveEntry.CompressionProgressed event

raw ストリームの一部が圧縮されたときに発生します。

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### 備考

イベント送信者は[`SevenZipArchiveEntry`](../)実例。

### 例

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### 関連項目

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [SevenZipArchiveEntry](../)
* 名前空間 [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* 組み立て [Aspose.Zip](../../../)


