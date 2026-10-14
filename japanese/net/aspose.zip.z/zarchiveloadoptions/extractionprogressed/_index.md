---
title: "ZArchiveLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ZArchiveLoadOptions イベント。いくつかのバイトが抽出されたときに呼び出されるデリゲートを取得または設定します"
type: docs
weight: 30
url: /ja/net/aspose.zip.z/zarchiveloadoptions/extractionprogressed/
---
## ZArchiveLoadOptions.ExtractionProgressed event

バイトが抽出されたときに呼び出されるデリゲートを取得または設定します。

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## 備考

イベント送信者は抽出が進行している [`ZArchive`](../../zarchive/) インスタンスです。

## 例

```csharp
ZArchive archive = new ZArchive("archive.z", 
new ZArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### 関連項目

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveLoadOptions](../)
* namespace [Aspose.Zip.Z](../../zarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


