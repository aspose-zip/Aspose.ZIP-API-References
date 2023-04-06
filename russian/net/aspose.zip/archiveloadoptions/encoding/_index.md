---
title: ArchiveLoadOptions.Encoding
second_title: Aspose.ZIP для справочника API .NET
description: ArchiveLoadOptions свойство. Получает или задает кодировку имен записей.
type: docs
weight: 30
url: /ru/net/aspose.zip/archiveloadoptions/encoding/
---
## ArchiveLoadOptions.Encoding property

Получает или задает кодировку имен записей.

```csharp
public Encoding Encoding { get; set; }
```

### Примеры

Имя записи, составленное с использованием указанной кодировки независимо от свойств zip-файла.

```csharp
using (FileStream fs = File.OpenRead("archive.zip"))
{      
    using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(932) }))
    {
        string name = archive.Entries[0].Name;
    }    
}
```

### Смотрите также

* class [ArchiveLoadOptions](../)
* пространство имен [Aspose.Zip](../../archiveloadoptions/)
* сборка [Aspose.Zip](../../../)


