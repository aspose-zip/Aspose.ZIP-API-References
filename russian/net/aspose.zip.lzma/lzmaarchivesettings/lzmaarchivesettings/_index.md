---
title: "LzmaArchiveSettings.LzmaArchiveSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор LzmaArchiveSettings. Инициализирует новый экземпляр класса LzmaArchiveSettings с размером словаря по умолчанию 16 мегабайт, количеством быстрых байтов 32 и количеством битов контекста литералов 3."
type: docs
weight: 10
url: /ru/net/aspose.zip.lzma/lzmaarchivesettings/lzmaarchivesettings/
---
## LzmaArchiveSettings constructor

Инициализирует новый экземпляр класса [`LzmaArchiveSettings`](../) с размером словаря по умолчанию 16 мегабайт, количеством быстрых байтов 32 и количеством битов контекста литералов 3.

```csharp
public LzmaArchiveSettings()
```

## Примеры

```csharp
using (LzmaArchive archive = new LzmaArchive(new LzmaArchiveSettings() { DictionarySize = 1048576 })
{
    archive.SetSource("data.bin");
    archive.Save(lzmaFile);
}
```

### См. также

* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


