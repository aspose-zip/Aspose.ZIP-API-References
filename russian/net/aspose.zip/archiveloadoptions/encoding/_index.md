---
title: "ArchiveLoadOptions.Encoding"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Свойство ArchiveLoadOptions. Возвращает или задает кодировку для имён записей"
type: docs
weight: 40
url: /ru/net/aspose.zip/archiveloadoptions/encoding/
---
## ArchiveLoadOptions.Encoding property

Получает или задает кодировку для имён записей.

```csharp
public Encoding Encoding { get; set; }
```

## Примеры

Имя записи формируется с использованием указанной кодировки независимо от свойств zip‑файла.

```csharp
using (FileStream fs = File.OpenRead("archive.zip"))
{      
    using (var archive = new Archive(fs, new ArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(932) }))
    {
        string name = archive.Entries[0].Name;
    }    
}
```

### См. также

* class [ArchiveLoadOptions](../)
* namespace [Aspose.Zip](../../archiveloadoptions/)
* assembly [Aspose.Zip](../../../)


