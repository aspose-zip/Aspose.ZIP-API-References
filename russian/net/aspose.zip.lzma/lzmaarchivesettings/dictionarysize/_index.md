---
title: "LzmaArchiveSettings.DictionarySize"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Свойство LzmaArchiveSettings. Размер буфера истории словаря указывает, сколько байтов недавно обработанных несжатых данных хранится в памяти. Если не задан, будет выбран в соответствии с размером записи"
type: docs
weight: 20
url: /ru/net/aspose.zip.lzma/lzmaarchivesettings/dictionarysize/
---
## LzmaArchiveSettings.DictionarySize property

Размер словаря (буфера истории) указывает, сколько байтов недавно обработанных несжатых данных хранится в памяти. Если не задан, будет выбран в соответствии с размером записи.

```csharp
public int DictionarySize { get; set; }
```

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | Значение слишком маленькое или слишком большое. |
| ArgumentException | Значение не является степенью двойки или тройным произведением степени двойки. |

## Примечания

Чем больше словарь, тем обычно лучше коэффициент сжатия — но словари, превышающие размер несжатых данных, являются пустой тратой ОЗУ.

Размер словаря LZMA-архива должен быть либо степенью двойки (2^n), либо в три раза больше степени двойки (3*2^n).

### См. также

* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


