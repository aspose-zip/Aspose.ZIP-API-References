---
title: "AlzArchiveLoadOptions.Encoding"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Свойство AlzArchiveLoadOptions. Получает или задает кодировку для имён записей. По умолчанию Korean Windows code page 949 CP949"
type: docs
weight: 40
url: /ru/net/aspose.zip.alz/alzarchiveloadoptions/encoding/
---
## AlzArchiveLoadOptions.Encoding property

Получает или задает кодировку имен записей. По умолчанию используется корейская кодовая страница Windows 949 (CP949).

```csharp
public Encoding Encoding { get; set; }
```

## Примечания

Архивы ALZ исторически сохраняют имена файлов, используя кодовую страницу Korean Windows ANSI.

## Примеры

Имя записи сформировано с использованием указанной кодировки.

```csharp
using (FileStream fs = File.OpenRead("archive.alz"))
{
    using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(949) }))
    {
        string name = archive.Entries[0].Name;
    }
}
```

### См. также

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


