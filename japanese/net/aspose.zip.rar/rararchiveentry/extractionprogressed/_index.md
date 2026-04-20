---
title: RarArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP for .NET API リファレンス
description: RarArchiveEntry イベント. raw ストリームの一部が抽出されたときに発生します
type: docs
weight: 80
url: /ja/net/aspose.zip.rar/rararchiveentry/extractionprogressed/
---
## RarArchiveEntry.ExtractionProgressed event

raw ストリームの一部が抽出されたときに発生します。

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### 備考

イベント送信者は[`RarArchiveEntry`](../)実例。

### 例

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((RarArchiveEntry)s).UncompressedSize); };
```

### 関連項目

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [RarArchiveEntry](../)
* 名前空間 [Aspose.Zip.Rar](../../rararchiveentry/)
* 組み立て [Aspose.Zip](../../../)


