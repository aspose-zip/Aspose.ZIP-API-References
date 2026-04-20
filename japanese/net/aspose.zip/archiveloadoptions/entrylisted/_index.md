---
title: ArchiveLoadOptions.EntryListed
second_title: Aspose.ZIP for .NET API リファレンス
description: ArchiveLoadOptions 財産. エントリが目次内にリストされたときに呼び出されるデリゲートを取得または設定します
type: docs
weight: 50
url: /ja/net/aspose.zip/archiveloadoptions/entrylisted/
---
## ArchiveLoadOptions.EntryListed property

エントリが目次内にリストされたときに呼び出されるデリゲートを取得または設定します。

```csharp
public EventHandler<EntryEventArgs> EntryListed { get; set; }
```

### 例

```csharp
Archive archive = new Archive("archive.zip", new ArchiveLoadOptions() { EntryListed = (s, e) => { Console.WriteLine(e.Entry.Name); } });
```

### 関連項目

* class [EntryEventArgs](../../entryeventargs/)
* class [ArchiveLoadOptions](../)
* 名前空間 [Aspose.Zip](../../archiveloadoptions/)
* 組み立て [Aspose.Zip](../../../)


