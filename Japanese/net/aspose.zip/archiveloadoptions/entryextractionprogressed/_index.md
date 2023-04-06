---
title: ArchiveLoadOptions.EntryExtractionProgressed
second_title: Aspose.ZIP for .NET API リファレンス
description: ArchiveLoadOptions 財産. 一部のバイトが抽出されたときに呼び出されるデリゲートを取得または設定します
type: docs
weight: 40
url: /ja/net/aspose.zip/archiveloadoptions/entryextractionprogressed/
---
## ArchiveLoadOptions.EntryExtractionProgressed property

一部のバイトが抽出されたときに呼び出されるデリゲートを取得または設定します。

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

### 備考

イベント送信者は[`ArchiveEntry`](../../archiveentry/)抽出が進行するインスタンス。

### 例

```csharp
Archive archive = new Archive("archive.zip", 
new ArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); } })                 
```

### 関連項目

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveLoadOptions](../)
* 名前空間 [Aspose.Zip](../../archiveloadoptions/)
* 組み立て [Aspose.Zip](../../../)


