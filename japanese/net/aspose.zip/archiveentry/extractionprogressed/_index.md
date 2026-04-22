---
title: ArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP for .NET API リファレンス
description: ArchiveEntry イベント. raw ストリームの一部が抽出されたときに発生します
type: docs
weight: 90
url: /ja/net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

raw ストリームの一部が抽出されたときに発生します。

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### 備考

イベント送信者は[`ArchiveEntry`](../)実例。

### 例

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

### 関連項目

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* 名前空間 [Aspose.Zip](../../archiveentry/)
* 組み立て [Aspose.Zip](../../../)


