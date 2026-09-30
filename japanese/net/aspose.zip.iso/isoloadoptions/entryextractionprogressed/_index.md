---
title: "IsoLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "IsoLoadOptions プロパティ。いくつかのバイトが抽出されたときに呼び出されるデリゲートを取得または設定します。"
type: docs
weight: 30
url: /ja/net/aspose.zip.iso/isoloadoptions/entryextractionprogressed/
---
## IsoLoadOptions.EntryExtractionProgressed property

バイトが抽出されたときに呼び出されるデリゲートを取得または設定します。

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## 備考

イベント送信者は抽出が進行している [`IsoEntry`](../../isoentry/) インスタンスです。

## 例

```csharp
IsoArchive archive = new IsoArchive("archive.iso", 
new IsoLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })                 
```

### 関連項目

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [IsoLoadOptions](../)
* namespace [Aspose.Zip.Iso](../../isoloadoptions/)
* assembly [Aspose.Zip](../../../)


