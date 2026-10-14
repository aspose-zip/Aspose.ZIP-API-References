---
title: "ArchiveEntry.CompressionProgressed"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ArchiveEntry イベント。生ストリームの一部が圧縮されたときに発生します"
type: docs
weight: 90
url: /ja/net/aspose.zip/archiveentry/compressionprogressed/
---
## ArchiveEntry.CompressionProgressed event

生ストリームの一部が圧縮されたときに発生します。

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## 備考

イベント送信者は [`ArchiveEntry`](../) インスタンスです。

## 例

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### 関連項目

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* namespace [Aspose.Zip](../../archiveentry/)
* assembly [Aspose.Zip](../../../)


