---
title: ArchiveEntry.CompressionProgressed
second_title: Aspose.ZIP for .NET API リファレンス
description: ArchiveEntry イベント. raw ストリームの一部が圧縮されたときに発生します
type: docs
weight: 80
url: /ja/net/aspose.zip/archiveentry/compressionprogressed/
---
## ArchiveEntry.CompressionProgressed event

raw ストリームの一部が圧縮されたときに発生します。

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### 備考

イベント送信者は[`ArchiveEntry`](../)実例。

### 例

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### 関連項目

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* 名前空間 [Aspose.Zip](../../archiveentry/)
* 組み立て [Aspose.Zip](../../../)


