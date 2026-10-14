---
title: "ArchiveLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ArchiveLoadOptions プロパティ。いくつかのバイトが抽出されたときに呼び出されるデリゲートを取得または設定します"
type: docs
weight: 50
url: /ja/net/aspose.zip/archiveloadoptions/entryextractionprogressed/
---
## ArchiveLoadOptions.EntryExtractionProgressed property

バイトが抽出されたときに呼び出されるデリゲートを取得または設定します。

```csharp
public EventHandler<ProgressCancelEventArgs> EntryExtractionProgressed { get; set; }
```

## 備考

イベント送信者は抽出が進行中の [`ArchiveEntry`](../../archiveentry/) インスタンスです。

## 例

エントリ抽出の進行状況を追跡します。

```csharp
var archive = new Archive("archive.zip", 
new ArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); } })                 
```

一定時間後にエントリ抽出をキャンセルします。

```csharp
Stopwatch watch = Stopwatch.StartNew();
using (Archive a = new Archive("big.zip", new ArchiveLoadOptions() {
    EntryExtractionProgressed = (s, e) => { if (watch.ElapsedMilliseconds > 1000) e.Cancel = true; } }))
{
    a.Entries[0].Extract("first.bin");
}
```

### 関連項目

* class [ProgressCancelEventArgs](../../progresscanceleventargs/)
* class [ArchiveLoadOptions](../)
* namespace [Aspose.Zip](../../archiveloadoptions/)
* assembly [Aspose.Zip](../../../)


