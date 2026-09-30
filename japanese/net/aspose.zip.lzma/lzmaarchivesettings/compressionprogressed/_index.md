---
title: "LzmaArchiveSettings.CompressionProgressed"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "LzmaArchiveSettings イベント。生ストリームの一部が圧縮されたときに発生します"
type: docs
weight: 50
url: /ja/net/aspose.zip.lzma/lzmaarchivesettings/compressionprogressed/
---
## LzmaArchiveSettings.CompressionProgressed event

生ストリームの一部が圧縮されたときに発生します。

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## 例

```csharp
lzmaArchiveSettings.CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### 関連項目

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


