---
title: "ArchiveLoadOptions.EntryListed"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ArchiveLoadOptions プロパティ。目次内にエントリが列挙されたときに呼び出されるデリゲートを取得または設定します"
type: docs
weight: 60
url: /ja/net/aspose.zip/archiveloadoptions/entrylisted/
---
## ArchiveLoadOptions.EntryListed property

目次内にリストされたエントリが呼び出されたときに実行されるデリゲートを取得または設定します。

```csharp
public EventHandler<EntryEventArgs> EntryListed { get; set; }
```

## 例

```csharp
var archive = new Archive("archive.zip", new ArchiveLoadOptions() { EntryListed = (s, e) => { Console.WriteLine(e.Entry.Name); } });
```

### 関連項目

* class [EntryEventArgs](../../entryeventargs/)
* class [ArchiveLoadOptions](../)
* namespace [Aspose.Zip](../../archiveloadoptions/)
* assembly [Aspose.Zip](../../../)


