---
title: ArchiveLoadOptions.EntryListed
second_title: .NET API 참조용 Aspose.ZIP
description: ArchiveLoadOptions 재산. 목차에 항목이 나열될 때 호출되는 대리자를 가져오거나 설정합니다.
type: docs
weight: 50
url: /ko/net/aspose.zip/archiveloadoptions/entrylisted/
---
## ArchiveLoadOptions.EntryListed property

목차에 항목이 나열될 때 호출되는 대리자를 가져오거나 설정합니다.

```csharp
public EventHandler<EntryEventArgs> EntryListed { get; set; }
```

### 예

```csharp
Archive archive = new Archive("archive.zip", new ArchiveLoadOptions() { EntryListed = (s, e) => { Console.WriteLine(e.Entry.Name); } });
```

### 또한보십시오

* class [EntryEventArgs](../../entryeventargs/)
* class [ArchiveLoadOptions](../)
* 네임스페이스 [Aspose.Zip](../../archiveloadoptions/)
* 집회 [Aspose.Zip](../../../)


