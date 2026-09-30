---
title: "Bzip2SaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Bzip2SaveOptions イベント。生ストリームの一部が圧縮されたときに発生します。"
type: docs
weight: 40
url: /ja/net/aspose.zip.bzip2/bzip2saveoptions/compressionprogressed/
---
## Bzip2SaveOptions.CompressionProgressed event

生ストリームの一部が圧縮されたときに発生します。

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## 備考

マルチスレッドモードで圧縮する場合、このイベントは発生しません。

## 例

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### 関連項目

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


