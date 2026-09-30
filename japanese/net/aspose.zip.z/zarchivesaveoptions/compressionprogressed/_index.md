---
title: "ZArchiveSaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ZArchiveSaveOptions イベント。生ストリームの一部が圧縮されたときに発生します"
type: docs
weight: 20
url: /ja/net/aspose.zip.z/zarchivesaveoptions/compressionprogressed/
---
## ZArchiveSaveOptions.CompressionProgressed event

生ストリームの一部が圧縮されたときに発生します。

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## 例

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### 関連項目

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveSaveOptions](../)
* namespace [Aspose.Zip.Z](../../zarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


