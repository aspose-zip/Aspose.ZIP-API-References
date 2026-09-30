---
title: "XarFileEntry.CompressionProgressed"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "XarFileEntry イベント。生ストリームの一部が圧縮されたときに発生します"
type: docs
weight: 20
url: /ja/net/aspose.zip.xar/xarfileentry/compressionprogressed/
---
## XarFileEntry.CompressionProgressed event

生ストリームの一部が圧縮されたときに発生します。

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## 備考

イベント送信元は [`XarFileEntry`](../) インスタンスです。

## 例

```csharp
archive.Entries.First().CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### 関連項目

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
* assembly [Aspose.Zip](../../../)


