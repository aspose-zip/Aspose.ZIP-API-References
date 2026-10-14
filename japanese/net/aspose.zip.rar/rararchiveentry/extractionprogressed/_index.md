---
title: "RarArchiveEntry.ExtractionProgressed"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "RarArchiveEntry イベント。生ストリームの一部が抽出されたときに発生します"
type: docs
weight: 80
url: /ja/net/aspose.zip.rar/rararchiveentry/extractionprogressed/
---
## RarArchiveEntry.ExtractionProgressed event

生ストリームの一部が抽出されたときに発生します。

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## 備考

イベント送信者は [`RarArchiveEntry`](../) インスタンスです。

## 例

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((RarArchiveEntry)s).UncompressedSize); };
```

### 関連項目

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [RarArchiveEntry](../)
* namespace [Aspose.Zip.Rar](../../rararchiveentry/)
* assembly [Aspose.Zip](../../../)


