---
title: "XarLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "XarLoadOptions プロパティ。バイトが抽出されたときに呼び出されるデリゲートを取得または設定します"
type: docs
weight: 30
url: /ja/net/aspose.zip.xar/xarloadoptions/entryextractionprogressed/
---
## XarLoadOptions.EntryExtractionProgressed property

バイトが抽出されたときに呼び出されるデリゲートを取得または設定します。

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## 備考

イベント送信者は、抽出が進行している [`XarFileEntry`](../../xarfileentry/) インスタンスです。

## 例

```csharp
XarArchive archive = new XarArchive("archive.xar", 
new XarLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((XarFileEntry)s).Length); } })                 
```

### 関連項目

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarLoadOptions](../)
* namespace [Aspose.Zip.Xar](../../xarloadoptions/)
* assembly [Aspose.Zip](../../../)


