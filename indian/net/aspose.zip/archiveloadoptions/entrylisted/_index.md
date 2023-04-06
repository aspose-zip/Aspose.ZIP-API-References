---
title: ArchiveLoadOptions.EntryListed
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: ArchiveLoadOptions संपत्त. समग्र क तलक के भतर सूचबद्ध एक प्रवष्ट हने पर नमत प्रतनध क प्रप्त य सेट करत है
type: docs
weight: 50
url: /hi/net/aspose.zip/archiveloadoptions/entrylisted/
---
## ArchiveLoadOptions.EntryListed property

सामग्री की तालिका के भीतर सूचीबद्ध एक प्रविष्टि होने पर नामित प्रतिनिधि को प्राप्त या सेट करता है।

```csharp
public EventHandler<EntryEventArgs> EntryListed { get; set; }
```

### उदाहरण

```csharp
Archive archive = new Archive("archive.zip", new ArchiveLoadOptions() { EntryListed = (s, e) => { Console.WriteLine(e.Entry.Name); } });
```

### यह सभी देखें

* class [EntryEventArgs](../../entryeventargs/)
* class [ArchiveLoadOptions](../)
* नाम स्थान [Aspose.Zip](../../archiveloadoptions/)
* सभा [Aspose.Zip](../../../)


